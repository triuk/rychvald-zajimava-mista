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

Dokončeno je dvacet dva dávek po pěti snímcích, tedy `urbanek-ccs-001` až `110`.

Dosavadní stav nové kolekce:

- zpracováno: **110 z 201 položek**;
- proti Git blob SHA ověřeno: **110 položek**;
- vizuálně klasifikováno: **110 položek**;
- zdrojově indexováno: **110 položek**;
- zbývá: **91 položek**.

### Zjištění dávky 22

Dávka 22 pokračuje v podsložce `5 Kaple CČS na Ostravici`.

- `urbanek-ccs-106` zachycuje uvítání duchovního mužem v obleku. Vložený popisek je čitelný jako „Uvítání br.biskupa zástupcem MNV“. Přepis je ověřen, identity, úřady, MNV, událost a datum nikoli.
- `urbanek-ccs-107` zachycuje nízkou tmavě dřevem obloženou stavbu na zalesněném svahu se sedlovou střechou, komínem a bílými okenicemi. Archivní název ji označuje jako chatku na Ostravici; vztah ke kapli není prokázán.
- `urbanek-ccs-108` zachycuje vysokou otevřenou dřevěnou věžovou konstrukci se stříškou, horní kovovou tyčí, kamennou nebo betonovou plošinou a venkovními lavicemi. Konstrukce odpovídá věži na historickém snímku `urbanek-ccs-102`, ale označení Winklerova zvonička, funkce a datace zůstávají k ověření.
- `urbanek-ccs-109` zachycuje pamětní desku s nápisem o Husově kapli, Winklerově zvonici, roce 1937 a prvním ostravském biskupu Ferdinandu Stiborovi.
- `urbanek-ccs-110` zachycuje druhou desku s údajem o stavbě od 21. 3. do 4. 7. 1937 za biskupa Ferdinanda Stibora a předsedy propagačního sboru Bohumíra Lišky podle návrhu architekta inženýra Alfreda Farníka z darů příslušníků CČS.
- U obou desek je ověřeno přesné znění hlavního nápisu. Nápis sám neověřuje historickou správnost tvrzení, dobu vzniku desky ani její autoritu.
- Dávka nepřidala nové ID a rozšířila `URB-U-0069` a `URB-U-0070`.

Pracovní soubory dávky 22:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-22.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-22.yml`;
- `sources/index.d/urbanek-ccs-22.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-17.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

Dávka 22 nepřidala nové ID. `URB-U-0069` nyní zahrnuje dřevěnou chatku, moderní detail staré zvonice, oba pamětní nápisy, rok 1937, Ferdinanda Stibora, Bohumíra Lišku a Alfreda Farníka. `URB-U-0070` byla rozšířena o uvítání biskupa zástupcem MNV.

Čitelné pamětní nebo stavební nápisy potvrzují své znění, nikoli automaticky historickou správnost údajů v nich.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 110 zpracovaných a 91 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-111` až `urbanek-ccs-115`.
- Očekávané archivní názvy v podsložce `5 Kaple CČS na Ostravici`: `6.jpg`, `7.jpg`, `8  Winklerova zvonička.jpg`, `8a  V r. 2016 byla stará zvonička demontována a nahrazena novou.jpg` a `8b.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
