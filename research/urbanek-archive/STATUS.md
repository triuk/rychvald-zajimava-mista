# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdroj: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a plán příslušné kolekce.

## Etapy

| Kolekce / etapa | Stav |
|---|---|
| Rychvaldské větrné mlýny | klasifikace a první OCR dokončeny |
| Články z Českého slova | první OCR i druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | **první textový průchod dokončen, druhá kontrola čeká** |
| fotodokument/den po dešti | čeká |
| Nálet na Ostravu 1944 | čeká |
| Pull request | čeká |

## Ochotníci rychvald

- Inventář: 63 položek — 60 JPEG, 1 DOC a 2 technické cache.
- Ve větvi je 62 položek; chybí pouze `Thumbs.db`.
- Všech 63 položek bylo klasifikováno nebo technicky auditováno.
- Plán: `research/urbanek-archive/collections/ochotnici-rychvald-processing-plan.yml`.

## Dokončený první textový průchod

Zpracovány byly všechny plánované textové zdroje:

- nativní DOC `061`;
- krátké programy, soutěžní program, čestné uznání a úřední dopis;
- kroměřížské články a tiskové recenze;
- dvoustránkový článek Bořivoje Pešky z časopisu Těšínsko;
- knižní strany 40–45;
- rukopisná kronika, strany 260–262;
- rukopisný přehled činnosti Miroslava Neboráka;
- scénický text fotografie divadelního kroužku z roku 1923;
- selektivní text dvou výstavních panelů.

### Knižní strany 40–45

Autoritativní výstupy:

- `urbanek-ochotnici-017-a-document-text.md` — založení Sokola;
- `urbanek-ochotnici-015-017-bohdan-horak-document-text.md` — Bohdan Horák, celý článek;
- `urbanek-ochotnici-015-b-document-text.md` — sčítání lidu 1910;
- `urbanek-ochotnici-015-c-document-text.md` — neúplný začátek Hospodářského přehledu.

Duplicitní Horákův přepis byl odstraněn. V autoritativním souboru byl podle obrazu opraven tvar `zaplašil`.

### Rukopisná kronika 260–262

Výstup:

`research/urbanek-archive/ocr/urbanek-ochotnici-006-007-008-document-text.md`

Nejasná slova a příjmení jsou označena hranatými závorkami a vedena pod `URB-U-0030`.

### Přehled Miroslava Neboráka

Kvůli velikosti je jeden pramen rozdělen do dvou navazujících souborů:

- `urbanek-ochotnici-003-a-document-text.md` — hlavní seznam 32 her a souhrn režisérů;
- `urbanek-ochotnici-003-b-document-text.md` — šest doplňkových her a celkový součet.

List uvádí celkem **38 her a 110 představení**. Nejasná rukopisná čtení a rozpor datace jsou vedeny jako `URB-U-0031`.

### Text ve scéně

- `urbanek-ochotnici-018-scene-text.md` — tabulka `DIV. KROUŽEK / I. odb. / S. M. O. L. / v Rychvaldě`, datace `1923` a ateliérová značka;
- `urbanek-ochotnici-002-021-scene-text.md` — časové členění výstavy a unikátní plakát II. festivalu divadelních ochotníků.

Osoby nebyly identifikovány podle tváří.

## Registr nejistot

- `open`: 22
- `deferred`: 3
- `resolved`: 5
- `not_actionable`: 1
- celkem: 31

Otevřené položky Ochotníků: `URB-U-0024` až `URB-U-0031` podle registru.

## Následující krok

Zahájit druhou řádkovou kontrolu krátkých strukturovaných dokumentů:

1. `032–033` — program Večera tříkrálového;
2. `013` — program celostátní soutěže;
3. `023` — čestné uznání;
4. `039` — Poslední noc v roce;
5. `042` — Slavnost lampiónů;
6. `047` — dopis o věcné ceně.

Stav `visually_verified` se přidá pouze po úplném porovnání se zdrojovým obrazem.
