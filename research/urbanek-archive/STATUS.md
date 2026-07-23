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

Dokončeno je jedenáct dávek po pěti snímcích, tedy `urbanek-ccs-001` až `055`.

Dosavadní stav nové kolekce:

- zpracováno: **55 z 201 položek**;
- proti Git blob SHA ověřeno: **55 položek**;
- vizuálně klasifikováno: **55 položek**;
- zdrojově indexováno: **55 položek**;
- zbývá: **146 položek**.

### Zjištění dávky 11

Dávka 11 pokračuje ve fotografické sérii husovské vzpomínky a otevírá dokumentaci živého betléma.

- `urbanek-ccs-051` zachycuje venkovní průvod vedený mužem s českou vlajkou, za nímž kráčí dechová hudba a další účastníci. Vztah ke stejnému průvodu jako `urbanek-ccs-050` je pravděpodobný, nikoli definitivně potvrzený.
- `urbanek-ccs-052` zachycuje nezapálenou hranici z polen s připevněným kresleným portrétem a okolním davem.
- `urbanek-ccs-053` zachycuje tutéž konstrukci a portrét při hoření v detailu.
- `urbanek-ccs-054` zachycuje stejnou hořící hranici v širokém pohledu s početným davem a hasiči. Obraz dokládá početnou účast, nikoli přesný počet ani opakování tvrzené slovem „vždy“.
- Přesné obrazové porovnání potvrzuje, že `urbanek-ccs-052` až `054` tvoří posloupnost téže hranice před zapálením a při hoření. Spojení s konkrétním průvodem a ročníkem zůstává otevřené.
- `urbanek-ccs-055` zachycuje venkovní kostýmovanou scénu archivně označenou jako živý betlém. EXIF uvádí 10. prosince 2011 v 16:14:43 a fotoaparát Panasonic DMC-TZ3; datum musí být ještě potvrzeno programem nebo kronikou. Pořadatel, účinkující, role a vztah k místním ochotníkům nejsou ověřeny.

Pracovní soubory dávky 11:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-11.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-11.yml`;
- `sources/index.d/urbanek-ccs-11.yml`;
- `research/urbanek-archive/uncertainties/open-14.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-13.yml`.

Úplný inventář, blob verifikace, vizuální klasifikace, OCR relevantního textu a audit `Thumbs.db` pokračují po dávkách 5–10 souborů.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 32;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 66.

Nejistoty z kolekce CČS jsou vedeny pod `URB-U-0039` až `URB-U-0066`. Dávka 11:

- rozšířila `URB-U-0065` o průvod s dechovou hudbou a obrazově potvrzenou posloupnost hranice před zapálením a při hoření;
- přidala `URB-U-0066` – datum, pořadatel, lokalita, účinkující, role a opakování živého betléma včetně tvrzené účasti místních ochotníků.

Dřívější aktivní položky zůstávají otevřené. Negativní dílčí hledání není důvodem k uzavření. Archivní název souboru je dokladem archivního označení, nikoli automaticky ověřeného data, osoby, události nebo funkce. Osoby se neidentifikují pouze podle obličeje a technická data se používají jako historická datace až po věcném posouzení.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 55 zpracovaných a 146 zbývajících položek;
- registr používá součty 32/31/3/66;
- každá podstatná nejistota má stabilní ID a návratové podmínky;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-056` až `urbanek-ccs-060`.
- Očekávané archivní názvy: soubory `56`, `57`, `58`, `59` a `60`; přesné mapování se ověří proti větvi před zápisem.
- Snímek `56` porovnat s živým betlémem kvůli archivnímu tvrzení o místních ochotnících.
- Každá položka musí mít `repo_path`, `repo_status`, `git_blob_sha`, vizuální popis, stav práv a oddělený `document_text`/`scene_text`.
- Každá podstatná nejistota musí být okamžitě zapsána pod stabilním `URB-U-XXXX`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
