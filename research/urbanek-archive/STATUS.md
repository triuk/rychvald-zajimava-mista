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

Dokončeny jsou tři dávky po pěti snímcích:

1. `urbanek-ccs-001` až `005` – položení základního kamene a výstavba;
2. `urbanek-ccs-006` až `010` – dokončený exteriér, původní interiér a rané slavnostní bohoslužby;
3. `urbanek-ccs-011` až `015` – první přijímání, rada starších a technické snímky zvonů.

Dosavadní stav nové kolekce:

- zpracováno: **15 z 201 položek**;
- proti Git blob SHA ověřeno: **15 položek**;
- vizuálně klasifikováno: **15 položek**;
- zdrojově indexováno: **15 položek**;
- zbývá: **186 položek**.

Dávka 03 ověřila obrazově zejména společný vstup na skupinových fotografiích, částečný popisek desetiletí CČS v Rychvaldě s rokem 1930, letopočet `1920` na jednom zvonu a existenci nejméně tří zvonů. Význam letopočtu, identita osob a historie zvonění zůstávají otevřené.

Pracovní soubory dávky 03:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-03.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-03.yml`;
- `sources/index.d/urbanek-ccs-03.yml`;
- `research/urbanek-archive/uncertainties/open-06.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 8;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 42.

Nově založené položky:

- `URB-U-0039` – datace a osoby na fotografiích prvního přijímání;
- `URB-U-0040` – úplný popisek, událost a osoby rady starších roku 1930;
- `URB-U-0041` – význam letopočtu 1920, původ a identita zvonů;
- `URB-U-0042` – původní ovládání, elektrifikace a změny mechanismu zvonění.

Dřívější aktivní položky `URB-U-0008`, `URB-U-0036`, `URB-U-0037` a `URB-U-0038` zůstávají otevřené. Negativní dílčí hledání není důvodem k uzavření. Archivní název souboru je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, události nebo technické historie.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 15 zpracovaných a 186 zbývajících položek;
- registr používá součty 8/31/3/42;
- každá nejistota z dávky 03 má stabilní ID a vlastní návratové podmínky;
- GitHub nevrací pro kontrolovaný head žádné CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-016` až `urbanek-ccs-020`.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
