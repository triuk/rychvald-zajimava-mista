# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový kořen: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt bylo potvrzeno.
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Autoritativním pracovním úložištěm je Git repozitář.

## Draft pull request

- PR: [#1 – Import and classify Jaromír Urbánek archive (pilot + CČS batch)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

## Dokončený pilot

| Kolekce | Obsahové soubory | Technické soubory | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | dokončeno |
| Články z Českého slova | 37 | 2 | 39 | dokončeno |
| Ochotníci rychvald | 61 | 2 | 63 | dokončeno |
| fotodokument/den po dešti | 8 | 2 | 10 | dokončeno |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | dokončeno |
| **Celkem** | **144** | **15** | **159** | **159 z 159 položek přítomno** |

Audity pilotních cache prokázaly **11 chybějících plných originálů** dochovaných pouze jako náhledy.

## Kolekce historie Církve československé

Kolekce: `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`

- 10 tematických podsložek;
- 200 JPEGů;
- 1 technický soubor `Thumbs.db`;
- celkem 201 položek;
- stav: `processing_in_progress`.

Dokončeno je třicet pět dávek po pěti snímcích, tedy `urbanek-ccs-001` až `175`.

- zpracováno: **175 z 201 položek**;
- proti Git blob SHA ověřeno: **175 položek**;
- vizuálně klasifikováno: **175 položek**;
- zdrojově indexováno: **175 položek**;
- zbývá: **26 položek**.

### Zjištění dávky 35

Dávka 35 uzavírá podsložku `7 Pohřeb biskupa br. Ferdinanda Stibora v říjnu 1956`.

- `urbanek-ccs-171` zachycuje několik oddělených skupin nesoucích velké květinové věnce v uličním průvodu.
- `urbanek-ccs-172` zachycuje osoby v dlouhých tmavých oděvech; několik drží knihy, desky nebo jiné obdélné předměty.
- `urbanek-ccs-173` je široký pohled na dlouhou řadu podobně oděných osob, za nimiž je nesena zdobená uzavřená rakev a následuje početný zástup.
- `urbanek-ccs-174` je bližší záběr stejné nebo bezprostředně navazující situace s rakví. Nejde o binární duplikát položek `166`, `169` ani `173`.
- `urbanek-ccs-175` zachycuje početný civilní zástup s muži, ženami a dětmi; rakev v tomto výřezu viditelná není.
- Všech pět souborů má odlišné Git blob SHA a žádný nemá použitelné embedded datum.
- Dávka nepřidala nové ID a rozšířila `URB-U-0071`.
- Všech 20 JPEGů v sedmé podsložce je nyní vizuálně klasifikováno a proti Git blob SHA ověřeno.

Pracovní soubory dávky 35:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-35.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-35.yml`;
- `sources/index.d/urbanek-ccs-35.yml`;
- aktualizované `research/urbanek-archive/uncertainties/open-18.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 37;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 71.

`URB-U-0071` nyní zahrnuje položky `156` až `175`: portrét, vystavení a nesení rakve, věnce, osoby u rakve, výstup ze sboru, schodiště, uliční průvod, řetězy, medailony, knihy, znaky připomínající kalich, pásku s křížovitým znakem, prapory a civilní účastníky.

Archivní názvy jsou atribuce, nikoli nezávislé potvrzení. Oděv, řetěz, medailon, znak, pokrývka hlavy, páska na paži, kniha, věnec, nesení rakve nebo postavení v průvodu samy neurčují identitu, úřad, organizaci, dárce nebo formální roli.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 175 zpracovaných a 26 zbývajících položek;
- registr používá součty 37/31/3/71;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-176` až `urbanek-ccs-180`.
- Očekávané názvy v podsložce `8 Farář Leonard Bogumský v Doubravě u příležitosti neznámých oslav`: `1.jpg`, `2.jpg`, `3.jpg`, `4.jpg` a `5.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
