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

Dokončeno je dvacet devět dávek po pěti snímcích, tedy `urbanek-ccs-001` až `145`.

- zpracováno: **145 z 201 položek**;
- proti Git blob SHA ověřeno: **145 položek**;
- vizuálně klasifikováno: **145 položek**;
- zdrojově indexováno: **145 položek**;
- zbývá: **56 položek**.

### Zjištění dávky 29

Dávka 29 uzavírá podsložku `5 Kaple CČS na Ostravici` a otevírá podsložku `6 Červen 1970. Pohřeb br. faráře ThDr Karla Vodičky.  Husova Č (1)`.

- `urbanek-ccs-141` zachycuje velký skupinový portrét dospělých a dětí před vstupem do budovy. Archivní název uvádí přibližný rok 1947 a zájezd Rychvaldských s biskupem; obraz sám datum, místo ani biskupa neurčuje.
- `urbanek-ccs-142` zachycuje rakev pod krucifixem, četné věnce, květiny a svíce a čtyři uniformované muže; dva v popředí mají viditelné dekorace nebo medaile.
- `urbanek-ccs-143` je široký pohled do téhož interiéru s rakví, dvěma viditelnými uniformovanými strážnými a početným shromážděním.
- `urbanek-ccs-144` a `145` zachycují rakev a čtyři osoby v dlouhých tmavých oděvech nebo pláštích; jejich identity ani přesné role nejsou obrazem určeny.
- Název podsložky připisuje položky `142` až `145` pohřbu faráře ThDr. Karla Vodičky v červnu 1970. Jde o archivní atribuci, nikoli samostatné obrazové potvrzení.
- Žádný z pěti souborů neobsahuje použitelné embedded datum.
- Dávka nepřidala nové ID. Rozšířila `URB-U-0067` a `URB-U-0070`.

Pracovní soubory dávky 29:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-29.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-29.yml`;
- `sources/index.d/urbanek-ccs-29.yml`;
- rozšířené `research/urbanek-archive/uncertainties/open-15.yml` a `open-17.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

`URB-U-0067` nyní zahrnuje také první čtyři fotografie pohřební série: rakev, výzdobu, uniformované muže stojící u rakve, shromáždění a čtyři osoby v dlouhých tmavých oděvech. `URB-U-0070` byla rozšířena o závěrečný skupinový portrét ostravické podsložky a archivní tvrzení o přibližném roce 1947, zájezdu Rychvaldských a přítomnosti biskupa.

Název složky nebo souboru je archivní atribuce, nikoli nezávislé potvrzení osoby, data nebo události. Oděv, uniforma ani poloha v obraze samy neurčují identitu nebo funkci.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 145 zpracovaných a 56 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-146` až `urbanek-ccs-150`.
- Očekávané názvy: `5.jpg`, `6.jpg`, `7.jpg`, `8.jpg` a `9.jpg` v podsložce `6 Červen 1970. Pohřeb br. faráře ThDr Karla Vodičky.  Husova Č (1)`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
