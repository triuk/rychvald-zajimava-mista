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
- stav: `processing_in_progress`.

Dokončeno je třicet tři dávek po pěti snímcích, tedy `urbanek-ccs-001` až `165`.

- zpracováno: **165 z 201 položek**;
- proti Git blob SHA ověřeno: **165 položek**;
- vizuálně klasifikováno: **165 položek**;
- zdrojově indexováno: **165 položek**;
- zbývá: **36 položek**.

### Zjištění dávky 33

Dávka 33 pokračuje v podsložce `7 Pohřeb biskupa br. Ferdinanda Stibora v říjnu 1956`.

- `urbanek-ccs-161` až `163` zachycují navazující záběry vstupu a schodiště. Osoby v dlouhých tmavých oděvech sestupují z budovy nebo stojí po stranách schodiště.
- Na `161` jsou světlé znaky připomínající kalich nebo medailon a u pravého okraje žena se světlou páskou na paži a tmavým křížovitým znakem. Význam znaků ani pásky není určen.
- `162` zachycuje dva muže s výraznými řetězy a oválnými medailony; fotografie sama neurčuje jejich jména ani úřady.
- `163` je široký pohled na zaplněné schodiště s převážně volným středním průchodem. Formální účel uspořádání zůstává neověřen.
- `164` a `165` zachycují navazující venkovní pohyb mezi shromážděním. Na `164` drží jeden muž světlou knihu, desky nebo složku; na `165` mají dva muži velké světlé znaky připomínající kalich.
- Všech pět souborů má odlišné Git blob SHA a žádný není binárním duplikátem. Jde však o obrazově navazující sekvenci, nikoli pět nezávislých důkazů archivního popisu.
- Žádný soubor nemá použitelné embedded datum.
- Dávka nepřidala nové ID a rozšířila `URB-U-0071`.

Pracovní soubory dávky 33:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-33.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-33.yml`;
- `sources/index.d/urbanek-ccs-33.yml`;
- aktualizované `research/urbanek-archive/uncertainties/open-18.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 37;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 71.

`URB-U-0071` nyní zahrnuje položky `156` až `165`: portrét, vystavení rakve, osoby u rakve, výstup ze sboru, schodiště, řetězy, medailony, znaky připomínající kalich, pásku s křížovitým znakem, prapory a navazující venkovní pohyb.

Archivní názvy jsou atribuce, nikoli nezávislé potvrzení. Oděv, řetěz, medailon, znak, pokrývka hlavy, páska na paži ani postavení v průvodu samy neurčují identitu, úřad, organizaci nebo formální roli.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 165 zpracovaných a 36 zbývajících položek;
- registr používá součty 37/31/3/71;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-166` až `urbanek-ccs-170`.
- Očekávané názvy v téže podsložce: `11.jpg`, `12.jpg`, `13.jpg`, `14.jpg` a `15.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
