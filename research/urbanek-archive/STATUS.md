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

Audity pilotních cache prokázaly **11 chybějících plných originálů**:

- 0 – Rychvaldské větrné mlýny;
- 8 – Články z Českého slova;
- 2 – Ochotníci rychvald;
- 1 – `den po dešti`;
- 0 – Nálet na Ostravu 1944.

Náhled v `Thumbs.db` není náhradou plného originálu. Přesně ověřená kopie obrazu dochovaná pod jiným názvem se však nepovažuje za další chybějící obrazový obsah.

## Nová dávka – historie Církve československé

Kolekce: `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`

- 10 tematických podsložek;
- 200 JPEGů;
- 1 technický soubor `Thumbs.db`;
- celkem 201 položek;
- stav: `processing_in_progress`;
- pilotní součty se touto dávkou nemění.

První dávka pěti snímků dokumentujících položení základního kamene a výstavbu byla:

- vizuálně zkontrolována;
- položkově inventarizována;
- ověřena proti Git blob SHA;
- zapsána do kolekčního zdrojového indexu;
- klasifikována se samostatným `document_text` a `scene_text`.

Pracovní soubory:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-overview.yml`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-01.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-01.yml`;
- `sources/index.d/urbanek-ccs.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 4;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 38.

Aktivní zůstávají:

- `URB-U-0008` – neidentifikovaná historická fotografie větrného mlýna;
- `URB-U-0036` – poloha a historie Kakalova mlýna;
- `URB-U-0037` – význam `304` a archivní vztah fotografie kostela;
- `URB-U-0038` – historická poloha a vlastník mlýnku za domem č. 339.

Tyto otázky se znovu prověří pouze tehdy, přinese-li nová dávka relevantní podklad. Negativní dílčí hledání není důvodem k jejich uzavření.

## Kontrola konzistence draftu

Provedeno:

- součty registru sjednoceny na 4/31/3/38;
- pilot oddělen od nové dávky;
- popis a název PR aktualizovány podle skutečného obsahu větve;
- dočasný export a fragmenty k `URB-U-0032` odstraněny;
- nový kolekční přehled, inventář, klasifikace a zdrojový shard vytvořeny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejné součty nové dávky: 200 + 1 = 201.

GitHub pro aktuální head nevrací žádné CI status checks; nejde tedy o úspěšně proběhlý test, ale o repozitář bez hlášených kontrol.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-006` až `urbanek-ccs-010`.
- Pokračovat po dávkách 5–10 souborů.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
