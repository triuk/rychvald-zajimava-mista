# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený revizní checkpoint: `506c4a60166284f4e6f96fee14c67c5379551b4e`
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
| Druhá vizuální kontrola Českého slova | probíhá; ověřeno 26 textových jednotek |
| Řešení nejistot | centrálně evidováno |
| Ostatní tři pilotní kolekce | čekají |
| Pull request | čeká |

## Registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

Souhrn:

- `open`: 15
- `in_progress`: 1
- `deferred`: 2
- `resolved`: 4
- `not_actionable`: 1
- celkem: 22

Nově vyřešeno:

- `URB-U-0019`: poškozené slovo v článku `015` je při zvětšení čitelné jako **„dosazováni“**. Věta v tisku skutečně postrádá sloveso `jsou` a nebyla jazykově opravena.

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – klasifikace všech 31 obrazů a první OCR dokončeny.
2. `Články z Českého slova` – první OCR dokončeno, druhá kontrola probíhá.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Články z Českého slova

- 37 obrazových položek ověřeno, seskupeno a přepsáno v prvním průchodu.
- Druhou kontrolou prošlo 26 textových jednotek od `001` po `017-d`, včetně oddělených fragmentů.
- Všechny zkontrolované soubory mají stav `visually_verified`.

### Opravy z dosavadní druhé kontroly

1. `001`: odstraněny vydavatelské údaje, které na výřezu nebyly.
2. `004`: oddělena samostatná krátká zpráva `004-b2`.
3. `005`: vizuálně potvrzeno příjmení `Jarábáč`.
4. `007`: oddělen a potvrzen fragment `007-b` – **„Malhomme se vrátil“**.
5. `010`: oddělen cizí horní fragment `010-b`; jeho článek zůstává neidentifikován.
6. `015`: poškozené slovo přečteno jako `dosazováni`; `URB-U-0019` uzavřena.
7. `017-c`: do reklamního textu doplněn viditelný koncový kód `=2M.`.
8. `012–014`, `016-a`, `016-b`, `017-a`, `017-b` a `017-d` odpovídaly obrazu bez textové opravy.

## Následující přesný krok

Druhá řádková kontrola položek ze zdrojových obrazů `17.jpg–22.jpg`:

- `018`;
- `019`;
- `020`;
- `021-a`, `021-b`;
- `022-a`, `022-b`, `022-c`, `022-d`;
- `023-a`, `023-b`.

U `020` zachovat fyzické poškození vedené jako `URB-U-0020`, pokud obraz neposkytne dostatek znaků k bezpečnému doplnění. U `022-a` znovu posoudit nespojitý přechod vedený jako `URB-U-0021`.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a korekční soubor seskupení.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat pouze uvedenou revizní dávkou.
5. Po dávce commitnout každý opravený soubor a aktualizovat checkpoint.
