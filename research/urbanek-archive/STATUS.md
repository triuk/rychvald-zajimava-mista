# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový kořen: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt bylo potvrzeno.
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Autoritativním pracovním úložištěm je Git repozitář.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties/index.yml` včetně odkazovaných shard souborů, `reports/pilot-reconciliation.md` a kolekční přehledy v `collections/`.

## Draft pull request

- PR: [#1 – Import and classify Jaromír Urbánek archive (pilot + CČS batch)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

PR obsahuje dokončený pilot a rozpracovanou následující archivní dávku. Tyto dva rozsahy jsou evidovány odděleně.

## Dokončený pilot

| Kolekce | Obsahové soubory | Technické soubory | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | klasifikace a první OCR dokončeny |
| Články z Českého slova | 37 | 2 | 39 | OCR a druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | 61 | 2 | 63 | textový průchod a druhá vizuální kontrola dokončeny |
| fotodokument/den po dešti | 8 | 2 | 10 | audit a vizuální klasifikace dokončeny |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | audit a vizuální klasifikace dokončeny |
| **Celkem** | **144** | **15** | **159** | **159 z 159 položek přítomno** |

Podrobná reconciliace: `research/urbanek-archive/reports/pilot-reconciliation.md`.

Audity pilotních cache prokázaly **11 chybějících plných originálů**. Náhled v `Thumbs.db` není náhradou plného originálu; přesně ověřená kopie obrazu dochovaná pod jiným názvem se však nepovažuje za další chybějící obrazový obsah.

## Nová dávka – historie Církve československé

Kolekce: `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`

- 10 tematických podsložek;
- 200 JPEGů;
- 1 technický soubor `Thumbs.db`;
- celkem 201 položek;
- stav: `processing_in_progress`;
- pilotní součty se touto dávkou nemění.

Dokončeno je čtrnáct dávek po pěti snímcích, tedy `urbanek-ccs-001` až `070`.

Dosavadní stav nové kolekce:

- zpracováno: **70 z 201 položek**;
- proti Git blob SHA ověřeno: **70 položek**;
- vizuálně klasifikováno: **70 položek**;
- zdrojově indexováno: **70 položek**;
- zbývá: **131 položek**.

### Zjištění dávky 14

Dávka 14 uzavírá druhou podsložku výročním přivítáním a křty a otevírá sérii připisovanou Ferdinandu Stiborovi.

- `urbanek-ccs-066` a `067` jsou dvě archivní reprodukce **téhož fotografického obrazu** přivítání duchovního dítětem. Technické porovnání nalezlo 306 geometricky konzistentních shod a 96,8 % vybraných bodů odpovídá jednomu modelu výřezu a změny měřítka. Soubor `066` proto není druhým nezávislým fotografickým okamžikem.
- Název `066` končí řetězcem `Kare`; celé jméno nebylo rekonstruováno. Název `067` označuje levého duchovního jako biskupa Marcelucha, ale jméno, pravopis a úřad nejsou obrazem potvrzeny.
- `urbanek-ccs-068` zachycuje křestní obřad s jedním jasně viditelným kojencem, křestní svící, duchovním a několika rodinnými skupinami. Archivní tvrzení o trojích křtinách nelze z jediného obrazu ověřit.
- `urbanek-ccs-069` zachycuje další rodinnou skupinu s kojencem před duchovním s řetězem nebo insignií. Totožnost dítěte, rodičů, kmotrů a duchovního není známa.
- `urbanek-ccs-070` zachycuje venkovní uvítání chlebem a solí ženou v lidovém či slavnostním kroji. Ferdinand Stibor, rok 1948 a vztah k dřívější skupinové fotografii `urbanek-ccs-025` pocházejí z archivního kontextu a zůstávají otevřené.

Pracovní soubory dávky 14:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-14.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-14.yml`;
- `sources/index.d/urbanek-ccs-14.yml`;
- rozšířené `research/urbanek-archive/uncertainties/open-08.yml` a `open-13.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 34;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 68.

Dávka 14 nepřidala nové ID, ale rozšířila:

- `URB-U-0063` – padesáté výročí roku 1970, useknuté jméno `Kare…`, biskup Marceluch, hosté a program;
- `URB-U-0064` – počet křtů, rodiny, děti, duchovní a matrika;
- `URB-U-0050` – uvítání chlebem a solí, návštěva připisovaná Ferdinandu Stiborovi a vztah ke skupinové fotografii.

Dřívější aktivní položky zůstávají otevřené. Dvě reprodukce stejného fotografického obrazu jsou dvěma archivními soubory, nikoli dvěma nezávislými důkazy události. Archivní názvy ani názvy podsložek automaticky nepotvrzují osoby, data a funkce.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 70 zpracovaných a 131 zbývajících položek;
- registr používá součty 34/31/3/68;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-071` až `urbanek-ccs-075`.
- Očekávané archivní názvy v podsložce `3 Biskup Ferdinand Stibor v Rychvaldě`: `2.jpg`, `2a.jpg`, `3 Před oltářem.jpg`, `4.jpg` a `5 Společná fotografie také s dětmi.jpg`.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
