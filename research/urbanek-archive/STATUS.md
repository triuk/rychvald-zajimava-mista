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

Dokončeno je třicet dávek po pěti snímcích, tedy `urbanek-ccs-001` až `150`.

- zpracováno: **150 z 201 položek**;
- proti Git blob SHA ověřeno: **150 položek**;
- vizuálně klasifikováno: **150 položek**;
- zdrojově indexováno: **150 položek**;
- zbývá: **51 položek**.

### Zjištění dávky 30

Dávka 30 pokračuje v podsložce `6 Červen 1970. Pohřeb br. faráře ThDr Karla Vodičky.  Husova Č (1)`.

- `urbanek-ccs-146` zachycuje stojící osobu v dlouhém tmavém oděvu u rakve nebo katafalku, věnců, svící a řad sedících účastníků.
- `urbanek-ccs-147` je široký pohled na zaplněný interiér pod varhanní kruchtou; několik osob v přední řadě drží kapesníky nebo ruce u obličeje.
- `urbanek-ccs-148` zachycuje vynášení rakve z budovy označené čitelným nápisem „HUSOVA ČESKOSLOVENSKÁ BOHOSLOVECKÁ FAKULTA V PRAZE“. Nápis dokládá označení budovy, nikoli sám o sobě identitu zemřelého, datum, přesnou adresu nebo konkrétní místnost obřadu.
- `urbanek-ccs-149` zachycuje před stejným vstupem nejméně dvě salutující uniformované osoby, osobu s četnými dekoracemi, účastníky ve dveřích a číslo 5 na fasádě.
- `urbanek-ccs-150` navazuje na tutéž situaci; jde o odlišný snímek, nikoli binární duplikát položky `149`.
- Žádný z pěti souborů neobsahuje použitelné embedded datum.
- Dávka nepřidala nové ID. Rozšířila `URB-U-0067`.

Pracovní soubory dávky 30:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-30.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-30.yml`;
- `sources/index.d/urbanek-ccs-30.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-15.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

`URB-U-0067` nyní zahrnuje také pokračování pohřební série, čitelný nápis Husovy československé bohoslovecké fakulty v Praze, číslo 5 na fasádě, vynášení rakve, salutující uniformované osoby a osobu s četnými dekoracemi.

Čitelný nápis dokládá označení zachycené budovy, nikoli automaticky identitu zemřelého, datum nebo přesnou adresu. Salutování je obrazově ověřitelné gesto; organizace osob ani status čestné stráže z něj samy nevyplývají.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 150 zpracovaných a 51 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-151` až `urbanek-ccs-155`.
- Očekávané názvy: `10.jpg`, `11.jpg`, `12  Před oltářem v Rychvaldě.jpg`, `13  Fotografie Karla Vodičky.jpg` a `14  Pamětní deska v kostele v Rychvaldě, za níž jsou uloženy.JPG` v téže podsložce.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
