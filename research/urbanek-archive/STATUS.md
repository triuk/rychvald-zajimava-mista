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

Dokončeno je patnáct dávek po pěti snímcích, tedy `urbanek-ccs-001` až `075`.

Dosavadní stav nové kolekce:

- zpracováno: **75 z 201 položek**;
- proti Git blob SHA ověřeno: **75 položek**;
- vizuálně klasifikováno: **75 položek**;
- zdrojově indexováno: **75 položek**;
- zbývá: **126 položek**.

### Zjištění dávky 15

Dávka 15 pokračuje v sérii návštěvy archivně připisované Ferdinandu Stiborovi.

- `urbanek-ccs-071` a `072` zachycují tutéž nebo bezprostředně navazující venkovní skupinu z odlišných záběrů. Opakují se účastníci a oděvy, ale jejich jména ani identita hlavního hosta nejsou obrazem potvrzeny.
- `urbanek-ccs-073` zachycuje menší skupinu dospělých a duchovních před oltářem.
- `urbanek-ccs-074` je další formální skupinový snímek duchovních a civilních účastníků.
- `urbanek-ccs-075` zachycuje velkou společnou skupinu dospělých, duchovních a dětí.
- Společná podsložka, pořadí, prostředí a opakující se osoby podporují jednu návštěvní sérii, nikoli však samy o sobě jméno Ferdinand Stibor, rok 1948 ani přesný program.

Pracovní soubory dávky 15:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-15.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-15.yml`;
- `sources/index.d/urbanek-ccs-15.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-08.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 34;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 68.

Dávka 15 nepřidala nové ID. Rozšířila `URB-U-0050` o venkovní záběry, skupinu před oltářem, formální skupinu a společnou fotografii s dětmi. Osoby se neidentifikují pouze podle obličeje a souvislost obrazové série sama nepotvrzuje datum ani funkce.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 75 zpracovaných a 126 zbývajících položek;
- registr používá součty 34/31/3/68;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-076` až `urbanek-ccs-080`.
- Očekávaný přechod: poslední soubor podsložky `3 Biskup Ferdinand Stibor v Rychvaldě` (`6 Biskup Stibor s radou starších...`) a první čtyři soubory podsložky `4 Slavnostní volba a jmenování biskupem Gabriela Chrobáčka...`; přesné mapování se ověří před zápisem.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.