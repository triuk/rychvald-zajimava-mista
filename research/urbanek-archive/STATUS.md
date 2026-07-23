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

Dokončeno je sedm dávek po pěti snímcích:

1. `urbanek-ccs-001` až `005` – položení základního kamene a výstavba;
2. `urbanek-ccs-006` až `010` – dokončený exteriér, původní interiér a rané slavnostní bohoslužby;
3. `urbanek-ccs-011` až `015` – první přijímání, rada starších a technické snímky zvonů;
4. `urbanek-ccs-016` až `020` – nástěnné malby, exteriéry spojované s okupacemi a skupina u varhan;
5. `urbanek-ccs-021` až `025` – svatební série, interiér před rekonstrukcí s varhanami a návštěva připisovaná Ferdinandu Stiborovi;
6. `urbanek-ccs-026` až `030` – rekonstruované kněžiště, bohoslužba, koberce a malby připisované Obšilovi;
7. `urbanek-ccs-031` až `035` – výroční shromáždění a velké skupiny prvního přijímání.

Dosavadní stav nové kolekce:

- zpracováno: **35 z 201 položek**;
- proti Git blob SHA ověřeno: **35 položek**;
- vizuálně klasifikováno: **35 položek**;
- zdrojově indexováno: **35 položek**;
- zbývá: **166 položek**.

### Zjištění dávky 07

- `urbanek-ccs-031` zachycuje mimořádně zaplněný hlavní prostor i galerie sboru; rok 1965 a výroční kontext jsou zatím pouze archivním tvrzením.
- `urbanek-ccs-032` zachycuje smíšenou slavnostní skupinu dětí, duchovního a dva civilní dospělé; označení prvního poválečného přijímání, jméno Chrobáček a řetězec `Anna Nedělo…` nejsou obrazem ověřeny.
- `urbanek-ccs-033` a `035` mohou představovat oddělenou dívčí a chlapeckou část téhož přijímání; `urbanek-ccs-034` může být následující ročník. Jde o pracovní hypotézu, nikoli identifikaci osob podle tváře.
- Na snímcích `urbanek-ccs-033` a `034` je čitelný fasádní nápis **PRAVDA VÍTĚZÍ**; na `034` také znak kalicha s křížem.
- Tři názvy souborů jsou zjevně useknuté. Chybějící text nebyl rekonstruován.
- Snímek početné skupiny sám nedokládá pozdější pokles účasti ani jeho politickou příčinu.

Pracovní soubory dávky 07:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-07.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-07.yml`;
- `sources/index.d/urbanek-ccs-07.yml`;
- `research/urbanek-archive/uncertainties/open-10.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 23;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 57.

Nejistoty z kolekce CČS jsou vedeny pod `URB-U-0039` až `URB-U-0057`. Dávka 07 přidala:

- `URB-U-0054` – datum a povaha výročí roku 1965, účast a úplné znění useknutého popisku;
- `URB-U-0055` – první poválečné přijímání, identita duchovního a osoby označené `Anna Nedělo…`;
- `URB-U-0056` – přesné roky, vztah skupin, počty a identity účastníků přijímání;
- `URB-U-0057` – doložení pozdějšího poklesu dětské účasti a případné příčinné vazby na politiku komunistického režimu.

Dřívější aktivní položky zůstávají otevřené. Negativní dílčí hledání není důvodem k uzavření. Archivní název souboru je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, události, technické historie nebo příčinné interpretace. Osoby se neidentifikují pouze podle obličeje a useknuté názvy se nedoplňují odhadem.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 35 zpracovaných a 166 zbývajících položek;
- registr používá součty 23/31/3/57;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-036` až `urbanek-ccs-040`.
- Očekávané archivní názvy: soubory `38`, `39`, `40`, `41` a `42`; přesné mapování se ověří proti větvi před zápisem.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
