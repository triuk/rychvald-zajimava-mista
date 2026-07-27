# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový kořen: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt bylo potvrzeno.
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Autoritativním pracovním úložištěm je Git repozitář.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`,
`uncertainties/index.yml` včetně odkazovaných shardů,
`reports/pilot-reconciliation.md` a kolekční přehledy v `collections/`.

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

Audity pilotních cache prokázaly **11 chybějících plných originálů**. Náhled v
`Thumbs.db` není náhradou plného originálu.

## Kolekce historie Církve československé

Kolekce `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`
obsahuje 200 JPEGů a jeden technický soubor `Thumbs.db`, celkem 201 položek.

Dokončeno je **25 dávek**, tedy `urbanek-ccs-001` až `125`.

- zpracováno: **125 z 201 položek**;
- proti Git blob SHA ověřeno: **125 položek**;
- vizuálně klasifikováno: **125 položek**;
- zdrojově indexováno: **125 položek**;
- zbývá: **76 položek**.

### Zjištění dávky 25

Dávka 25 pokračuje v podsložce `5 Kaple CČS na Ostravici`.

- `urbanek-ccs-121` zachycuje tři muže v duchovním oděvu, otevřenou knihu a výrazný řetěz nebo insignii s motivem kalicha. Vložený popisek zní **„Závěr bohoslužeb.“**
- `urbanek-ccs-122` zachycuje velmi početné venkovní shromáždění; mnoho účastníků drží otevřené knihy nebo zpěvníky. Vložený popisek zní **„Záběr z bohoslužeb.“**
- Archivní název `122` končí po formulaci `asi v r. 1945 nebo .`; chybějící druhý rok ani pokračování nebyly doplněny.
- `urbanek-ccs-123` až `125` zachycují průvod na venkovské silnici s několika vysokými prapory, ženami nebo dívkami ve zdobeném oděvu, dětmi, civilními účastníky a početnou skupinou duchovních.
- Texty, znaky a příslušnost praporů nejsou bezpečně čitelné. Označení „prapory sborů“ a „krojovaní“ pochází z archivních názvů.
- Sdílené prapory, trasa a archivní posloupnost podporují společný slavnostní okruh, nikoli přesné datum, organizace nebo identity.
- Dávka nepřidala nové ID. Rozšířila `URB-U-0070` a tematicky ji propojila s `URB-U-0059`; přítomnost osoby označené jako Horský nelze určit pouze podle obličeje, oděvu nebo insignie.

Pracovní soubory dávky 25:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-25.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-25.yml`;
- `sources/index.d/urbanek-ccs-25.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-17.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

Vložený popisek potvrzuje své znění, nikoli automaticky osobu, úřad, událost
nebo datum. Useknutý název se nedoplňuje odhadem. Sdílené prapory a trasa
mohou doložit obrazovou posloupnost, nikoli příslušnost praporů či účastníků.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 125 zpracovaných a 76 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-126` až `urbanek-ccs-130`.
- Očekávané názvy: `15.jpg`, `16 Před kapličkou.jpg`,
  `17 Vlevo Leonard Bugumský.jpg`, `18.jpg` a `19.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
