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
- stav: `completed`.

Dokončeno je čtyřicet obrazových dávek `urbanek-ccs-001` až `200` a samostatný audit technického souboru.

- zpracováno: **201 z 201 položek**;
- proti Git blob SHA ověřeno: **201 položek**;
- vizuálně klasifikováno: **200 obrazových položek**;
- zdrojově indexováno: **201 položek**;
- zbývá: **0 položek**.

### Revize nejistot 01 – zvony Husova sboru

- `URB-U-0074` bylo uzavřeno pro úzce vymezenou otázku materiálu hlavních věžových zvonů a válečné rekvizice.
- Historický souhrn zveřejněný CČSH v roce 2025 uvádí, že zvony nebyly zabaveny pro vojenské účely, protože jsou ocelové, nikoli ze zvonoviny.
- Kalendář 2015 rovněž označuje dva zvony ve věži jako ocelové. Jeho tvrzení, že reliéf `1920` je rokem výroby, zůstává sekundárním popiskem bez nezávislého potvrzení.
- `URB-U-0041` zůstává otevřené pro zvonaře nebo slévárnu, úplné nápisy, původ, přesné datace, jména a rozmístění zvonů, vztah všech tří zvonů k jedné soupravě a pozdější opravy.
- `URB-U-0042` zůstává otevřené pro historii ručního ovládání, elektrifikace a technických přestaveb.
- Vyhledávání příjmení Kakalová ve zpravodaji z července 1998 přineslo pouze záznam životního jubilea bez doložitelné vazby na Kakalův mlýn; tato shoda nebyla použita jako důkaz.

Pracovní soubory revize:

- `research/urbanek-archive/verifications/urb-u-0074-rychvald-bells-material-and-wartime-requisition.md`;
- `research/urbanek-archive/uncertainties/closed-21.yml`;
- aktualizované `research/urbanek-archive/uncertainties/open-06.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 39;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 74.

Uzavření `URB-U-0074` je úmyslně úzké. Dva shodné místní sekundární zdroje umožňují bezpečnou atribuovanou formulaci o ocelových hlavních zvonech a jejich válečné nerekvizici, nikoli širší technickou nebo provenienční rekonstrukci.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- kolekce CČS je zpracována v rozsahu 201 z 201 položek;
- registr používá součty 39/32/3/74;
- pilotní údaj o 11 chybějících plných originálech zůstává beze změny a netýká se kolekce CČS;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Pracovní pořadí

Projekt je nově rozdělen do dvou navazujících fází:

1. **Úplná inventarizace a indexace archivu.** Nejprve se projde celý zdrojový kořen `sources/osobni-archiv-jaromira-urbanka/`, určí se všechny dosud nezpracované kolekce a jejich položky se inventarizují, Git-ověří, základně klasifikují a zdrojově indexují.
2. **Závěrečná revize nejistot.** Teprve po dokončení úplného indexu se všechna otevřená ID znovu seřadí podle významu a dostupnosti pramenů a začne jejich systematické řešení.

Během indexace se nejistoty neztrácejí: každá materiální nejasnost dostane nebo zachová stabilní ID, vazbu na zdrojové položky, stručný popis a případnou prioritu. Samostatná rešerše a uzavírání se odkládají do druhé fáze.

Výjimkou jsou pouze situace, kdy je dílčí ověření nutné pro správnou inventarizaci nebo ochranu provenience, například rozlišení technického souboru, přesného binárního duplikátu, skutečně chybějícího originálu nebo správného přiřazení položky ke kolekci.

## Aktuální krok

- Pilot: `completed`, ale nepředstavuje celý archiv.
- Kolekce historie CČS: `completed`.
- Známý dokončený rozsah: **6 kolekcí a 360 položek**.
- Úplný rozsah zdrojového kořene dosud není autoritativně zinventarizován.
- Aktivní fáze: `full_archive_indexing`.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Následuje úplný soupis zdrojového kořene a výběr další dosud neindexované kolekce.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
