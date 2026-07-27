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

Dokončeno je dvacet šest dávek po pěti snímcích, tedy `urbanek-ccs-001` až `130`.

- zpracováno: **130 z 201 položek**;
- proti Git blob SHA ověřeno: **130 položek**;
- vizuálně klasifikováno: **130 položek**;
- zdrojově indexováno: **130 položek**;
- zbývá: **71 položek**.

### Zjištění dávky 26

Dávka 26 pokračuje v podsložce `5 Kaple CČS na Ostravici`.

- `urbanek-ccs-126` zachycuje v interiéru kaple několik duchovních, ústředního muže s řetězem nebo insignií a listem papíru, dalšího duchovního u pultu a část shromáždění.
- `urbanek-ccs-127` zachycuje velmi početný dav před kaplí; viditelné jsou děti, šátky, deštníky a okraje praporů nebo jejich žerdí.
- `urbanek-ccs-128` zachycuje otevřený vstup kaple, oltář s kalichem, svícny a květinami a početnou skupinu duchovních. Archivní název zní `Vlevo Leonard Bugumský`, ale v levé části je několik mužů, takže přesný referent není jednoznačný.
- `urbanek-ccs-129` zachycuje dva duchovní s řetězy nebo insigniemi proti sobě; jeden drží světlý dokument nebo několik listů. Přesný úkon a obsah dokumentu nejsou určeny.
- `urbanek-ccs-130` zachycuje stojícího duchovního při projevu a sedícího duchovního s otevřenou složkou nebo knihou.
- Opakované prostředí, oděvy a insignie podporují souvislost se širší slavnostní sekvencí, nikoli přesné datum nebo identitu osob.
- Dávka nepřidala nové ID. Rozšířila `URB-U-0068` a `URB-U-0070`.

Pracovní soubory dávky 26:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-26.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-26.yml`;
- `sources/index.d/urbanek-ccs-26.yml`;
- rozšířené `research/urbanek-archive/uncertainties/open-16.yml` a `open-17.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

`URB-U-0068` nyní zahrnuje také variantu jména `Bugumský` a nejednoznačný směrový popisek na položce 128. `URB-U-0070` byla rozšířena o velké shromáždění, projevy duchovních a scénu s listinou nebo dokumentem.

Směrový archivní popisek jako `vlevo` potvrzuje své znění, ale osoba se podle něj při více možných referentích nepřiřazuje bez další anotace.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 130 zpracovaných a 71 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-131` až `urbanek-ccs-135`.
- Očekávané názvy: `20.jpg`, `21.jpg`, `22.jpg`, `23.jpg` a `24.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
