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
- stav: `content_complete_technical_audit_pending`.

Dokončeno je čtyřicet dávek po pěti snímcích, tedy `urbanek-ccs-001` až `200`.

- zpracováno: **200 z 201 položek**;
- proti Git blob SHA ověřeno: **200 obrazových položek**;
- vizuálně klasifikováno: **200 obrazových položek**;
- zdrojově indexováno: **200 obrazových položek**;
- zbývá: **1 technický soubor**.

### Zjištění dávky 40

Dávka 40 dokončila všech patnáct obrazových stran podsložky `10 Kalendář 2015` a tím všech 200 JPEGů kolekce.

- `urbanek-ccs-196` je zářijová strana s nástěnnými malbami. Znovu používá položky `017`, `016` a `030`; popisky připisují starší malby akademickému malíři Hanusovi roku 1932 a obrazy na čelní stěně akademickému malíři Obšilovi roku 1957.
- `urbanek-ccs-197` je říjnová strana. Znovu používá exteriér `018` a obsahuje dosud nepřiřazenou oltářní fotografii. Text tvrdí odstranění hesla „Pravda vítězí“ a kalicha po okupaci roku 1938 a neoprávněné přesvěcení sboru v srpnu 1939.
- `urbanek-ccs-198` je listopadová strana. Znovu používá koncertní položky `057` a `058`; detail varhan a varhanice nebyl bezpečně přiřazen. Popisky zmiňují Svatováclavský festival, Rychvaldské kulturní jaro, adventní koncert místní ZUŠ a třímanuálové varhany z roku 1946.
- `urbanek-ccs-199` je prosincová strana se čtyřmi portréty z položek `060` až `063`. Popisky uvádějí Karla Vodičku, Gabriela Chrobáčka, Leonarda Bogumského a Janu Šilerovou a sekundární údaje o jejich úřadech a letech působení.
- `urbanek-ccs-200` je závěrečná textová strana. Děkuje Jaromíru Urbánkovi a dalším spolupracovníkům, obsahuje podpis čitelný jako `Jana Šilerová` a údaj `zpracováno: fa. Grafik Aja`.
- Závěrečné údaje částečně zpřesňují provenienci, ale neurčují jednoznačně vydavatele, tiskárnu, právní subjekt, úplné autorství ani držitele práv.
- Všech pět souborů má odlišné Git blob SHA, rozměr 2385 × 3354 pixelů a barevný režim CMYK.
- EXIF `Artist` a `XPAuthor` uvádějí u `196` řetězec `Corel Corporation`, u `197`, `198` a `200` řetězec `Marta` a u `199` řetězec `Pavla`; použitelné embedded datum chybí.
- Dávka nepřidala nové ID a rozšířila `URB-U-0073` o položky `196` až `200`.

Pracovní soubory dávky 40:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-40.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-40.yml`;
- `sources/index.d/urbanek-ccs-40.yml`;
- aktualizované `research/urbanek-archive/uncertainties/open-20.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 39;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 73.

`URB-U-0073` nyní zahrnuje všech patnáct obrazových stran kalendáře `186` až `200`. Částečně je doloženo poděkování Jaromíru Urbánkovi, podpis Jany Šilerové a produkční údaj `fa. Grafik Aja`; úplná tiráž, bibliografie, autorské role a práva zůstávají otevřené.

Kalendářový popisek, podpis, produkční údaj ani EXIF jméno samy neurčují úplné autorství, vydavatelskou odpovědnost nebo historickou správnost tvrzení.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- všech 200 JPEGů je zpracováno, zbývá jediný technický soubor;
- registr používá součty 39/31/3/73;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Obrazový obsah nové kolekce: `completed`.
- Následující položka: `10 Kalendář 2015/Thumbs.db`.
- Úkol: auditovat cache, porovnat náhledy s patnácti kalendářovými JPEGy a ověřit, zda neodkazuje na chybějící obrazové podklady.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
