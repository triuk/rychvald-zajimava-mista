# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený revizní checkpoint: `38bcf6d08768ed8a253b6695ae521f47484a7985`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a `clanky-z-ceskeho-slova-grouping-corrections.yml`.

## Neměnná rozhodnutí

- Originály nepřejmenovávat, nepřesouvat ani neupravovat.
- Chybějící nebo nečitelné části textu nedoplňovat odhadem.
- Samostatné články a fragmenty ukládat pod vlastními stabilními ID.
- Stav `visually_verified` přidělit jen po úplném porovnání s obrazem.
- Strukturální opravy seskupení ukládat do korekčního souboru.
- Každou dávku commitnout a aktualizovat stav i registr nejistot.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Technický audit a inventář | probíhá po kolekcích |
| Klasifikace větrných mlýnů | dokončena |
| První OCR Českého slova | dokončeno pro všech 37 obrazů |
| Druhá vizuální kontrola Českého slova | probíhá; ověřeny položky 001–011 a nové fragmenty |
| Řešení nejistot | centrálně evidováno |
| Ostatní tři pilotní kolekce | čekají |
| Pull request | čeká |

## Registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

Souhrn:

- `open`: 16
- `in_progress`: 1
- `deferred`: 2
- `resolved`: 3
- `not_actionable`: 1
- celkem: 22

Nově vyřešeno:

- `URB-U-0015`: spodní cizí nadpis v `6.jpg` skutečně zní **„Malhomme se vrátil“**.

Stále otevřeno:

- `URB-U-0017`: horní fragment v `9.jpg` má čitelnou signaturu `-vk-`, ale nadpis ani původní článek nelze z výřezu určit.

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – klasifikace všech 31 obrazů a první OCR dokončeny.
2. `Články z Českého slova` – první OCR dokončeno, druhá kontrola probíhá.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Články z Českého slova

- 37 obrazových položek ověřeno, seskupeno a přepsáno v prvním průchodu.
- Druhou kontrolou prošly textové jednotky:
  - `001`, `002`, `003`;
  - `004-a`, `004-b`, `004-b2`, `004-c`;
  - `005`, `006`;
  - `007`, `007-b`;
  - `008`, `009`;
  - `010`, `010-b`;
  - `011`.
- Celkem je nyní `visually_verified` 16 textových jednotek.

### Opravy z druhé dávky

- `006`, `008`, `009` a `011` odpovídaly obrazu bez textové opravy.
- `007`: cizí spodní nadpis byl oddělen jako `007-b`; znění **„Malhomme se vrátil“** bylo potvrzeno.
- `010`: oříznutý konec předchozího článku byl oddělen jako `010-b`; signatura je `-vk-`, identita článku zůstává neznámá.
- Korekční soubor nyní pokrývá položky `004`, `007` a `010`.

## Následující přesný krok

Druhá řádková kontrola položek ze zdrojových obrazů `11.jpg–16.jpg`:

- `012`;
- `013`;
- `014`;
- `015`;
- `016-a`, `016-b`;
- `017-a`, `017-b`, `017-c`, `017-d`.

U `015` zachovat a znovu posoudit fyzickou lakunu `URB-U-0019`. U složených výstřižků ověřit skutečný tok sazby a hranice jednotlivých článků.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a korekční soubor seskupení.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat pouze uvedenou revizní dávkou.
5. Po dávce commitnout každý opravený soubor a aktualizovat checkpoint.
