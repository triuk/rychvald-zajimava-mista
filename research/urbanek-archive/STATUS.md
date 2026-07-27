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

## Dokončený pilot

| Kolekce | Obsahové soubory | Technické soubory | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | klasifikace a první OCR dokončeny |
| Články z Českého slova | 37 | 2 | 39 | OCR a druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | 61 | 2 | 63 | textový průchod a druhá vizuální kontrola dokončeny |
| fotodokument/den po dešti | 8 | 2 | 10 | audit a vizuální klasifikace dokončeny |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | audit a vizuální klasifikace dokončeny |
| **Celkem** | **144** | **15** | **159** | **159 z 159 položek přítomno** |

Audity pilotních cache prokázaly **11 chybějících plných originálů**. Náhled v `Thumbs.db` není náhradou plného originálu.

## Nová dávka – historie Církve československé

Kolekce: `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`

- 10 tematických podsložek;
- 200 JPEGů;
- 1 technický soubor `Thumbs.db`;
- celkem 201 položek;
- stav: `processing_in_progress`;
- pilotní součty se touto dávkou nemění.

Dokončeno je dvacet čtyři dávek po pěti snímcích, tedy `urbanek-ccs-001` až `120`.

Dosavadní stav nové kolekce:

- zpracováno: **120 z 201 položek**;
- proti Git blob SHA ověřeno: **120 položek**;
- vizuálně klasifikováno: **120 položek**;
- zdrojově indexováno: **120 položek**;
- zbývá: **81 položek**.

### Zjištění dávky 24

Dávka 24 pokračuje v podsložce `5 Kaple CČS na Ostravici`.

- `urbanek-ccs-116` zachycuje společně novou dřevěnou zvonici, nízkou bílou kapli, pamětní desku, střešní znak kříže a kalicha, kamennou zídku a jednu vzdálenou neidentifikovanou osobu.
- `urbanek-ccs-117` zachycuje čelní fasádu kaple se širokým tmavým vstupem nebo dveřní výplní, pamětní deskou a střešním znakem.
- `urbanek-ccs-118` je detail stejné fyzické pamětní desky jako `urbanek-ccs-109`. Hlavní nápis je totožný; jde o druhou fotografii stejného objektu, nikoli druhé nezávislé historické svědectví. Drobná značka vlevo dole zůstává jen částečně čitelná.
- `urbanek-ccs-119` zachycuje detail kovového střešního znaku tvořeného křížem a stylizovaným kalichem.
- EXIF položek `116–119` uvádí pořízení 2. října 2016 v časech 14:05:52 až 14:07:01. Spolu s položkami `114–115` jde o souvislou fotografickou sérii areálu dlouhou 2 minuty a 38 sekund.
- `urbanek-ccs-120` zachycuje duchovního v brýlích s kyticí a insignií s motivem kalicha. Vložený popisek zní „Biskup dr.Horský“; rozmezí 1945–1946 pochází pouze z archivního názvu. Osoba, doktorát, úřad, datum a vztah k useknutému popisku na `urbanek-ccs-037` nejsou nezávisle ověřeny.
- Dávka nepřidala nové ID. Rozšířila `URB-U-0069` a starší `URB-U-0059`.

Pracovní soubory dávky 24:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-24.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-24.yml`;
- `sources/index.d/urbanek-ccs-24.yml`;
- rozšířené `research/urbanek-archive/uncertainties/open-11.yml` a `open-17.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

Dávka 24 nepřidala nové ID. `URB-U-0069` nyní zahrnuje také celkový stav areálu 2. října 2016, průčelí kaple, další fotografii stejné pamětní desky a střešní znak kříže a kalicha. `URB-U-0059` byla rozšířena o portrét s popiskem „Biskup dr.Horský“ a otázku jeho vztahu ke skupině rady starších z let 1945–1946.

EXIF datum může podporovat, že objekt existoval v okamžiku pořízení fotografie; samo neprokazuje datum stavby, demontáže nebo instalace. Druhá fotografie stejného fyzického nápisu není druhým nezávislým historickým pramenem.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 120 zpracovaných a 81 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-121` až `urbanek-ccs-125`.
- Očekávané archivní názvy v podsložce `5 Kaple CČS na Ostravici`: `10.jpg`, `11 Celkový pohled na účastníky slavnosti asi v r. 1945 nebo .jpg`, `12  Průvod účastníků.jpg`, `13  Krojovaní, prapory sborů a děti v průvodu.jpg` a `14  Účast duchovních.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
