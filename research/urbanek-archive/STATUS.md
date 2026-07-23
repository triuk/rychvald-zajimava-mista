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

Dokončeno je deset dávek po pěti snímcích, tedy `urbanek-ccs-001` až `050`.

Dosavadní stav nové kolekce:

- zpracováno: **50 z 201 položek**;
- proti Git blob SHA ověřeno: **50 položek**;
- vizuálně klasifikováno: **50 položek**;
- zdrojově indexováno: **50 položek**;
- zbývá: **151 položek**.

### Zjištění dávky 10

Dávka 10 dokumentuje Chrobáčkovu biskupskou událost, výročí roku 1970, křtiny a novodobou husovskou vzpomínku.

- `urbanek-ccs-046` zachycuje duchovního s řetězem při předání listiny a plastiky sedící mužské postavy. Jméno Gabriel Chrobáček a tvrzení, že se stal biskupem, pocházejí z archivního názvu; snímek rozšiřuje `URB-U-0062`.
- `urbanek-ccs-047` zachycuje v kněžišti tři duchovní a muže v obleku, kytice, insignii a kalich. Rok 1970 a padesáté výročí založení CČS v Rychvaldě jsou zatím archivními tvrzeními.
- `urbanek-ccs-048` zachycuje křestní obřad s dítětem, svící a několika duchovními. EXIF datum **1. září 2014** dokládá digitalizaci nebo reprodukci historického snímku, nikoli křtiny roku 1970. Označení faráře Vodičky podle brýlí vyžaduje dokumentární ověření.
- `urbanek-ccs-049` zachycuje hořící hranici s portrétem, početný dav a ženu v liturgickém oděvu. EXIF datum **15. března 2012** je v rozporu s plně olistěnou letní scénou a bez dalšího dokladu není spolehlivou datací události. Název je useknutý za řetězcem `far`.
- `urbanek-ccs-050` zachycuje průvod od kostela vedený dvěma ženami, za nimiž jdou hasiči a další účastníci. Vztah k fotografii hranice je pracovní hypotéza založená na tématu a pořadí, nikoli potvrzený společný ročník.

Pracovní soubory dávky 10:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-10.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-10.yml`;
- `sources/index.d/urbanek-ccs-10.yml`;
- `research/urbanek-archive/uncertainties/open-13.yml`;
- aktualizovaný `research/urbanek-archive/uncertainties/open-12.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 31;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 65.

Nejistoty z kolekce CČS jsou vedeny pod `URB-U-0039` až `URB-U-0065`. Dávka 10 přidala:

- `URB-U-0063` – přesný kontext padesátého výročí roku 1970, osoby a program;
- `URB-U-0064` – křtiny roku 1970, rodina, duchovní a identifikace faráře Vodičky;
- `URB-U-0065` – obnovení husovské hranice, průvod, datace, osoby, hasiči a useknutý popisek.

`URB-U-0062` byla rozšířena o fotografii předání plastiky při Chrobáčkově biskupské události. Dřívější aktivní položky zůstávají otevřené. Negativní dílčí hledání není důvodem k uzavření. Archivní název souboru je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, události nebo funkce. Osoby se neidentifikují pouze podle obličeje a useknuté názvy se nedoplňují odhadem.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 50 zpracovaných a 151 zbývajících položek;
- registr používá součty 31/31/3/65;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-051` až `urbanek-ccs-055`.
- Očekávané archivní názvy: soubory `52a`, `52b`, `53`, `54` a `55`; přesné mapování se ověří proti větvi před zápisem.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
