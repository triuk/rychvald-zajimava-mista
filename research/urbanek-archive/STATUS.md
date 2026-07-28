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

Dokončeno je třicet čtyři dávek po pěti snímcích, tedy `urbanek-ccs-001` až `170`.

- zpracováno: **170 z 201 položek**;
- proti Git blob SHA ověřeno: **170 položek**;
- vizuálně klasifikováno: **170 položek**;
- zdrojově indexováno: **170 položek**;
- zbývá: **31 položek**.

### Zjištění dávky 34

Dávka 34 pokračuje v podsložce `7 Pohřeb biskupa br. Ferdinanda Stibora v říjnu 1956`.

- `urbanek-ccs-166` zachycuje bohatě zdobenou uzavřenou rakev nesenou několika muži z prostoru vstupu nebo sloupové předsíně mezi početným davem.
- `urbanek-ccs-167` zachycuje tři muže v dlouhých tmavých oděvech s řetězy a medailony; nejméně dva drží knihu, desky nebo jiný obdélný předmět.
- `urbanek-ccs-168` je širší uliční záběr několika podobně oděných osob; v pozadí jsou civilní přihlížející, kočárek, automobil a domy.
- `urbanek-ccs-169` zachycuje zdobenou rakev nesenou ulicí. Jde o jiný záběr stejné nebo bezprostředně navazující situace jako u `166`, nikoli binární duplikát.
- `urbanek-ccs-170` zachycuje delší uliční průvod s osobami v dlouhých tmavých oděvech, světlými znaky připomínajícími kalich nebo medailon a civilními účastníky.
- Všech pět souborů má odlišné Git blob SHA a žádný nemá použitelné embedded datum.
- Dávka nepřidala nové ID a rozšířila `URB-U-0071`.

Pracovní soubory dávky 34:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-34.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-34.yml`;
- `sources/index.d/urbanek-ccs-34.yml`;
- aktualizované `research/urbanek-archive/uncertainties/open-18.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 37;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 71.

`URB-U-0071` nyní zahrnuje položky `156` až `170`: portrét, vystavení a nesení rakve, osoby u rakve, výstup ze sboru, schodiště, uliční průvod, řetězy, medailony, znaky připomínající kalich, pásku s křížovitým znakem, prapory a další účastníky.

Archivní názvy jsou atribuce, nikoli nezávislé potvrzení. Oděv, řetěz, medailon, znak, pokrývka hlavy, páska na paži, držená kniha nebo postavení v průvodu samy neurčují identitu, úřad, organizaci nebo formální roli.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 170 zpracovaných a 31 zbývajících položek;
- registr používá součty 37/31/3/71;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-171` až `urbanek-ccs-175`.
- Očekávané názvy v téže podsložce: `16.jpg`, `17.jpg`, `18.jpg`, `19.jpg` a `20.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
