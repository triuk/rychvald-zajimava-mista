# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený revizní checkpoint: `77a1ecb796c90a678e80b715f97e6894682c307a`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a `clanky-z-ceskeho-slova-grouping-corrections.yml`.

## Neměnná rozhodnutí

- Originály nepřejmenovávat, nepřesouvat ani neupravovat.
- Chybějící nebo nečitelné části textu nedoplňovat odhadem.
- Samostatné články a fragmenty ukládat pod vlastními stabilními ID.
- Stav `visually_verified` přidělit jen po úplném porovnání s obrazem.
- U úplně ověřeného zachovaného textu s fyzickou mezerou používat `visually_verified_with_lacuna` a ponechat příslušnou nejistotu otevřenou.
- Scénický text, který je jen částečně čitelný a doplněný dobovým popiskem, označit `visually_verified_with_caption_support`.
- Každou dávku commitnout a aktualizovat stav i registr nejistot.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Technický audit a inventář | probíhá po kolekcích |
| Klasifikace větrných mlýnů | dokončena |
| První OCR Českého slova | dokončeno pro všech 37 obrazů |
| Druhá vizuální kontrola Českého slova | probíhá; zkontrolováno 48 textových jednotek |
| Řešení nejistot | centrálně evidováno |
| Ostatní tři pilotní kolekce | čekají |
| Pull request | čeká |

## Registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

- `open`: 15
- `in_progress`: 1
- `deferred`: 2
- `resolved`: 4
- `not_actionable`: 1
- celkem: 23

Nadále otevřené textové problémy:

- `URB-U-0020`: fyzicky zničený úsek v `19.jpg`.
- `URB-U-0021`: chybějící sloupcový přechod v `21.jpg`.
- `URB-U-0022`: poškozený blok v `33.jpg`, který bude znovu posouzen v poslední dávce.
- `URB-U-0023`: neidentifikované zakončení cizího článku `019-b`.

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – klasifikace všech 31 obrazů a první OCR dokončeny.
2. `Články z Českého slova` – první OCR dokončeno, druhá kontrola probíhá.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Články z Českého slova

- 37 obrazových položek bylo ověřeno, seskupeno a přepsáno v prvním průchodu.
- Druhou kontrolou prošlo 48 jednotek od `001` po `030`, včetně oddělených fragmentů a scénického textu `025`.
- `020` a `022-a` mají stav `visually_verified_with_lacuna`.
- `025-scene-text` má stav `visually_verified_with_caption_support`: na tabuli je přímo rozpoznatelné zejména `Rychvald`, celé znění `Městys Rychvald` potvrzuje dobový popisek.
- Ostatní dokončené jednotky mají stav `visually_verified`.

### Výsledek dávky `024–030`

- `024`: potvrzeny podoby `Malhomm`, `Malhomme`, `Szustik`, `Rziman` a `Kotas` přesně podle tisku.
- `025`: celý fotografický popisek odpovídá obrazu; dokumentový a scénický text zůstávají oddělené.
- `026`: potvrzeno jméno faráře `Syrčin`; zachováno neobvyklé tištěné spojení `opustili čs. území`.
- `027-a` a `027-b`: potvrzen skutečný tok překrývající se sazby horního a dolního článku.
- `028`: zachováno tištěné vypuštění předložky před spojením `obsazeného území Těšínska`.
- `029-a`, `029-b` a `030`: text odpovídal obrazům bez obsahové opravy.
- V této dávce nevznikla nová materiální nejistota.

## Následující přesný krok

Dokončit druhou řádkovou kontrolu posledních položek:

- `031`;
- společný článek `032-033`;
- `034`;
- `035` s otevřenou lakunou `URB-U-0022`;
- `036`;
- `037-a`, `037-b`, `037-c`.

Zdrojové obrazy: `30.jpg`, `31 a.jpg`, `31 b.jpg`, `32.jpg`, `33.jpg`, `34.jpg`, `35.jpg`.

Po dokončení této dávky uzavřít `URB-U-0018`, označit druhou vizuální kontrolu kolekce jako dokončenou a teprve poté přejít k další pilotní kolekci.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a korekční soubor seskupení.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat pouze uvedenou poslední revizní dávkou.
5. Po dávce aktualizovat všechny autoritativní soubory.
