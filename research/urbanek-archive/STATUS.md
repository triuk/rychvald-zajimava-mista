# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený obsahový checkpoint: `47b931aeb6ea1a9217ab70cbb62d78deb82f1637`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt: potvrzeno uživatelem.

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml` a `uncertainties.yml`.

## Neměnná rozhodnutí

- Originální soubory nepřejmenovávat, nepřesouvat ani neupravovat.
- Zachovat původní strukturu a názvy.
- `Thumbs.db` a `ZbThumbnail.info` ponechat pro budoucí analýzu.
- Dokumentový a scénický text evidovat odděleně.
- Chybějící, poškozený nebo nespojitý text nedoplňovat odhadem.
- Fyzicky samostatné články a fragmenty ukládat pod vlastními stabilními ID.
- První OCR přepis má stav `machine_unverified`; po řádkové kontrole proti obrazu lze změnit na `visually_verified`.
- Každou dokončenou dávku commitnout a aktualizovat stav i registr nejistot.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Pravidla a workflow | dokončeno |
| Technický audit | probíhá po kolekcích |
| Inventář | probíhá |
| Klasifikace pilotu | probíhá |
| První OCR Českého slova | dokončeno |
| Druhá vizuální kontrola OCR | následuje |
| Řešení nejistot | centrálně evidováno |
| Pull request | čeká |

## Centrální registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

Aktuální souhrn:

- `open`: 18
- `deferred`: 2
- `resolved`: 1
- `not_actionable`: 1
- celkem: 22

Nejistoty související s poškozením textu:

- `URB-U-0019` – věta v článku `015`;
- `URB-U-0020` – možná chybějící celá krátká zpráva v `020`;
- `URB-U-0021` – nespojitý sloupcový přechod v `022-a`;
- `URB-U-0022` – poškozený blok v `035`, který může skrývat více krátkých zpráv.

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – klasifikace všech 31 obrazů a první OCR dokončeny.
2. `Články z Českého slova` – inventář, audit, seskupení a první OCR všech 37 obrazů dokončeny; čeká druhá řádková kontrola.
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
- Všech 37 obrazových položek má dokončený první OCR průchod.
- Výstupy jsou v `research/urbanek-archive/ocr/`.
- Složené výstřižky jsou rozděleny na samostatné textové jednotky.
- `31 a.jpg` a `31 b.jpg` jsou přepsány společně v `urbanek-ceske-slovo-032-033-document-text.md`.
- `24.jpg` má oddělený dokumentový popisek a scénický OCR záznam **„Městys Rychvald“**.

### Poslední dokončené položky

- `028`: **„Jednání o Češích na Těšínsku“**.
- `029-a`: **„Zprávy z Těšínska“**.
- `029-b`: **„Hledá se nezvěstný“** – Miloslav Baron.
- `030`: **„Zprávy z Těšínska“**.
- `031`: **„V Polsku střelba do Ukrajinců“**.
- `032–033`: **„Milé klopoty“**.
- `034`: **„Které sňatky na Těšínsku musí býti znovu provedeny“**.
- `035`: poškozené **„Zprávy z Těšínska“**.
- `036`: **„Protest uprchlíků z Petřvaldu“**.
- `037-a`: hlavička vydání **31. října 1938**.
- `037-b`: **„Beck pro spolupráci s Československem“**.
- `037-c`: neúplný článek **„Úmluvy gentlemanů“**.

### Oprava mapování 20. července 2026

- `011` odpovídá `10.jpg`;
- `012` odpovídá `11.jpg`;
- `013` odpovídá `12.jpg`.

Pod žádným ID nezůstává nesprávně přiřazený obsah.

## Následující přesný krok

Zahájit druhou řádkovou kontrolu proti zdrojovým obrazům pro první dávku:

- `001`;
- `002`;
- `003`;
- `004-a`, `004-b`, `004-c`;
- `005`.

Každý přepis opravit pouze tam, kde rozdíl prokazuje obraz. Po úplné kontrole změnit stav daného souboru z `machine_unverified` na `visually_verified`. Nevyřešené znaky nebo jména zapsat do `uncertainties.yml` a průběh evidovat pod `URB-U-0018`.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, tento soubor, `state.yml` a `uncertainties.yml`.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat pouze výše uvedeným krokem.
5. Po malé dávce commitnout výstupy a aktualizovat všechny stavové soubory.
