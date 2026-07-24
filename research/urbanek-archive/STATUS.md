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

Dokončeno je dvacet dávek po pěti snímcích, tedy `urbanek-ccs-001` až `100`.

Dosavadní stav nové kolekce:

- zpracováno: **100 z 201 položek**;
- proti Git blob SHA ověřeno: **100 položek**;
- vizuálně klasifikováno: **100 položek**;
- zdrojově indexováno: **100 položek**;
- zbývá: **101 položek**.

### Zjištění dávky 20

Dávka 20 pokračuje v závěrečné části série archivně připisované volbě a jmenování Gabriela Chrobáčka.

- `urbanek-ccs-096` zachycuje ženu nebo dívku v bohatě zdobeném kroji s velkou kyticí před duchovním s řetězem nebo insignií. Identita, původ kroje ani role nejsou obrazem určeny.
- `urbanek-ccs-097` a `098` jsou užší a širší reprodukce téhož původního snímku: muž v obleku stojí vedle duchovního s řetězem, který drží světlou plastiku; mezi nimi je kytice.
- Přesné obrazové porovnání potvrdilo, že stejnou původní fotografii používá také dřívější `urbanek-ccs-046`. Tři soubory jsou archivně samostatné, ale představují pouze jeden nezávislý obrazový záznam.
- Porovnání současně opravilo starší interpretaci `urbanek-ccs-046`: samostatná listina není na třech reprodukcích spolehlivě rozeznatelná; světlý útvar odpovídá plastice a jejímu podstavci nebo drapérii.
- `urbanek-ccs-099` zachycuje duchovního s řetězem při vystoupení nebo čtení z listu papíru.
- `urbanek-ccs-100` zachycuje stojící shromáždění v dřevěných lavicích. Stejné prostředí a opakující se účastníci podporují vztah k `urbanek-ccs-080`, kde je přední řada zachycena vsedě.
- Jména, datum, úřady, původ kroje, role muže v obleku, námět a provenience plastiky ani přesné pořadí úkonů nejsou fotografiemi samostatně potvrzeny.

Pracovní soubory dávky 20:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-20.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-20.yml`;
- `sources/index.d/urbanek-ccs-20.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-12.yml`;
- opravené `historie-cirkve-ceskoslovenske-batch-10.yml` a `sources/index.d/urbanek-ccs-10.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 34;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 68.

Dávka 20 nepřidala nové ID. Rozšířila `URB-U-0062` o krojovanou gratulantku, tři reprodukce stejné fotografie, opravu interpretace listiny, proslov s papírem a vztah stojícího shromáždění k dřívějšímu záběru.

Osoby se neidentifikují pouze podle obličeje. Přesná shoda reprodukcí potvrzuje společnou fotografickou předlohu, nikoli nezávislé historické potvrzení události.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 100 zpracovaných a 101 zbývajících položek;
- registr používá součty 34/31/3/68;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-101` až `urbanek-ccs-105`.
- Očekávané archivní názvy: `25  S rychvaldskými občany.jpg`, poté v podsložce `5 Kaple CČS na Ostravici` soubory `1  Kaple CČS na Ostravici s  Winklerovou zvoničkou.jpg`, `2  Oltář, za ním okno s obrazem Jana  Husa.jpg`, `3.jpg` a `4.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
