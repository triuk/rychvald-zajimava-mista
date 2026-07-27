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

Dokončeno je třicet jedna dávek po pěti snímcích, tedy `urbanek-ccs-001` až `155`.

- zpracováno: **155 z 201 položek**;
- proti Git blob SHA ověřeno: **155 položek**;
- vizuálně klasifikováno: **155 položek**;
- zdrojově indexováno: **155 položek**;
- zbývá: **46 položek**.

### Zjištění dávky 31

Dávka 31 uzavírá podsložku `6 Červen 1970. Pohřeb br. faráře ThDr Karla Vodičky.  Husova Č (1)`.

- `urbanek-ccs-151` pokračuje venkovní sérií před vstupem Husovy československé bohoslovecké fakulty v Praze; zachycuje civilní, uniformované a osoby v dlouhých tmavých oděvech.
- `urbanek-ccs-152` zachycuje ženu v tmavém oděvu mezi dvěma muži, kteří ji drží nebo podpírají za paže. Identity, vzájemné vztahy a důvod podpory nejsou obrazem určeny.
- `urbanek-ccs-153` zachycuje oltář s krucifixem, svícemi, květinami a rámovaným portrétem s černou stuhou. Lokalizace před oltář v Rychvaldě pochází z archivního názvu.
- `urbanek-ccs-154` je bližší záběr stejného pietního uspořádání. Identifikace portrétu jako Karla Vodičky pochází z archivního názvu, nikoli z rozpoznání obličeje.
- `urbanek-ccs-155` je přesný binární duplikát položky `059` pod jinou archivní cestou. Deska uvádí jména Karel Vodička a Libuše Vodičková, jejich životní data a role Karla Vodičky; nápis dokládá své znění, nikoli automaticky historickou správnost.
- Fotografická metadata položky `155` uvádějí `2010-10-14 17:45:12`; jde o datum pořízení digitální fotografie, ne instalace desky.
- Archivní názvy položek `059` a `155` neuvádějí, co je za deskou umístěno nebo uloženo. Obsah nelze doplnit odhadem.
- Dávka nepřidala nové ID a rozšířila `URB-U-0067`.

Pracovní soubory dávky 31:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-31.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-31.yml`;
- `sources/index.d/urbanek-ccs-31.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-15.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

`URB-U-0067` nyní zahrnuje celou pohřební podsložku, dvojici pietních záběrů před oltářem, archivní identifikaci portrétu, přesný duplikát pamětní desky a stále neúplné tvrzení o obsahu za deskou.

Přesná binární duplicita je samostatná archivní položka, nikoli další nezávislý obrazový důkaz. Čitelné jméno nebo role na desce potvrzuje znění nápisu; správnost vyžaduje nezávislý pramen.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 155 zpracovaných a 46 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-156` až `urbanek-ccs-160`.
- Očekávané názvy v podsložce `7 Pohřeb biskupa br. Ferdinanda Stibora v říjnu 1956`: `1   Ferdinand Stibor ještě v r. 1956.jpg`, `2  V radvanickém Husově sboru.jpg`, `3  U rakve se střídala čestná stráž.jpg`, `4.jpg` a `5.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
