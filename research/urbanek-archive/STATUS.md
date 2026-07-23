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

Dokončeno je devět dávek po pěti snímcích, tedy `urbanek-ccs-001` až `045`.

Dosavadní stav nové kolekce:

- zpracováno: **45 z 201 položek**;
- proti Git blob SHA ověřeno: **45 položek**;
- vizuálně klasifikováno: **45 položek**;
- zdrojově indexováno: **45 položek**;
- zbývá: **156 položek**.

### Zjištění dávky 09

Dávka 09 dokumentuje čtyři novodobé snímky pěveckého sboru a hudebníků a jednu velkou historickou skupinu spojovanou s inaugurací Gabriela Chrobáčka.

- `urbanek-ccs-041` zachycuje smíšený sbor zpívající z notových desek; rok 2001 pochází pouze z archivního názvu.
- `urbanek-ccs-042` zachycuje sbor, komorní soubor a dirigenta před ozdobeným jehličnatým stromem. Výzdoba naznačuje vánoční období, nikoli sama o sobě přesnou událost.
- `urbanek-ccs-043` je skupinový portrét více než dvou desítek dospělých, jednoho dítěte a ženy v liturgické štole s motivem kalicha. EXIF datum **8. září 2014** dokládá digitální pořízení nebo reprodukci souboru, nikoli datum zachycené události.
- `urbanek-ccs-044` zachycuje varhanici, houslistku, další mladou ženu a část publika; příjmení Dziadziová a titul učitelky pocházejí z archivního názvu.
- `urbanek-ccs-045` zachycuje velkou skupinu před monumentálním vstupem a ústředního duchovního s řetězem nebo insignií. Inaugurace, jméno Gabriel Chrobáček a účast lidí z Rychvaldu pocházejí z useknutého archivního názvu končícího řetězcem `Rychv`.

Podobný interiér a opakující se osoby na snímcích `041–044` jsou vodítkem k souvislosti, nikoli důkazem jediné události.

Pracovní soubory dávky 09:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-09.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-09.yml`;
- `sources/index.d/urbanek-ccs-09.yml`;
- `research/urbanek-archive/uncertainties/open-12.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 28;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 62.

Nejistoty z kolekce CČS jsou vedeny pod `URB-U-0039` až `URB-U-0062`. Dávka 09 přidala:

- `URB-U-0061` – přesná data a vzájemný vztah novodobých sborových snímků, sbor, Dajč, Dziadziová, členové a program;
- `URB-U-0062` – inaugurace Gabriela Chrobáčka, její datum, místo, úřad, rychvaldská delegace, osoby a useknutý popisek.

Dřívější aktivní položky zůstávají otevřené. Negativní dílčí hledání není důvodem k uzavření. Archivní název souboru je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, události nebo funkce. Osoby se neidentifikují pouze podle obličeje a useknuté názvy se nedoplňují odhadem.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 45 zpracovaných a 156 zbývajících položek;
- registr používá součty 28/31/3/62;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-046` až `urbanek-ccs-050`.
- Očekávané archivní názvy: soubory `48`, `49`, `50`, `51` a `52`; přesné mapování se ověří proti větvi před zápisem.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
