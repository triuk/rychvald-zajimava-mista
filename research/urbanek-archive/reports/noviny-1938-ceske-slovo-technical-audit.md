# Technický audit `Thumbs.db` a `ZbThumbnail.info` – Noviny 1938 České slovo

Datum auditu: 2026-08-06

## Rozsah

Audit se týká dvou technických souborů kolekce:

- `Noviny 1938 České slovo/Thumbs.db`;
- `Noviny 1938 České slovo/ZbThumbnail.info`.

Oba soubory jsou evidovány jako cache či index náhledů. Nejsou klasifikovány ani OCR zpracovány jako běžné obrazové prameny.

## Ověření originálů

### `Thumbs.db`

- velikost: `132608` B;
- SHA-256: `df1156f17c3c79b2892741be41d5e54a48e07c9a11498f1378d1534db106418b`;
- Git blob SHA: `d8f7138ed11eb5131549f085cfff5d3d76986652`;
- Drive ID: `1lYNM39TGU2fPm7-2D08KPRn6JhKsy2yj`.

### `ZbThumbnail.info`

- velikost: `246456` B;
- SHA-256: `ece09ea3e2611d1fc2e6804ae23a54735d5033dd0098a0f11b8e5063fbe8b002`;
- Git blob SHA: `e3a0aae9c8fb6482818306c13a4929f709746703`;
- Drive ID: `1O_hFMBbjXqjYzQlnpzvdBFVsNztYGc31`.

U obou souborů se shoduje velikost z Google Drive s lokálním souborem a lokálně vypočtený Git blob SHA odpovídá blobu na pracovní větvi.

## Metoda

Audit zahrnoval:

1. binární identifikaci souborů a výpočet kontrolních součtů;
2. u `Thumbs.db` rozbor CFB/OLE hlavičky, FAT, MiniFAT, adresáře, mini-streamu a streamu `Catalog`;
3. dekódování všech vložených JPEG náhledů a vazby katalogových ID na datové streamy;
4. u `ZbThumbnail.info` kontrolu signatury `zbex`, vyhledání vložených JPEGů a názvů souborů v interních strukturách;
5. porovnání množiny názvů v obou cache se 33 plnými JPEGy kolekce;
6. obrazové porovnání všech cache náhledů se zmenšenými plnými originály.

## `Thumbs.db`

Soubor je CFB/OLE dokument verze 3:

- velikost sektoru: `512` B;
- velikost minisektoru: `64` B;
- katalog verze: `7`;
- deklarované položky katalogu: `34`;
- deklarovaný cílový rozměr: `96 × 96` px;
- datové obrazové streamy: `34`;
- platné JPEG streamy: `34`;
- binárně duplicitní JPEG streamy: `0`.

Jedna katalogová položka je spojena s GUID `{A42CD7B6-E9B9-4D02-B7A6-288B71AD28BA}` a obsahuje čtvercový náhled ikony složky se dvěma vloženými miniaturami novinových stran. Není to samostatný zdrojový obrázek ani důkaz chybějícího plného originálu.

Zbývajících 33 položek katalogu nese názvy plných JPEGů kolekce. Náhledy mají:

- 29krát `96 × 72` px;
- 4krát `72 × 96` px.

Množina 33 názvů se přesně shoduje s plnými JPEGy v Git a na Drive. `P1020282.JPG` se v katalogu nevyskytuje. Každý z 33 pojmenovaných náhledů má jednoznačně nejlepší obrazovou shodu se stejně pojmenovaným plným souborem.

Katalogové časy pojmenovaných položek sahají od `2013-02-15 11:36:52` do `2013-02-15 16:10:52`. Téměř kopírují časový rozsah reprodukčního fotografování, ale jsou to metadata cache, nikoli datum vydání novin nebo historické události.

## `ZbThumbnail.info`

Soubor používá vlastní binární strukturu se signaturou `zbex`:

- vložené platné JPEG náhledy: `33`;
- binárně duplicitní JPEG náhledy: `0`;
- 29 náhledů má `160 × 120` px;
- 4 náhledy mají `120 × 160` px;
- jedinečné názvy JPEGů v interních UTF-16 strukturách: `33`.

Názvy se přesně shodují s plnými soubory `P1020273.JPG` až `P1020306.JPG` s přirozenou mezerou `P1020282.JPG`. Soubor neobsahuje další jedinečný název zdrojového JPEG souboru. Všech 33 vložených náhledů bylo jednoznačně přiřazeno ke stejně pojmenovaným plným originálům podle obrazové shody.

Opakované výskyty názvů uvnitř souboru jsou součástí interních indexových a metadatových struktur; nejde o další samostatné zdrojové položky.

## Kontrola úplnosti

| Kontrola | `Thumbs.db` | `ZbThumbnail.info` |
|---|---:|---:|
| jedinečné názvy plných JPEGů | 33 | 33 |
| vložené náhledy plných JPEGů | 33 | 33 |
| názvy bez plného souboru | 0 | 0 |
| plné soubory bez názvu v cache | 0 | 0 |
| cache-only plné originály doložené souborem | 0 | 0 |
| evidence pro `P1020282.JPG` | 0 | 0 |

Obě cache pokrývají právě aktuálních 33 plných JPEGů. Neprokazují existenci chybějícího `P1020282.JPG` ani jiného plného originálu.

## Závěr

- všech 35 položek kolekce je nyní Git-ověřeno a zdrojově indexováno;
- 33 JPEGů je vizuálně klasifikováno;
- oba technické soubory jsou auditovány;
- technické cache nedokládají žádný chybějící plný originál ani další samostatný obrazový pramen;
- kolekce je v rámci aktuálního Git a Drive snapshotu uzavřena.

Audit neřeší provenienci fyzických novin, úplnost vůči materiálům mimo aktuální snapshot, přesnou posloupnost vydání a stran, autorství reprodukčních fotografií ani práva. Tyto otázky zůstávají otevřené pod `URB-U-0081`.
