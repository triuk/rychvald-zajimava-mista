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

Dokončeno je třináct dávek po pěti snímcích, tedy `urbanek-ccs-001` až `065`.

Dosavadní stav nové kolekce:

- zpracováno: **65 z 201 položek**;
- proti Git blob SHA ověřeno: **65 položek**;
- vizuálně klasifikováno: **65 položek**;
- zdrojově indexováno: **65 položek**;
- zbývá: **136 položek**.

### Zjištění dávky 13

Dávka 13 uzavírá první podsložku třemi portréty duchovních a otevírá druhou podsložku dvěma skupinovými snímky návštěvy.

- `urbanek-ccs-061` zachycuje muže v duchovním oděvu s výrazným řetězem nebo insignií u stolu s kalichem, knihami a listinami. Jméno a titul biskupa Gabriela Chrobáčka pocházejí z archivního názvu; snímek rozšiřuje `URB-U-0062`.
- `urbanek-ccs-062` zachycuje duchovního ve světlé štóle čtoucího z knihy za liturgickým stolem se znakem kalicha a kříže. Archiv jej označuje jako faráře Leonarda Bogumského; používá přitom varianty `Bogumski` a `Bogumský`.
- `urbanek-ccs-063` zachycuje ženu v duchovním oděvu, bílé štóle s červeným kalichem a řetězem nebo insignií. Jméno Jana Šilerová, titul Mgr. a funkce biskupky pocházejí z archivního názvu; fotografie rozšiřuje `URB-U-0058`.
- `urbanek-ccs-064` zachycuje širší skupinu, v jejíž přední řadě sedí dvě ženy a dva muži. Název je označuje jako faráře Vodičku a Bogumského s manželkami, ale jednotlivé osoby nelze přiřadit pouze podle vzhledu.
- `urbanek-ccs-065` zachycuje stejnou čtveřici samostatně v zahradě před plotem. Jde o samostatný záběr, nikoli prostý výřez. Lokalizace k faráři Bogumskému a rok 1965 nebo 1970 nejsou obrazem potvrzeny.

Pracovní soubory dávky 13:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-13.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-13.yml`;
- `sources/index.d/urbanek-ccs-13.yml`;
- `research/urbanek-archive/uncertainties/open-16.yml`;
- rozšířené `research/urbanek-archive/uncertainties/open-11.yml`, `open-12.yml` a `open-15.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 34;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 68.

Nejistoty z kolekce CČS jsou vedeny pod `URB-U-0039` až `URB-U-0068`. Dávka 13:

- rozšířila `URB-U-0058` o portrét Jany Šilerové, její služební a biskupskou funkci a význam insignie;
- rozšířila `URB-U-0062` o samostatný portrét připisovaný Gabrielu Chrobáčkovi;
- rozšířila `URB-U-0067` o skupinové snímky Karla a Libuše Vodičkových a dataci návštěvy;
- přidala `URB-U-0068` – pravopis jména, identitu, službu, manželku, zahradu a návštěvu Leonarda Bogumského.

Dřívější aktivní položky zůstávají otevřené. Archivní název je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, příbuzenského vztahu nebo funkce. Opakování stejných lidí ve více obrazech potvrzuje obrazovou souvislost, nikoli jejich jména.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 65 zpracovaných a 136 zbývajících položek;
- registr používá součty 34/31/3/68;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-066` až `urbanek-ccs-070`.
- Očekávané mapování: druhá podsložka soubory `3` až `6` a první soubor podsložky `3 Biskup Ferdinand Stibor v Rychvaldě`.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
