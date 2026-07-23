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

Dokončeno je dvanáct dávek po pěti snímcích, tedy `urbanek-ccs-001` až `060`.

Dosavadní stav nové kolekce:

- zpracováno: **60 z 201 položek**;
- proti Git blob SHA ověřeno: **60 položek**;
- vizuálně klasifikováno: **60 položek**;
- zdrojově indexováno: **60 položek**;
- zbývá: **141 položek**.

### Zjištění dávky 12

Dávka 12 rozšiřuje dokumentaci živého betléma, přináší dva koncertní záběry a dokumentuje pamětní desku a portrét Karla Vodičky.

- `urbanek-ccs-056` zachycuje kostýmovanou scénu živého betléma se zřetelně živým dítětem. Archivní název tvrdí, že účinkují místní ochotníci. EXIF uvádí 6. prosince 2008 v 16:04:44 a fotoaparát Sony DCR-HC96E.
- Předchozí `urbanek-ccs-055` má EXIF 10. prosince 2011. Jde tedy o nejméně dvě digitální série; přesná data veřejných ročníků musí potvrdit program nebo kronika. Živé dítě na snímku 056 neurčuje povahu dětské postavy na snímku 055.
- `urbanek-ccs-057` zachycuje velký smíšený sbor s dirigentem a publikem. Archivní název jej připisuje Svatováclavskému festivalu; EXIF uvádí 12. června 2011 v 17:02:40.
- `urbanek-ccs-058` zachycuje dětský a mládežnický hudební soubor. Název jej připisuje adventnímu koncertu a místní ZUŠ, ale EXIF stejného fotoaparátu uvádí 12. června 2011 v 16:13:05. Shodný den, fotoaparát, interiér a časová návaznost silně ukazují na společnou akci; označení adventního koncertu je s červnovým datem v konfliktu.
- `urbanek-ccs-059` zachycuje čitelnou pamětní desku Karla a Libuše Vodičkových. Nápis označuje Karla Vodičku za prvního faráře zdejší náboženské obce, budovatele sboru a spoluzakladatele Církve československé husitské. Přepis dokládá znění desky, nikoli automaticky historickou správnost tvrzení. Archivní název končí řetězcem `umíst`; obsah za deskou nebyl domýšlen.
- `urbanek-ccs-060` zachycuje muže v duchovním oděvu a brýlích. Identifikace jako ThDr. Karel Vodička a první farář pochází z archivního názvu a musí být potvrzena dokumentárně.

Pracovní soubory dávky 12:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-12.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-12.yml`;
- `sources/index.d/urbanek-ccs-12.yml`;
- `research/urbanek-archive/uncertainties/open-15.yml`;
- rozšířené `research/urbanek-archive/uncertainties/open-12.yml` a `open-14.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 33;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 67.

Nejistoty z kolekce CČS jsou vedeny pod `URB-U-0039` až `URB-U-0067`. Dávka 12:

- rozšířila `URB-U-0061` o dva koncertní záběry, jejich společné červnové datum a konflikt mezi označením Svatováclavského festivalu a adventního koncertu;
- rozšířila `URB-U-0066` o druhou sérii živého betléma z embedded roku 2008 a archivní tvrzení o místních ochotnících;
- přidala `URB-U-0067` – instalace a obsah pamětní desky, neznámý obsah za ní, životopisná tvrzení o Karlu a Libuši Vodičkových a provenience portrétu.

Dřívější aktivní položky zůstávají otevřené. Negativní dílčí hledání není důvodem k uzavření. Archivní název souboru je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, události nebo funkce. Čitelný nápis dokládá text na objektu, nikoli automaticky správnost všech jeho historických tvrzení.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 60 zpracovaných a 141 zbývajících položek;
- registr používá součty 33/31/3/67;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-061` až `urbanek-ccs-065`.
- První tři očekávané archivní názvy jsou `61 Biskup Gabriel Chrobáček`, `62 Farář Leonard Bogumski` a `63 Biskupka Mgr Jana Šilerová`; další dvě položky již přecházejí do druhé podsložky a jejich přesné mapování se ověří před zápisem.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
