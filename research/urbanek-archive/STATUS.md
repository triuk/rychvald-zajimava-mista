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

Dokončeno je osmnáct dávek po pěti snímcích, tedy `urbanek-ccs-001` až `090`.

Dosavadní stav nové kolekce:

- zpracováno: **90 z 201 položek**;
- proti Git blob SHA ověřeno: **90 položek**;
- vizuálně klasifikováno: **90 položek**;
- zdrojově indexováno: **90 položek**;
- zbývá: **111 položek**.

### Zjištění dávky 18

Dávka 18 pokračuje v obřadní a gratulační části série archivně připisované volbě a jmenování Gabriela Chrobáčka.

- `urbanek-ccs-086` zachycuje dva stojící duchovní s řetězy nebo insigniemi a třetího skloněného či klečícího duchovního. Jeden stojící muž drží ruku nad jeho hlavou, druhý knihu; mezi nimi je vysoká svíce. Přesný význam úkonu není obrazem určen.
- `urbanek-ccs-087` zachycuje skupinu duchovních u oltáře s otevřenou knihou, kalichem a mužem s řetězem držícím další knihu.
- `urbanek-ccs-088` je detail početné skupiny duchovních s kalichem a otevřenou knihou. Otevřená ústa několika osob mohou znamenat zpěv nebo recitaci, nikoli však doložený konkrétní text.
- `urbanek-ccs-089` zachycuje duchovního s řetězem nebo insignií držícího kalich před oltářem.
- `urbanek-ccs-090` zachycuje pozdrav nebo předání mezi duchovním a skupinou čtyř žen. Označení „manželka“ pochází pouze z archivního názvu a neurčuje, která žena je míněna.
- Snímky `086–089` tvoří podle prostředí a opakujících se osob pravděpodobnou obřadní posloupnost. Absolutní datum, osoby, úřady, význam řetězů a přesné rituály zůstávají otevřené.

Pracovní soubory dávky 18:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-18.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-18.yml`;
- `sources/index.d/urbanek-ccs-18.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-12.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 34;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 68.

Dávka 18 nepřidala nové ID. Rozšířila `URB-U-0062` o položení ruky, úkony s knihou a kalichem, gratulaci označenou jako gratulace manželce a další podmínky dokumentárního ověření.

Osoby se neidentifikují pouze podle obličeje. Řetěz nebo insignie sám neurčuje úřad, gesto neurčuje přesný rituál a rodinné vztahy z názvů se nepovažují za obrazově ověřené.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 90 zpracovaných a 111 zbývajících položek;
- registr používá součty 34/31/3/68;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-091` až `urbanek-ccs-095`.
- Očekávané archivní názvy: `15.jpg`, `16.jpg`, `17.jpg`, `18.jpg` a `19.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
