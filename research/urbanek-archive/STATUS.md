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

Dokončeno je šestnáct dávek po pěti snímcích, tedy `urbanek-ccs-001` až `080`.

Dosavadní stav nové kolekce:

- zpracováno: **80 z 201 položek**;
- proti Git blob SHA ověřeno: **80 položek**;
- vizuálně klasifikováno: **80 položek**;
- zdrojově indexováno: **80 položek**;
- zbývá: **121 položek**.

### Zjištění dávky 16

Dávka 16 uzavírá podsložku návštěvy archivně připisované Ferdinandu Stiborovi a otevírá sérii slavnostní volby a jmenování Gabriela Chrobáčka.

- `urbanek-ccs-076` zachycuje sedm sedících dospělých ve venkovním prostředí. Uprostřed je duchovní s řetězem nebo insignií a kyticí. Archivní název označuje skupinu jako biskupa Stibora s radou starších a obsahuje useknuté fragmenty jmen `Herman, nn,Trant. Šm`; pokračování nebylo rekonstruováno.
- `urbanek-ccs-077` zachycuje čtyři duchovní s výraznými řetězy nebo insigniemi, otevřenou velkou knihu a další účastníky v pozadí.
- `urbanek-ccs-078` zachycuje duchovního v kulatých brýlích držícího listy nebo dokument před skupinou přihlížejících.
- `urbanek-ccs-079` zachycuje obřad u oltáře se třemi hlavními duchovními, kalichem, knihami a dalším duchovním u pultu. Prostřední má přívěsek připomínající kalich.
- `urbanek-ccs-080` zachycuje zaplněný interiér se samostatnou přední řadou; nejméně dva muži v ní mají výrazné řetězy nebo insignie.
- Snímky `077–080` podle prostředí, pořadí a opakujících se účastníků pravděpodobně tvoří jednu obřadní posloupnost. Jméno Gabriel Chrobáček, volba, jmenování a neúplný rok `19…` však pocházejí z názvu podsložky a nejsou obrazem samostatně potvrzeny.

Pracovní soubory dávky 16:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-16.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-16.yml`;
- `sources/index.d/urbanek-ccs-16.yml`;
- rozšířené `research/urbanek-archive/uncertainties/open-08.yml` a `open-12.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 34;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 68.

Dávka 16 nepřidala nové ID. Rozšířila:

- `URB-U-0050` – úplnou Stiborovu podsložku, skupinu označenou jako rada starších a useknuté fragmenty jmen;
- `URB-U-0062` – úvodní část volby a jmenování, osoby s insigniemi, čtení dokumentu, obřad u oltáře, účastníky a neúplný rok v názvu podsložky.

Osoby se neidentifikují pouze podle obličeje. Řetěz nebo insignie sám neurčuje úřad a useknutá jména ani rok se nedoplňují odhadem.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 80 zpracovaných a 121 zbývajících položek;
- registr používá součty 34/31/3/68;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-081` až `urbanek-ccs-085`.
- Očekávané archivní názvy: `5  Syn Jaromír snacha Milena,dcera Miluše, manželka a paní S.jpg`, `6.jpg`, `7.jpg`, `8.jpg` a `9.jpg`.
- Název souboru `5` je useknutý za řetězcem `paní S`; pokračování ani rodinné vztahy se nesmějí domýšlet.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
