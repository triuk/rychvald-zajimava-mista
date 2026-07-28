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

Dokončeno je třicet sedm dávek po pěti snímcích, tedy `urbanek-ccs-001` až `185`.

- zpracováno: **185 z 201 položek**;
- proti Git blob SHA ověřeno: **185 položek**;
- vizuálně klasifikováno: **185 položek**;
- zdrojově indexováno: **185 položek**;
- zbývá: **16 položek**.

### Zjištění dávky 37

Dávka 37 zpracovala celou podsložku `9 V r. 1969 se konala v evangelickém chrámu na Ostravici ekumenick`.

- `urbanek-ccs-181` zachycuje muže v duchovním oděvu a světlé štole před oltářem; drží knihu nebo desky a gestikuluje.
- `urbanek-ccs-182` a `185` zachycují téhož nebo velmi pravděpodobně téhož muže s brýlemi při čtení z otevřené knihy před stejným oltářem. Jde o odlišné záběry, nikoli binární duplicity.
- `urbanek-ccs-183` zachycuje postavu zády k oltáři a další sedící osoby. Na oltářní textilii je čitelný odkaz `1 Petr 4,11`; úplný text je zčásti zakryt a nebyl rekonstruován.
- `urbanek-ccs-184` zachycuje muže v duchovním oděvu u vyvýšené dřevěné kazatelny nebo pultu s otevřenou knihou či listy.
- Všech pět snímků pochází ze stejného nebo velmi podobného interiéru a tvoří jednu bohoslužebnou sekvenci, nikoli pět nezávislých potvrzení archivního popisu.
- Archivní označení roku 1969, evangelického chrámu na Ostravici a ekumenického charakteru nebylo obrazem nezávisle potvrzeno.
- Všech pět souborů má odlišné Git blob SHA a žádný nemá použitelné embedded datum.
- Dávka přidala nové ID `URB-U-0072`.
- Všech pět JPEGů v deváté podsložce je nyní vizuálně klasifikováno a proti Git blob SHA ověřeno.

Pracovní soubory dávky 37:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-37.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-37.yml`;
- `sources/index.d/urbanek-ccs-37.yml`;
- nový záznam `research/urbanek-archive/uncertainties/open-19.yml`;
- aktualizovaný `research/urbanek-archive/uncertainties/index.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 38;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 72.

`URB-U-0072` sleduje nezávislé ověření roku 1969, přesného evangelického chrámu na Ostravici, ekumenického charakteru, programu, zúčastněných církví, identit duchovních, textu oltářní textilie a vztahu k dřívějším ostravickým sériím.

Archivní názvy jsou atribuce, nikoli nezávislé potvrzení. Duchovní oděv, štóla, oltář, kazatelna, gesto, biblický text ani opakovaný výskyt osoby samy neurčují identitu, úřad, denominaci, místo, datum nebo ekumenický charakter.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 185 zpracovaných a 16 zbývajících položek;
- registr používá součty 38/31/3/72;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-186` až `urbanek-ccs-190`.
- Očekávané názvy v podsložce `10 Kalendář 2015`: `1.jpg`, `2.jpg`, `3.jpg`, `4.jpg` a `5.jpg`.
- `Thumbs.db` v téže podsložce musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
