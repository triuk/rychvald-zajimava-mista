# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený obsahový checkpoint: `3e5555e8d636cde56ce2963ee72c1ab2edd7fa31`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt: potvrzeno uživatelem.

Autoritativní předání mezi chaty tvoří:

- `AGENTS.md`
- tento `STATUS.md`
- `research/urbanek-archive/state.yml`
- `research/urbanek-archive/uncertainties.yml`

## Neměnná rozhodnutí

- Originální soubory nepřejmenovávat, nepřesouvat ani neupravovat.
- Zachovat původní strukturu a názvy.
- `Thumbs.db` a `ZbThumbnail.info` ponechat pro budoucí analýzu.
- Dokumentový a scénický text evidovat odděleně.
- OCR má stav `machine_unverified`, dokud neproběhne druhá řádková kontrola.
- Chybějící nebo poškozený text nedoplňovat odhadem.
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

- `open`: 15
- `deferred`: 2
- `resolved`: 1
- `not_actionable`: 1
- celkem: 19

Položka `URB-U-0019` eviduje fyzicky poškozený úsek v článku `urbanek-ceske-slovo-015` mezi slovy `ostatní závody` a `vnucení správci`.

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

Dokončeny jsou položky:

- `001–003`;
- `004-a`, `004-b`, `004-c`;
- `005–015`;
- `016-a`, `016-b`;
- `017-a`, `017-b`, `017-c`, `017-d`.

Soubory jsou v `research/urbanek-archive/ocr/`.

### Oprava mapování 20. července 2026

- `011` správně odpovídá `10.jpg` a článku **„Zůstanou na Těšínsku české školy?“**;
- `012` správně odpovídá `11.jpg` a článku **„Fryštát už má polského starostu“**;
- `013` správně odpovídá `12.jpg` a článku **„První část fryštátského okresu obsazena“**.

Chybný obsah byl nahrazen a pod žádným ID již nezůstává nesprávné přiřazení.

### Poslední nové přepisy

- `014`: **„Fryštát s okolím zabrán“**.
- `015`: **„Poslední den polského záboru na Těšínsku“**.
- `016-a`: **„Sta lidí vypovídáno z Těšínska“**.
- `016-b`: **„Konsulární ataše v Ostravě“**.
- `017-a`: **„Přeplněné přívozské nádraží“**.
- `017-b`: neúplný začátek **„Poslanec Sliwka v Katovicích“**.
- `017-c`: částečný reklamní text **„Různé nečistoty pleti“**.
- `017-d`: pouze nadpis **„Sebevražda 24letého“**.

## Následující přesný krok

Přepsat `urbanek-ceske-slovo-018`, zdroj `Články z Českého slova/17.jpg`, článek **„Péče o uprchlíky z obsazeného území“** s podnadpisem **„Kde se mají uprchlíci hlásit v Mor. Ostravě“**.

Poté pokračovat položkou `urbanek-ceske-slovo-019`. Každou novou materiální nejistotu zapsat do `uncertainties.yml`.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, tento soubor, `state.yml` a `uncertainties.yml`.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat pouze výše uvedeným krokem.
5. Po malé dávce commitnout výstupy a aktualizovat všechny stavové soubory.
