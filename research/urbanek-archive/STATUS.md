# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený revizní checkpoint: `6a71d314fac4ec958174e5e99d8086162b97b770`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a korekční soubor seskupení.

## Neměnná rozhodnutí

- Originály nepřejmenovávat, nepřesouvat ani neupravovat.
- Chybějící nebo nečitelné části textu nedoplňovat odhadem.
- Samostatné články a fragmenty ukládat pod vlastními stabilními ID.
- Stav `visually_verified` lze přidělit pouze po úplném porovnání se zdrojovým obrazem.
- Strukturální opravy seskupení zapisovat do `clanky-z-ceskeho-slova-grouping-corrections.yml`.
- Každou dávku commitnout a aktualizovat stav i registr nejistot.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Technický audit a inventář | probíhá po kolekcích |
| Klasifikace větrných mlýnů | dokončena |
| První OCR Českého slova | dokončeno pro všech 37 obrazů |
| Druhá vizuální kontrola Českého slova | probíhá |
| Řešení nejistot | centrálně evidováno |
| Ostatní tři pilotní kolekce | čekají |
| Pull request | čeká |

## Registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

Souhrn:

- `open`: 17
- `in_progress`: 1
- `deferred`: 2
- `resolved`: 2
- `not_actionable`: 1
- celkem: 22

`URB-U-0018` nyní eviduje průběh druhé řádkové kontroly. `URB-U-0014` byla uzavřena: příjmení starosty je ve zdrojovém obraze čitelné jako **Jarábáč**; ověřena je podoba přepisu, nikoli nezávisle historická identita osoby.

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – klasifikace všech 31 obrazů a první OCR dokončeny.
2. `Články z Českého slova` – první OCR dokončeno, druhá kontrola probíhá.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Články z Českého slova

- 37 obrazových položek ověřeno, seskupeno a přepsáno v prvním průchodu.
- Výstupy jsou v `research/urbanek-archive/ocr/`.
- Druhou kontrolou prošly:
  - `001`;
  - `002`;
  - `003`;
  - `004-a`;
  - `004-b`;
  - nově oddělená `004-b2`;
  - `004-c`;
  - `005`.
- Všech osm jednotek má stav `visually_verified`.

### Zjištěné opravy druhé kontroly

1. `001`: odstraněny vydavatelské a kontaktní údaje, které na výřezu vůbec nejsou.
2. `004`: odstavec s novou datací `Bratislava 3. října. (er)` je samostatná zpráva a byl oddělen jako `004-b2`.
3. `005`: přepis příjmení `Jarábáč` byl potvrzen zvětšením zdrojového řádku.
4. `002`, `003` a `004-a` odpovídaly obrazu bez textové opravy.
5. U `004-c` bylo znovu potvrzeno, že je zachován pouze nadpis.

Autoritativní strukturální korekce:

`research/urbanek-archive/collections/clanky-z-ceskeho-slova-grouping-corrections.yml`

Větev byla po dokončení prvního OCR průchodu ověřena jako **114 commitů před `main` a 0 commitů za `main`**.

## Následující přesný krok

Druhá řádková kontrola položek:

- `006`;
- `007`;
- `008`;
- `009`;
- `010`;
- `011`.

Zvláštní pozornost:

- u `007` znovu posoudit oříznutý cizí nadpis vedený jako `URB-U-0015`;
- u `010` zachovat horní cizí fragment oddělený a případně zpřesnit `URB-U-0017`;
- každý úplně zkontrolovaný soubor označit `visually_verified`.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a korekční soubor seskupení.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat pouze uvedenou revizní dávkou.
5. Po dávce commitnout každý opravený soubor a aktualizovat checkpoint.
