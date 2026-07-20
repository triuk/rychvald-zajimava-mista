# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený obsahový checkpoint: `651fa3975169eec06acbdae6f5f483866bb31c43`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt: potvrzeno uživatelem.

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml` a `uncertainties.yml`.

## Neměnná rozhodnutí

- Originální soubory nepřejmenovávat, nepřesouvat ani neupravovat.
- Zachovat původní strukturu a názvy.
- `Thumbs.db` a `ZbThumbnail.info` ponechat pro budoucí analýzu.
- Dokumentový a scénický text evidovat odděleně.
- OCR má stav `machine_unverified`, dokud neproběhne druhá řádková kontrola.
- Chybějící, poškozený nebo nespojitý text nedoplňovat odhadem.
- Fyzicky samostatné články a fragmenty ukládat pod vlastními stabilními ID.
- Každou dokončenou dávku commitnout a aktualizovat stav i registr nejistot.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Pravidla a workflow | dokončeno |
| Technický audit | probíhá po kolekcích |
| Inventář | probíhá |
| Klasifikace pilotu | probíhá |
| OCR | probíhá |
| Druhá vizuální kontrola OCR | čeká po první sérii |
| Řešení nejistot | centrálně evidováno |
| Pull request | čeká |

## Centrální registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

Aktuální souhrn:

- `open`: 17
- `deferred`: 2
- `resolved`: 1
- `not_actionable`: 1
- celkem: 21

Novější položky:

- `URB-U-0019` – fyzicky poškozená věta v článku `015`;
- `URB-U-0020` – poškozený úsek, který může obsahovat celou chybějící krátkou zprávu v `020`;
- `URB-U-0021` – nespojitý přechod sloupců v článku `022-a`.

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – klasifikace všech 31 obrazů a první OCR dokončeny.
2. `Články z Českého slova` – inventář, audit cache, ověření cest a seskupení všech 37 obrazů dokončeny; OCR probíhá.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Rychvaldské větrné mlýny

- 31 obrazových souborů ověřeno a klasifikováno.
- Dva dokumentové přepisy a jeden scénický nápis dokončeny.
- Pět `Thumbs.db` chybí v GitHubu, ale zůstává na Drivu a bylo analyzováno.
- Kořenová cache obsahuje stopu po chybějícím `P1010269.JPG`.
- Podrobnosti: `research/urbanek-archive/reports/rychvaldske-vetrne-mlyny-thumbnail-cache.md`.

## Články z Českého slova

- Na Drivu: 37 obrazů a dvě technické cache.
- V GitHubu: všech 37 obrazů a `ZbThumbnail.info`; chybí `Thumbs.db`.
- Cache obsahuje osm unikátních náhledů bez současného plného souboru.
- Všech 37 obrazů je seskupeno ve čtyřech souborech `clanky-z-ceskeho-slova-grouping-01.yml` až `04.yml`.
- Číselné názvy souborů nejsou spolehlivá chronologie.

### Dokončené OCR

Dokončeny jsou:

- `001–015`;
- `016-a`, `016-b`;
- `017-a`, `017-b`, `017-c`, `017-d`;
- `018`, `019`, `020`;
- `021-a`, `021-b`;
- `022-a`, `022-b`, `022-c`, `022-d`;
- `023-a`, `023-b`.

Všechny soubory jsou v `research/urbanek-archive/ocr/`.

### Poslední zpracovaná dávka

- `018`: **„Péče o uprchlíky z obsazeného území“**.
- `019`: **„Vojenský dozor na šachtách na Těšínsku“**.
- `020`: **„Zprávy z Těšínska“**, s vyznačeným poškozeným úsekem.
- `021-a`: **„Situační zpráva z pohraničí“**.
- `021-b`: **„Rekvisice radiových aparátů neprospěla“**.
- `022-a`: **„Polský zábor českých obcí dokončen“**, se dvěma výslovně označenými lakunami.
- `022-b`: **„Zásobování Ostravy potravinami zajištěno“**.
- `022-c`: neúplný článek **„Mléčný vlak do Mor. Ostravy“**.
- `022-d`: pouze nadpis **„Dvě ultimata Arabů“**.
- `023-a`: **„Na Těšínsku propouštěni dělníci i úředníci“**.
- `023-b`: **„Svinovské nádraží neutrální“**.

### Oprava mapování 20. července 2026

- `011` odpovídá `10.jpg`;
- `012` odpovídá `11.jpg`;
- `013` odpovídá `12.jpg`.

Pod žádným ID již nezůstává nesprávně přiřazený obsah.

## Následující přesný krok

Přepsat `urbanek-ceske-slovo-024`, zdroj `Články z Českého slova/23.jpg`, jako soubor krátkých zpráv **„Zprávy z Těšínska“**. Zachovat oddělení jednotlivých zpráv a dobový pravopis.

Poté pokračovat `urbanek-ceske-slovo-025`, který obsahuje dvě novinové fotografie, jejich popisek a scénický nápis **„Městys Rychvald“**.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, tento soubor, `state.yml` a `uncertainties.yml`.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat pouze výše uvedeným krokem.
5. Po malé dávce commitnout výstupy a aktualizovat všechny stavové soubory.
