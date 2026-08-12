# Technický audit `Thumbs.db` a `ZbThumbnail.info` – Rychvald

Datum auditu: 2026-08-10

## Rozsah

Audit se týká dvou technických souborů kolekce `Rychvald`:

- `Rychvald/Thumbs.db`;
- `Rychvald/ZbThumbnail.info`.

Nejde o samostatné obrazové prameny. Soubory jsou evidovány jako cache či index náhledů a nejsou OCR ani vizuálně klasifikovány jako běžné fotografie.

## Ověření originálů

### `Thumbs.db`

- velikost: `118784` B;
- SHA-256: `454a4259547fc55f23645817d415b42a170f433b5fafd7481cc8fb66b15fc6c1`;
- Git blob SHA: `0c3f5c8ea878fc6b97fb69c8eef9bfc2571cfb8a`;
- Drive ID: `1CfKmAAQVtb0rD4U_Wm_i3ULqCMNaO62D`.

### `ZbThumbnail.info`

- velikost: `199546` B;
- SHA-256: `f2248e577904f5b87d7d9a7cebb8c2e4b4603ccd188daf3ef86d9ffd7eeea21b`;
- Git blob SHA: `b21c21108d8b2222263c64dd21867d1f6819076c`;
- Drive ID: `1UNA35ideuDwdP7yTkZH9KBsUExLHnI7Q`.

U obou souborů odpovídá velikost staženého souboru z Google Drive velikosti v repozitáři a lokálně vypočtený Git blob SHA přesně odpovídá blobu na pracovní větvi.

## Metoda

Audit zahrnoval binární identifikaci a kontrolní součty, rozbor CFB/OLE struktur `Thumbs.db`, načtení streamu `Catalog`, dekódování vložených JPEG náhledů, kontrolu struktury se signaturou `zbex` u `ZbThumbnail.info`, vyhledání vložených JPEGů a názvů zdrojových souborů a porovnání těchto názvů s 31 plnými JPEGy kolekce.

## `Thumbs.db`

Soubor je CFB/OLE dokument verze 3:

- velikost sektoru: `512` B;
- velikost minisektoru: `64` B;
- katalog verze: `7`;
- cílový rozměr katalogu: `96 × 96` px;
- katalogových položek: `32`;
- z toho názvů zdrojových JPEGů: `31`;
- jedna položka je náhled složky s GUID `{A42CD7B6-E9B9-4D02-B7A6-288B71AD28BA}`;
- platných JPEG streamů: `32`.

Všechny názvy 31 zdrojových položek odpovídají 31 plným JPEGům kolekce. Cache neobsahuje další název zdrojového obrázku bez odpovídajícího plného souboru.

Mezi 32 JPEG streamy je jedna binární duplicita. Odpovídá známé skutečnosti, že `Budova úřadu 005.jpg` a `Kopie - Budova úřadu 005.jpg` jsou bitově totožné. Nejde tedy o nový chybějící nebo další samostatný obrazový pramen.

Rozměry vložených náhledů se liší podle poměru stran zdroje; jedna položka náhledu složky má `96 × 96` px.

## `ZbThumbnail.info`

Soubor začíná signaturou `zbex` a obsahuje:

- 31 platných JPEG náhledů;
- 30 jedinečných JPEG obsahů;
- jednu binárně duplicitní dvojici odpovídající známé duplicitě `Budova úřadu 005.jpg` / `Kopie - Budova úřadu 005.jpg`;
- názvy všech 31 plných JPEGů kolekce v interních strukturách.

Nebyl nalezen další věrohodný název zdrojového JPEG souboru, který by neměl odpovídající plný originál v aktuální kolekci.

## Kontrola úplnosti

| Kontrola | `Thumbs.db` | `ZbThumbnail.info` |
|---|---:|---:|
| názvy zdrojových JPEGů | 31 | 31 |
| vložené náhledy zdrojových JPEGů | 31 | 31 |
| položky navíc bez plného originálu | 0 | 0 |
| doložené chybějící plné originály | 0 | 0 |
| známá duplicitní dvojice 002/007 | ano | ano |

## Závěr

- všech 33 položek kolekce `Rychvald` je nyní Git-ověřeno a zdrojově indexováno;
- všech 31 obrazových souborů je klasifikováno;
- oba technické soubory jsou auditovány;
- cache nedokládají žádný další ani chybějící plný obrazový originál;
- známá binární duplicita položek 002 a 007 se promítá i do náhledových cache;
- kolekce je v rámci aktuálního Git a Drive snapshotu uzavřena.

Audit nemění otevřenou provenienční nejistotu `URB-U-0082`; přesná lokalizace, autorství, původní účel sady a práva zůstávají předmětem pozdějšího řešení.
