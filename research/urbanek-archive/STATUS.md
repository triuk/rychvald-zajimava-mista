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

Dokončeno je devatenáct dávek po pěti snímcích, tedy `urbanek-ccs-001` až `095`.

Dosavadní stav nové kolekce:

- zpracováno: **95 z 201 položek**;
- proti Git blob SHA ověřeno: **95 položek**;
- vizuálně klasifikováno: **95 položek**;
- zdrojově indexováno: **95 položek**;
- zbývá: **106 položek**.

### Zjištění dávky 19

Dávka 19 pokračuje v obřadní a investiční části série archivně připisované volbě a jmenování Gabriela Chrobáčka.

- `urbanek-ccs-091` zachycuje vystoupení duchovního s řetězem nebo insignií na vyvýšeném stupni před dalšími duchovními a shromážděním.
- `urbanek-ccs-092` obrazově dokládá fyzické nasazení řetězu nebo insignie skloněnému duchovnímu. Fotografie sama neurčuje identitu příjemce, jeho úřad ani právní či liturgický význam aktu.
- `urbanek-ccs-093` zachycuje dva hlavní duchovní s řetězy u oltáře, před nimi kalich a otevřenou knihu.
- `urbanek-ccs-094` zachycuje setkání dvou duchovních; jeden drží složený list či dokument a druhý k němu natahuje ruku. Není jisté, zda jde o předání, čtení nebo pouze držení listiny.
- `urbanek-ccs-095` zachycuje stojícího duchovního s řetězem při proslovu, modlitbě nebo zpěvu a sedícího duchovního s otevřenou složkou či knihou.
- Snímky `091–095` navazují prostředím a opakujícími se osobami na předchozí obřadní sérii. Jména, úřady, datum, obsah dokumentu a přesná funkce insignie zůstávají otevřené.

Pracovní soubory dávky 19:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-19.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-19.yml`;
- `sources/index.d/urbanek-ccs-19.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-12.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 34;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 68.

Dávka 19 nepřidala nové ID. Rozšířila `URB-U-0062` o fyzické nasazení insignie, proslovy, listinu nebo složený dokument a úplnější investiční posloupnost.

Osoby se neidentifikují pouze podle obličeje. Řetěz nebo insignie sám neurčuje úřad a ani jeho fyzické nasazení samo nepotvrzuje identitu příjemce nebo právní význam aktu.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 95 zpracovaných a 106 zbývajících položek;
- registr používá součty 34/31/3/68;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-096` až `urbanek-ccs-100`.
- Očekávané archivní názvy: `20.jpg`, `21.jpg`, `22.jpg`, `23.jpg` a `24.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
