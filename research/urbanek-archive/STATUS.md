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

Dokončeno je třicet šest dávek po pěti snímcích, tedy `urbanek-ccs-001` až `180`.

- zpracováno: **180 z 201 položek**;
- proti Git blob SHA ověřeno: **180 položek**;
- vizuálně klasifikováno: **180 položek**;
- zdrojově indexováno: **180 položek**;
- zbývá: **21 položek**.

### Zjištění dávky 36

Dávka 36 zpracovala celou podsložku `8 Farář Leonard Bogumský v Doubravě u příležitosti neznámých oslav`.

- `urbanek-ccs-176` zachycuje čtyři muže v dlouhých tmavých oděvech u oltáře pod krucifixem; na oltáři jsou kalich, otevřená kniha a široká nádoba.
- `urbanek-ccs-177` zachycuje muže se vzpaženýma rukama u stejného oltáře; na krucifixu je čitelné označení `INRI`.
- `urbanek-ccs-178` zachycuje zaplněný interiér s galerií, velkou textilní korouhví nebo praporem, dvěma duchovními v uličce a několika křesťanskými symboly.
- `urbanek-ccs-179` zachycuje duchovního u pultu s textilií se znakem kalicha a jen částečně čitelným víceřádkovým textem.
- `urbanek-ccs-180` zachycuje obřadní úkon mezi dvěma muži u oltáře; přesný úkon ani identity osob nelze určit pouze z fotografie.
- Všech pět snímků pochází ze stejného nebo velmi podobného interiéru a zachycuje opakující se osoby. Jde o jednu obrazovou sekvenci, nikoli pět nezávislých potvrzení archivního popisu.
- Všech pět souborů má odlišné Git blob SHA a žádný nemá použitelné embedded datum.
- Dávka nepřidala nové ID; rozšířila `URB-U-0068` o položky `176` až `180`.
- Všech pět JPEGů v osmé podsložce je nyní vizuálně klasifikováno a proti Git blob SHA ověřeno.

Pracovní soubory dávky 36:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-36.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-36.yml`;
- `sources/index.d/urbanek-ccs-36.yml`;
- aktualizované `research/urbanek-archive/uncertainties/open-16.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 37;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 71.

`URB-U-0068` nyní vedle portrétu, skupinových návštěv a ostravické slavnosti zahrnuje také položky `176` až `180`. Neověřené zůstávají správná podoba jména, identita Leonarda Bogumského na jednotlivých snímcích, Doubrava jako místo, datum a účel bohoslužby nebo slavnosti, ostatní osoby, význam symbolů, text na závěsné textilii a přesný liturgický úkon.

Archivní názvy jsou atribuce, nikoli nezávislé potvrzení. Duchovní oděv, štóla, kalich, prapor, symbol, gesto, pozice u oltáře ani podávání předmětu samy neurčují osobu, úřad, organizaci, místo nebo přesný obřad.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 180 zpracovaných a 21 zbývajících položek;
- registr používá součty 37/31/3/71;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-181` až `urbanek-ccs-185`.
- Očekávané názvy v podsložce `9 V r. 1969 se konala v evangelickém chrámu na Ostravici ekumenick`: `1.jpg`, `2.jpg`, `3.jpg`, `4.jpg` a `5.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
