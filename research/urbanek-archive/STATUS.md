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

Dokončeno je dvacet sedm dávek po pěti snímcích, tedy `urbanek-ccs-001` až `135`.

- zpracováno: **135 z 201 položek**;
- proti Git blob SHA ověřeno: **135 položek**;
- vizuálně klasifikováno: **135 položek**;
- zdrojově indexováno: **135 položek**;
- zbývá: **66 položek**.

### Zjištění dávky 27

Dávka 27 pokračuje v podsložce `5 Kaple CČS na Ostravici`.

- `urbanek-ccs-131` zachycuje ženu ve zdobeném oděvu s velkou kyticí před duchovním s řetězem nebo insignií. Přesná krojová či organizační příslušnost ani osoby nejsou určeny.
- `urbanek-ccs-132` a `133` jsou dvě archivní reprodukce téhož podkladového záběru: muž v obleku stojí vedle duchovního, který drží zavinuté dítě a květiny.
- `urbanek-ccs-133` zachovává širší okolí; oba soubory jsou samostatné inventární položky, ale představují pouze jeden nezávislý obrazový doklad.
- `urbanek-ccs-134` zachycuje další projev nebo čtení duchovního s listem papíru.
- `urbanek-ccs-135` zachycuje zaplněný interiér s účastníky v dřevěných lavicích, některými knihami či zpěvníky a vysokou žerdí nebo standardou v zadní části.
- Žádný z pěti souborů neobsahuje použitelné embedded datum.
- Dávka nepřidala nové ID. Rozšířila `URB-U-0070`.

Pracovní soubory dávky 27:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-27.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-27.yml`;
- `sources/index.d/urbanek-ccs-27.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-17.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

`URB-U-0070` nyní zahrnuje také uvítání ženou ve zdobeném oděvu, dítě v náručí duchovního, dvě reprodukce téhož záběru, další projev a zaplněný interiér.

Dvě reprodukce téhož podkladového snímku jsou dvě archivní položky, ale pouze jeden nezávislý obrazový doklad. Přítomnost dítěte sama neurčuje křest, požehnání ani jiný přesný úkon.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 135 zpracovaných a 66 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-136` až `urbanek-ccs-140`.
- Očekávané názvy: `25.jpg`, `26.jpg`, `27.jpg`, `28.jpg` a `29.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
