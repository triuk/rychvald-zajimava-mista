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

Dokončeno je osm dávek po pěti snímcích, tedy `urbanek-ccs-001` až `040`.

Dosavadní stav nové kolekce:

- zpracováno: **40 z 201 položek**;
- proti Git blob SHA ověřeno: **40 položek**;
- vizuálně klasifikováno: **40 položek**;
- zdrojově indexováno: **40 položek**;
- zbývá: **161 položek**.

### Zjištění dávek 07 a 08

Dávka 07 dokumentuje zaplněný interiér a početné skupiny prvního přijímání. Tři názvy jsou useknuté; rok 1965, první poválečné přijímání, jména osob, vztah „o rok později“ a politická příčinná interpretace zůstávají archivními tvrzeními. Na dvou snímcích je čitelný nápis **PRAVDA VÍTĚZÍ**.

Dávka 08 dokumentuje:

- malou skupinu dětí se ženou v liturgickém oděvu, archivně připisovanou obnovenému přijímání Janou Šilerovou;
- tři generačně rozdílné skupiny spojované s radou starších, z toho jednu datovanou názvem na 26. dubna 1970 a jednu výslovně nedatovanou;
- velký smíšený pěvecký sbor, archivně označený rokem 1933 a jmény Šlachta a Vodička;
- slabý kreslený znak na listu drženém uprostřed sborové fotografie, jehož přesný motiv ani text nelze bezpečně přečíst.

Názvy souborů `38` a `39` jsou useknuté právě v identifikačně významné části a nebyly doplněny odhadem.

Pracovní soubory dávky 08:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-08.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-08.yml`;
- `sources/index.d/urbanek-ccs-08.yml`;
- `research/urbanek-archive/uncertainties/open-11.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 26;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 60.

Nejistoty z kolekce CČS jsou vedeny pod `URB-U-0039` až `URB-U-0060`. Dávka 08 přidala:

- `URB-U-0058` – datum, kontext a osoby při obnoveném prvním přijímání;
- `URB-U-0059` – chronologie, členství a osoby na třech fotografiích rady starších včetně useknutého popisku `bisk…`;
- `URB-U-0060` – pěvecký sbor roku 1933, Šlachta, Vodička, členové a držený znak nebo dokument.

Dřívější aktivní položky zůstávají otevřené. Negativní dílčí hledání není důvodem k uzavření. Archivní název souboru je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, události nebo funkce. Osoby se neidentifikují pouze podle obličeje a useknuté názvy se nedoplňují odhadem.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 40 zpracovaných a 161 zbývajících položek;
- registr používá součty 26/31/3/60;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-041` až `urbanek-ccs-045`.
- Očekávané archivní názvy: soubory `43`, `44`, `45`, `46` a `47`; přesné mapování se ověří proti větvi před zápisem.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
