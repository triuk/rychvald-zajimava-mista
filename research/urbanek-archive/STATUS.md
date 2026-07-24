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

Dokončeno je dvacet jedna dávek po pěti snímcích, tedy `urbanek-ccs-001` až `105`.

Dosavadní stav nové kolekce:

- zpracováno: **105 z 201 položek**;
- proti Git blob SHA ověřeno: **105 položek**;
- vizuálně klasifikováno: **105 položek**;
- zdrojově indexováno: **105 položek**;
- zbývá: **96 položek**.

### Zjištění dávky 21

Dávka 21 uzavírá Chrobáčkovu podsložku a otevírá podsložku `5 Kaple CČS na Ostravici`.

- `urbanek-ccs-101` zachycuje velkou skupinu před monumentálním vstupem. Je přesnou binární kopií `urbanek-ccs-045`; oba soubory mají blob SHA `d220a75fd2a69f43b2089c126488bbda84bea476`. Dvě archivní cesty proto představují jediný nezávislý obrazový záznam.
- `urbanek-ccs-102` zachycuje malou světlou stavbu na travnatém svahu s kamennou opěrnou zdí a vysokou úzkou věžovou konstrukcí. Označení kaple CČS na Ostravici a Winklerovy zvoničky pochází z archivního názvu.
- `urbanek-ccs-103` zachycuje oltář s motivem kalicha, svícny a kruhové figurální okno s profilem vousatého muže. Určení postavy jako Jana Husa pochází z archivního názvu.
- `urbanek-ccs-104` obsahuje čitelný vložený popisek: „Zástupce diec.rady br.Chrobáček vítá účastníky.“ Přepis textu je ověřen, identita muže a funkce uvedená v popisku nikoli.
- `urbanek-ccs-105` obsahuje čitelný vložený popisek: „Uvítání br.biskupa za děti“. Obraz zachycuje předání kytice mladou ženou nebo dívkou duchovnímu; identity, úřad a zastupování dětí nejsou samostatně ověřeny.
- Chrobáčkova podsložka má nyní zpracováno všech 25 souborů. Historické otázky v `URB-U-0062` zůstávají otevřené.
- Dávka vytvořila nové položky `URB-U-0069` pro kapli, zvoničku a figurální okno a `URB-U-0070` pro slavnost, Chrobáčka, biskupa a dětské uvítání.

Pracovní soubory dávky 21:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-21.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-21.yml`;
- `sources/index.d/urbanek-ccs-21.yml`;
- nový `research/urbanek-archive/uncertainties/open-17.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-12.yml`;
- doplněná vazba přesné kopie v dávce 09 a `sources/index.d/urbanek-ccs-09.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

Dávka 21 přidala `URB-U-0069` a `URB-U-0070` a rozšířila `URB-U-0062` o přesnou kopii položek `045/101`. Přesná binární kopie není druhým historickým svědectvím a čitelný vložený popisek potvrzuje své znění, nikoli automaticky osoby, úřady, událost nebo datum.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 105 zpracovaných a 96 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-106` až `urbanek-ccs-110`.
- Očekávané archivní názvy v podsložce `5 Kaple CČS na Ostravici`: `5.jpg`, `5a chatka na Ostravici.jpg`, `5 b Winklerova zvonička.jpg`, `5 c.jpg` a `5 d.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
