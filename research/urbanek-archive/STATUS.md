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

Dokončeno je třicet dva dávek po pěti snímcích, tedy `urbanek-ccs-001` až `160`.

- zpracováno: **160 z 201 položek**;
- proti Git blob SHA ověřeno: **160 položek**;
- vizuálně klasifikováno: **160 položek**;
- zdrojově indexováno: **160 položek**;
- zbývá: **41 položek**.

### Zjištění dávky 32

Dávka 32 otevírá podsložku `7 Pohřeb biskupa br. Ferdinanda Stibora v říjnu 1956`.

- `urbanek-ccs-156` je venkovní portrét staršího muže. Jméno Ferdinand Stibor a rok 1956 pocházejí pouze z archivního názvu.
- `urbanek-ccs-157` a `158` zachycují stejný pohřební interiér s otevřenou rakví, viditelným tělem, vysokými svícemi, květinami a stojícími účastníky. Lokalizace do radvanického Husova sboru pochází z názvu `157`.
- Název `158` uvádí střídání čestné stráže. Fotografie potvrzuje stojící osoby u rakve, nikoli sama o sobě jejich formální status nebo střídání.
- `urbanek-ccs-159` zachycuje větší počet osob v dlouhých tmavých oděvech na schodech; nejméně čtyři mají výrazné řetězy nebo medailony.
- `urbanek-ccs-160` zachycuje početné venkovní shromáždění s prapory nebo korouhvemi.
- Žádný z pěti souborů neobsahuje použitelné embedded datum.
- Dávka vytvořila nové otevřené ID `URB-U-0071`.

Pracovní soubory dávky 32:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-32.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-32.yml`;
- `sources/index.d/urbanek-ccs-32.yml`;
- nové `research/urbanek-archive/uncertainties/open-18.yml`;
- aktualizovaný `research/urbanek-archive/uncertainties/index.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 37;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 71.

`URB-U-0071` odděleně sleduje identitu Ferdinanda Stibora na portrétu a v rakvi, datum a místo pohřbu, lokalizaci do radvanického Husova sboru, osoby stojící u rakve, tvrzení o čestné stráži, řetězy a medailony, prapory a sled obřadu.

Archivní názvy jsou atribuce, nikoli nezávislé potvrzení. Postoj u rakve, uniformní prvek, dlouhý oděv, řetěz nebo medailon samy neurčují identitu, úřad ani formální status čestné stráže.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 160 zpracovaných a 41 zbývajících položek;
- registr používá součty 37/31/3/71;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-161` až `urbanek-ccs-165`.
- Očekávané názvy v téže podsložce: `6.jpg`, `7.jpg`, `8.jpg`, `9.jpg` a `10.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
