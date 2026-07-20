# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený OCR checkpoint: `75cd91620126f70787899912f3f11ccc150a8d1f`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a `clanky-z-ceskeho-slova-grouping-corrections.yml`.

## Neměnná rozhodnutí

- Originály nepřejmenovávat, nepřesouvat ani neupravovat.
- Chybějící nebo nečitelné části textu nedoplňovat odhadem.
- Samostatné články a fragmenty ukládat pod vlastními stabilními ID.
- Stav `visually_verified` přidělit jen po úplném porovnání s obrazem.
- Fyzicky chybějící text ponechat jako samostatnou otevřenou nejistotu.
- Každou dávku commitnout a aktualizovat stav i registr nejistot.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Technický audit a inventář | probíhá po kolekcích |
| Klasifikace větrných mlýnů | dokončena |
| První OCR Českého slova | dokončeno pro všech 37 obrazů |
| Druhá vizuální kontrola Českého slova | **dokončena pro všech 56 jednotek** |
| Řešení nejistot | centrálně evidováno |
| Ostatní tři pilotní kolekce | čekají |
| Pull request | čeká |

## Registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

- `open`: 15
- `in_progress`: 0
- `deferred`: 2
- `resolved`: 5
- `not_actionable`: 1
- celkem: 23

`URB-U-0018` je vyřešena: druhá řádková a strukturální kontrola byla dokončena pro všechny OCR jednotky Českého slova.

Nadále otevřené fyzické mezery:

- `URB-U-0020`: poškozený úsek v `19.jpg`.
- `URB-U-0021`: chybějící sloupcový přechod v `21.jpg`.
- `URB-U-0022`: poškozený blok v `33.jpg`.

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – klasifikace všech 31 obrazů a první OCR dokončeny.
2. `Články z Českého slova` – první OCR i druhá vizuální kontrola dokončeny.
3. `Ochotníci rychvald` – následuje inventář.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Články z Českého slova – uzavřený výsledek

- 37 obrazových položek bylo ověřeno, seskupeno a přepsáno.
- Druhou kontrolou prošlo 56 textových a scénických jednotek.
- Strukturální opravy zahrnují samostatné jednotky `004-b2`, `007-b`, `010-b` a `019-b`.
- `020`, `022-a` a `035` mají ověřený zachovaný text, ale otevřené fyzické lakuny.
- `025-scene-text` je potvrzen kombinací částečně čitelné tabule a úplného dobového popisku.
- V závěrečné dávce byly mimo jiné potvrzeny podoby `Karkoška`, `Karkošku`, `Karkoszky`, `Jan Žebrok`, `K. Buchta` a drobné vydavatelské údaje z 31. října 1938.
- Chybějící text nebyl nikde rekonstruován odhadem.

## Následující přesný krok

Vytvořit úplný rekurzivní inventář kolekce `Ochotníci rychvald`:

1. získat přesný obsah a strukturu z Google Drivu;
2. rozlišit obrazové soubory, dokumentové skeny a technické cache;
3. přidělit stabilní ID s prefixem `urbanek-ochotnici`;
4. ověřit přesné cesty a blob SHA v pilotní větvi;
5. teprve poté zahájit vizuální klasifikaci a OCR.

## Instrukce pro nový chat

1. Načíst autoritativní soubory.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat inventářem `Ochotníci rychvald`.
5. Po malé dokončené dávce aktualizovat checkpoint.
