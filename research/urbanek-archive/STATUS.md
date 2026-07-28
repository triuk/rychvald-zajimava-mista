# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový kořen: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt bylo potvrzeno.
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Autoritativním pracovním úložištěm je Git repozitář.

## Draft pull request

- PR: [#1 – Import and classify Jaromír Urbánek archive (pilot + CČS batch)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

## Dokončený pilot

| Kolekce | Obsahové soubory | Technické soubory | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | dokončeno |
| Články z Českého slova | 37 | 2 | 39 | dokončeno |
| Ochotníci rychvald | 61 | 2 | 63 | dokončeno |
| fotodokument/den po dešti | 8 | 2 | 10 | dokončeno |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | dokončeno |
| **Celkem** | **144** | **15** | **159** | **159 z 159 položek přítomno** |

Audity pilotních cache prokázaly **11 chybějících plných originálů** dochovaných pouze jako náhledy.

## Kolekce historie Církve československé

Kolekce: `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`

- 10 tematických podsložek;
- 200 JPEGů;
- 1 technický soubor `Thumbs.db`;
- celkem 201 položek;
- stav: `completed`.

Dokončeno je čtyřicet obrazových dávek `urbanek-ccs-001` až `200` a samostatný audit technického souboru.

- zpracováno: **201 z 201 položek**;
- proti Git blob SHA ověřeno: **201 položek**;
- vizuálně klasifikováno: **200 obrazových položek**;
- zdrojově indexováno: **201 položek**;
- zbývá: **0 položek**.

### Zjištění auditu `Thumbs.db`

- `10 Kalendář 2015/Thumbs.db` má 70 656 B; Drive originál a Git soubor jsou binárně totožné.
- SHA-256: `056cb436b5556dea975512e8ff00cd80ffb8eaa7ecbf7c3c4795e8f47831d037`; Git blob SHA: `91d73b30448ce8f8aa02a8ed79dafee5d349f0c2`.
- Katalog obsahuje přesně názvy `1.jpg` až `15.jpg` a jednu interní GUID položku se složeným náhledem složky Windows.
- Čtrnáct plných náhledů bylo dekódováno a jednoznačně přiřazeno k odpovídajícím kalendářovým stranám `1.jpg` až `14.jpg`.
- Stream náhledu `15.jpg` je neúplný: CFB struktura odkazuje na sektory za koncem dochovaného souboru. Plný soubor `15.jpg` je však v kolekci přítomen a samostatně Git-ověřen.
- Cache neobsahuje žádný další název zdrojového obrázku a nedokládá žádný chybějící plný originál.
- Počet chybějících plných originálů doložených pouze touto cache: **0**.
- Katalogové časy jsou metadata cache z 24. ledna 2015, nikoli data historických událostí.

Pracovní soubory auditu:

- `research/urbanek-archive/reports/historie-cirkve-ceskoslovenske-thumbs-audit.md`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-technical-inventory.csv`;
- `sources/index.d/urbanek-ccs-technical.yml`;
- aktualizované `research/urbanek-archive/uncertainties/open-20.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 39;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 73.

`URB-U-0073` bylo rozšířeno o výsledek technického auditu. Cache potvrzuje úplnost názvů patnácti kalendářových stran, ale nemění otevřené otázky autorství, vydavatele, bibliografie, původu vložených fotografií, historické správnosti popisků a práv.

Strukturální neúplnost cache sama není dokladem chybějícího originálu. Za takový doklad lze považovat pouze název nebo náhled, který nelze přiřadit k přítomnému plnému souboru.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- kolekce je zpracována v rozsahu 201 z 201 položek;
- registr používá součty 39/31/3/73;
- pilotní údaj o 11 chybějících plných originálech zůstává beze změny a netýká se této kolekce;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Kolekce historie CČS: `completed`.
- Zbývající archivní položky v této kolekci: `0`.
- Následuje uživatelská kontrola dokončené kolekce a rozhodnutí o prioritách 39 otevřených nejistot.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
