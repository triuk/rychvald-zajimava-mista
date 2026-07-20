# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: commit `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený pracovní checkpoint: commit `4a0f941144edb2ad2fc99456eeebf248a9eedeb7`
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
| Pilotní klasifikace | probíhá | Mlýny dokončeny; České slovo čeká seskupení stránek. |
| OCR | probíhá | Mlýny mají první přepisy; České slovo čeká na seskupení článků. |
| Draft pull request | čeká | Až po dokončení všech pěti pilotních kolekcí. |

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – **klasifikace a první OCR dokončeny**.
2. `Články z Českého slova` – **inventář, ověření cest a audit cache dokončeny; čeká seskupení a OCR**.
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

## Články z Českého slova – audit

- Na Drivu: 39 položek, z toho 37 obrazových souborů, `Thumbs.db` a `ZbThumbnail.info`.
- Kolekční inventář: `research/urbanek-archive/collections/clanky-z-ceskeho-slova-inventory.csv`.
- Všech 37 obrazových souborů bylo jednotlivě potvrzeno pod přesnými původními cestami.
- `ZbThumbnail.info` je v GitHubu přítomen.
- `Thumbs.db` je na Drivu, ale ve větvi chybí.
- Ověření cest a blob SHA jsou rozděleny do tří souborů:
  - `clanky-z-ceskeho-slova-verification-01.yml`;
  - `clanky-z-ceskeho-slova-verification-02.yml`;
  - `clanky-z-ceskeho-slova-verification-03.yml`.

### Audit `Thumbs.db`

- SHA-256 cache: `0647ec694c2bbbd6be13517d0e201f498199bd57e825b63140c4f32ae0c43800`.
- Katalog obsahuje 97 názvů a 97 platných JPEG náhledů.
- Po porovnání dekódovaných obrazů jde o 45 unikátních náhledů.
- Třicet sedm unikátních náhledů odpovídá současným souborům.
- Osm unikátních náhledů nemá v současné kolekci odpovídající plný soubor.
- Zbývajících 52 historických názvů jsou starší názvy nebo meziverze obrazů, které už v kolekci existují.
- Podrobný seznam osmi chybějících obrazů, rozměry a SHA-256: `research/urbanek-archive/reports/clanky-z-ceskeho-slova-thumbnail-cache.md`.
- Náhledy mají pouze 57–96 px, a proto nejsou vhodné pro plnohodnotný OCR přepis článků.

## Následující přesný krok

Vizuálně projít 37 obrazových souborů kolekce `Články z Českého slova`, určit pořadí a hranice jednotlivých článků nebo tematických skupin a výsledek uložit do samostatného seskupovacího souboru. Začít položkami `urbanek-ceske-slovo-001` až `011`. OCR provádět až po určení, které snímky jsou titulní listy, komentáře, celé články, pokračování nebo dílčí výřezy.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, `sources/README.md`, tento `STATUS.md` a `state.yml`.
2. Ověřit větev `agent/import-urbanek-pilot` a její aktuální hlavu.
3. Neměnit originální archivní soubory.
4. Pokračovat pouze krokem uvedeným v části **Následující přesný krok**.
5. Po malé dokončené dávce commitnout výstupy a aktualizovat oba stavové soubory.
