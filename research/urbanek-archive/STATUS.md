# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: commit `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený pracovní checkpoint: commit `3026ce49e6633d9a8b7f95e54b51407515f46497`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt: potvrzeno uživatelem.

Tento soubor a `state.yml` jsou autoritativním předávacím bodem mezi chaty. Nový chat musí nejdříve načíst pravidla repozitáře, tento soubor a `state.yml` a ověřit aktuální hlavu větve.

## Neměnná rozhodnutí

- Originální soubory nepřejmenovávat, nepřesouvat ani neupravovat.
- Zachovat původní strukturu složek a názvy souborů.
- `Thumbs.db` a `ZbThumbnail.info` ponechat pro případnou další analýzu.
- Technické cache evidovat jako `technical_thumbnail_cache`; nezahrnovat je do běžné klasifikace ani OCR fotografií.
- Normalizované názvy používat pouze v inventáři nebo u odvozených pracovních výstupů.
- Fotografie zatím nevybírat do konkrétních článků.
- Každou dokončenou dávku commitnout a aktualizovat stavové soubory.

## OCR

OCR se vede odděleně jako:

1. `document_text` – články, dokumenty, popisky, titulní strany a podobné předlohy;
2. `scene_text` – nápisy na budovách, cedule, uliční tabule, pamětní desky, vývěsní štíty, plakáty, transparenty a další text zachycený ve scéně.

Strojový výstup má stav `machine_unverified`. Nečitelná místa se nedoplňují odhadem.

## Stav etap

| Etapa | Stav | Poznámka |
|---|---|---|
| Ruční import originálů | dokončeno s nesrovnalostmi | Obrazové soubory prvních dvou kolekcí jsou kompletní; chybí některé `Thumbs.db`. |
| Zachování technických cache | odloženo, zdokumentováno | Chybějící cache zůstávají na Drivu a jejich obsah je auditován. |
| Pravidla OCR včetně textu ve scéně | dokončeno | Zapsáno v `AGENTS.md`. |
| Technický audit importu | probíhá | První dvě pilotní kolekce mají dokončený inventář a ověření cest. |
| Hlavní inventář | probíhá | Mlýny jsou v hlavním inventáři; České slovo má samostatný kolekční inventář. |
| Pilotní klasifikace | probíhá | Mlýny dokončeny; všech 37 obrazů Českého slova je seskupeno podle fyzických článků. |
| OCR | probíhá | Mlýny mají první přepisy; u Českého slova jsou dokončeny položky 001 a 002. |
| Draft pull request | čeká | Až po dokončení všech pěti pilotních kolekcí. |

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – **klasifikace a první OCR dokončeny**.
2. `Články z Českého slova` – **audit a seskupení dokončeny, OCR probíhá**.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Rychvaldské větrné mlýny – souhrn

- Na Drivu: 39 položek, z toho 31 obrazových a 8 technických cache.
- V GitHubu: všech 31 obrazových souborů a 3 `ZbThumbnail.info`; chybí 5 `Thumbs.db`.
- Všech 31 obrazových souborů bylo ověřeno a klasifikováno.
- Dokončeny dva dokumentové přepisy a jeden krátký scénický nápis.
- Potvrzené binární duplicity:
  - `urbanek-mlyny-011` = `urbanek-mlyny-021`;
  - `urbanek-mlyny-012` = `urbanek-mlyny-022` = `urbanek-mlyny-039`.
- `urbanek-mlyny-018` zachycuje interiér kostela a je pravděpodobně chybně zařazen.
- Kořenový `Thumbs.db` navíc eviduje chybějící `P1010269.JPG`; z cache je obnovitelný náhled 72 × 96 px.
- Podrobný audit: `research/urbanek-archive/reports/rychvaldske-vetrne-mlyny-thumbnail-cache.md`.

## Články z Českého slova – technický audit

- Na Drivu: 39 položek, z toho 37 obrazových souborů, `Thumbs.db` a `ZbThumbnail.info`.
- Kolekční inventář: `research/urbanek-archive/collections/clanky-z-ceskeho-slova-inventory.csv`.
- Všech 37 obrazových souborů bylo jednotlivě potvrzeno pod přesnými původními cestami.
- `ZbThumbnail.info` je v GitHubu přítomen; `Thumbs.db` je na Drivu, ale ve větvi chybí.
- Ověření cest a blob SHA jsou uloženy ve třech souborech `clanky-z-ceskeho-slova-verification-01.yml` až `03.yml`.

### Audit `Thumbs.db`

- SHA-256 cache: `0647ec694c2bbbd6be13517d0e201f498199bd57e825b63140c4f32ae0c43800`.
- Katalog obsahuje 97 názvů a 97 platných JPEG náhledů.
- Po porovnání dekódovaných obrazů jde o 45 unikátních náhledů.
- Třicet sedm odpovídá současným souborům a osm nemá v současné kolekci odpovídající plný soubor.
- Podrobnosti: `research/urbanek-archive/reports/clanky-z-ceskeho-slova-thumbnail-cache.md`.

## Články z Českého slova – seskupení

Všech 37 obrazových položek bylo vizuálně rozděleno na hlavičky vydání, samostatné články, složené výstřižky, pokračování, krátké zprávy, fotografické položky a neúplné okrajové fragmenty. Výsledek je uložen ve čtyřech souborech:

- `research/urbanek-archive/collections/clanky-z-ceskeho-slova-grouping-01.yml`
- `research/urbanek-archive/collections/clanky-z-ceskeho-slova-grouping-02.yml`
- `research/urbanek-archive/collections/clanky-z-ceskeho-slova-grouping-03.yml`
- `research/urbanek-archive/collections/clanky-z-ceskeho-slova-grouping-04.yml`

Důležitá zjištění:

- číselné názvy souborů nejsou spolehlivá chronologie;
- `31 a.jpg` a `31 b.jpg` tvoří jeden pokračující článek „Milé klopoty“;
- `24.jpg` obsahuje dvě fotografie z předávání území v Rychvaldě, úplný novinový popisek a scénický nápis **„Městys Rychvald“**;
- `35.jpg` dokládá vydání `České slovo – pondělník`, 31. října 1938, ročník 10, číslo 301;
- složené výstřižky se musí při OCR přepisovat po jednotlivých článcích, nikoli jako jeden souvislý text.

## Dokončené OCR Českého slova

- `urbanek-ceske-slovo-001`: hlavička vydání **Sobota 1. října 1938**, ročník X, číslo 271.
  - `research/urbanek-archive/ocr/urbanek-ceske-slovo-001-document-text.md`
- `urbanek-ceske-slovo-002`: článek **„Zněmčilá území máme odevzdat do 10. října“**, včetně otištěného znění dohody a dodatkových prohlášení.
  - `research/urbanek-archive/ocr/urbanek-ceske-slovo-002-document-text.md`

Oba přepisy mají stav `machine_unverified` a zachovávají dobový pravopis.

## Následující přesný krok

Přepsat `urbanek-ceske-slovo-003` jako samostatný článek **„Československo odstoupí Polsku část Těšínska“**. Poté pokračovat složenou položkou `urbanek-ceske-slovo-004`, kterou je nutné rozdělit na tři samostatné textové jednotky `004-a`, `004-b` a viditelný fragment `004-c` podle `clanky-z-ceskeho-slova-grouping-01.yml`.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, `sources/README.md`, tento `STATUS.md` a `state.yml`.
2. Ověřit větev `agent/import-urbanek-pilot` a její aktuální hlavu.
3. Neměnit originální archivní soubory.
4. Pokračovat pouze krokem uvedeným v části **Následující přesný krok**.
5. Po malé dokončené dávce commitnout výstupy a aktualizovat oba stavové soubory.
