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

Dokončeno je šest dávek po pěti snímcích:

1. `urbanek-ccs-001` až `005` – položení základního kamene a výstavba;
2. `urbanek-ccs-006` až `010` – dokončený exteriér, původní interiér a rané slavnostní bohoslužby;
3. `urbanek-ccs-011` až `015` – první přijímání, rada starších a technické snímky zvonů;
4. `urbanek-ccs-016` až `020` – nástěnné malby, exteriéry spojované s okupacemi a skupina u varhan;
5. `urbanek-ccs-021` až `025` – svatební série, interiér před rekonstrukcí s varhanami a skupinová návštěva připisovaná Ferdinandu Stiborovi;
6. `urbanek-ccs-026` až `030` – rekonstruované kněžiště, slavnostní bohoslužba, kobercová úprava a figurální malby připisované Obšilovi.

Dosavadní stav nové kolekce:

- zpracováno: **30 z 201 položek**;
- proti Git blob SHA ověřeno: **30 položek**;
- vizuálně klasifikováno: **30 položek**;
- zdrojově indexováno: **30 položek**;
- zbývá: **171 položek**.

Dávka 06 obrazově potvrzuje relativní posloupnost tří stavů kněžiště: zjednodušený stav po rekonstrukci, pozdější kobercovou úpravu a následnou figurální výzdobu čelní stěny. Tato posloupnost sama nepotvrzuje roky 1949 a 1957 uvedené v názvech souborů.

Na barevném snímku `urbanek-ccs-030` je v EXIF datum pořízení **28. srpna 2009**. Dokládá pořízení digitální fotografie, nikoli vznik maleb. Obrazově čitelné nápisy znějí:

- „NENARODÍ-LI SE KDO Z VODY A Z DUCHA, NEMŮŽE VEJÍTI DO KRÁLOVSTVÍ BOŽÍHO. JAN 3,5“;
- „KRISTUS VSTAL Z MRTVÝCH JAKO PRVNÍ Z TĚCH, KDOŽ ZESNULI. I KOR 15,20“.

Pracovní soubory dávky 06:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-06.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-06.yml`;
- `sources/index.d/urbanek-ccs-06.yml`;
- `research/urbanek-archive/uncertainties/open-09.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 19;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 53.

Nejistoty z kolekce CČS jsou vedeny pod `URB-U-0039` až `URB-U-0053`. Z dávek 05 a 06 nově přibyly:

- `URB-U-0048` – zda tři fotografie zachycují tutéž svatbu, její datace a identity osob;
- `URB-U-0049` – přesná chronologie rekonstrukce interiéru a vztah k varhanám, kobercům a pozdějším malbám;
- `URB-U-0050` – návštěva připisovaná Ferdinandu Stiborovi, její datum, účel, místo a osoby;
- `URB-U-0051` – slavnostní bohoslužba po rekonstrukci, její datum, účel, duchovní a tabule s čísly;
- `URB-U-0052` – datace, původ a financování koberců a identifikace zachycené události;
- `URB-U-0053` – plná identita malíře Obšila, vznik, technika, objednání a historie oprav maleb.

`URB-U-0046` byla rozšířena o další snímek interiéru s varhanními píšťalami. `URB-U-0049` nyní obsahuje celou dosud známou obrazovou posloupnost interiéru. Dřívější aktivní položky zůstávají otevřené. Negativní dílčí hledání není důvodem k uzavření.

Archivní název souboru je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, události nebo technické historie. Osoby se neidentifikují pouze podle obličeje.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 30 zpracovaných a 171 zbývajících položek;
- registr používá součty 19/31/3/53;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- stavový checkpoint po dávce 06 je commit `a927354c392b11d570eb9904fb472363e312083c`;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-031` až `urbanek-ccs-035`.
- Očekávané archivní názvy: soubory `33`, `34`, `35`, `36` a `37`; přesné mapování se ověří proti větvi před zápisem.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
