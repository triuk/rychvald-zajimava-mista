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

Dokončeno je dvacet osm dávek po pěti snímcích, tedy `urbanek-ccs-001` až `140`.

- zpracováno: **140 z 201 položek**;
- proti Git blob SHA ověřeno: **140 položek**;
- vizuálně klasifikováno: **140 položek**;
- zdrojově indexováno: **140 položek**;
- zbývá: **61 položek**.

### Zjištění dávky 28

Dávka 28 pokračuje v podsložce `5 Kaple CČS na Ostravici`.

- `urbanek-ccs-136` zachycuje skupinu nejméně sedmi mužů v duchovních oděvech s knihami nebo zpěvníky; několik osob zřejmě zpívá nebo recituje.
- `urbanek-ccs-137` zachycuje početné venkovní shromáždění s knihami, dvě ženy ve zdobeném oděvu a ženu stojící zády se zdviženou paží. Gesto a otevřená ústa skupiny podporují interpretaci vedeného společného zpěvu, nikoli přesné určení sboru nebo skladby.
- `urbanek-ccs-138` zachycuje dva duchovní s knihami, dvě ženy ve zdobeném oděvu, děti, několik žerdí nebo praporů a muže v uniformě s čepicí.
- `urbanek-ccs-139` zachycuje duchovního s otevřenou knihou a ozdobným řetězem s medailonem motivu kalicha a kříže u oltáře. Je vizuálně podobný portrétu `120`, ale podobnost není dokumentární identifikací a jméno ani úřad se nepřiřazují.
- `urbanek-ccs-140` zachycuje velmi početný dav na zalesněném svahu, několik deštníků, knihy a fotografa s fotoaparátem na vyvýšeném místě.
- Žádný z pěti souborů neobsahuje vložený popisek ani použitelné embedded datum.
- Dávka nepřidala nové ID. Rozšířila `URB-U-0059` a `URB-U-0070`.

Pracovní soubory dávky 28:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-28.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-28.yml`;
- `sources/index.d/urbanek-ccs-28.yml`;
- rozšířené `research/urbanek-archive/uncertainties/open-11.yml` a `open-17.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

`URB-U-0059` nyní zahrnuje také vizuální paralelu mezi archivně popsaným portrétem `120` a projevem na položce `139`, výslovně bez obrazového přiřazení identity. `URB-U-0070` byla rozšířena o skupinu duchovních, vedený společný zpěv, krojované ženy, děti, prapory, samostatný projev a fotografa v davu.

Vizuální podobnost osob není identifikací. Gesto vedení zpěvu určuje pouze pravděpodobnou činnost, nikoli jméno vedoucí, sbor nebo skladbu.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 140 zpracovaných a 61 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-141` až `urbanek-ccs-145`.
- Očekávané názvy: poslední soubor podsložky kaple `30  Fotografie asi z r. 1947. Zájezd Rychvaldských  s biskup.jpg`, poté `1.jpg`, `2.jpg`, `3.jpg` a `4.jpg` v podsložce `6 Červen 1970. Pohřeb br. faráře ThDr Karla Vodičky.  Husova Č (1)`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
