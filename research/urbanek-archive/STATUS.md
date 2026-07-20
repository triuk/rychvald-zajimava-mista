# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený revizní checkpoint: `214e0de09d030b15a39601e942d29fbb13f77dc6`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a `clanky-z-ceskeho-slova-grouping-corrections.yml`.

## Neměnná rozhodnutí

- Originály nepřejmenovávat, nepřesouvat ani neupravovat.
- Chybějící nebo nečitelné části textu nedoplňovat odhadem.
- Samostatné články a fragmenty ukládat pod vlastními stabilními ID.
- Stav `visually_verified` přidělit jen po úplném porovnání s obrazem.
- U úplně ověřeného zachovaného textu s fyzickou mezerou používat `visually_verified_with_lacuna` a ponechat příslušnou nejistotu otevřenou.
- Strukturální opravy seskupení ukládat do korekčního souboru.
- Každou dávku commitnout a aktualizovat stav i registr nejistot.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Technický audit a inventář | probíhá po kolekcích |
| Klasifikace větrných mlýnů | dokončena |
| První OCR Českého slova | dokončeno pro všech 37 obrazů |
| Druhá vizuální kontrola Českého slova | probíhá; ověřeno 38 textových jednotek |
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
- celkem: 23

Aktuální zjištění:

- `URB-U-0020` zůstává otevřená: mezi zprávou o dr. Benetkovi a zprávou o footballových hřištích v `19.jpg` je fyzicky zničený úsek bez bezpečně čitelných znaků.
- `URB-U-0021` zůstává otevřená: v `21.jpg` chybí sloupcový přechod mezi větou o deputaci z Bohumínska a blokem začínajícím `čs. národnosti`.
- Nová `URB-U-0023` eviduje neidentifikované zakončení článku `…cích. -bi-`, oddělené jako `019-b`.

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – klasifikace všech 31 obrazů a první OCR dokončeny.
2. `Články z Českého slova` – první OCR dokončeno, druhá kontrola probíhá.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Články z Českého slova

- 37 obrazových položek ověřeno, seskupeno a přepsáno v prvním průchodu.
- Druhou kontrolou prošlo 38 textových jednotek od `001` po `023-b`, včetně dodatečně oddělených fragmentů.
- `020` a `022-a` mají stav `visually_verified_with_lacuna`; veškerý zachovaný text je ověřen, fyzicky chybějící části nikoli.
- Ostatní dokončené jednotky mají stav `visually_verified`.

### Opravy z dosavadní druhé kontroly

1. `001`: odstraněny vydavatelské údaje, které na výřezu nebyly.
2. `004`: oddělena samostatná krátká zpráva `004-b2`.
3. `005`: vizuálně potvrzeno příjmení `Jarábáč`.
4. `007`: oddělen a potvrzen fragment `007-b` – **„Malhomme se vrátil“**.
5. `010`: oddělen cizí horní fragment `010-b`; jeho článek zůstává neidentifikován.
6. `015`: poškozené slovo přečteno jako `dosazováni`; `URB-U-0019` uzavřena.
7. `017-c`: do reklamního textu doplněn viditelný koncový kód `=2M.`.
8. `019`: horní zakončení jiného článku bylo odděleno jako `019-b`; vznikla `URB-U-0023`.
9. `020`: jména `Karkošky`, `Lejska`, `Ďáska` a `Benetka` byla vizuálně potvrzena; fyzická lakuna zůstala.
10. `022-a`: zachované čtyři sloupce byly řádkově potvrzeny; opravena poznámka na tištěnou podobu `Rydz-Śmigleho`, chybějící přechod zůstává.
11. `018`, `021-a`, `021-b`, `022-b`, `022-c`, `022-d`, `023-a` a `023-b` odpovídaly obrazu bez obsahové opravy.

## Následující přesný krok

Druhá řádková kontrola položek ze zdrojových obrazů `23.jpg–29.jpg`:

- `024`;
- `025` a samostatný scénický text `025-scene-text`;
- `026`;
- `027-a`, `027-b`;
- `028`;
- `029-a`, `029-b`;
- `030`.

U `025` zachovat oddělení novinového popisku a scénického nápisu. Každou fyzicky samostatnou zprávu nebo fragment vést pod samostatným ID.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a korekční soubor seskupení.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat pouze uvedenou revizní dávkou.
5. Po dávce commitnout každý opravený soubor a aktualizovat checkpoint.
