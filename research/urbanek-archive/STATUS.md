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

- PR: [#1 – Index and classify Jaromír Urbánek archive (in progress)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

## Úplný soupis zdrojového kořene

Pro aktuální Git snapshot je pod `sources/osobni-archiv-jaromira-urbanka/` evidováno:

- 13 adresářů nejvyšší úrovně;
- 6 volných souborů přímo v kořeni;
- **587 obsahových souborů**;
- **29 technických souborů**;
- **616 položek celkem**.

Soupis je autoritativní pro soubory přítomné na pracovní větvi. Neprokazuje,
že mimo Git neexistují další dosud nepřidané archivní soubory.

Podrobný přehled: `research/urbanek-archive/archive-root-inventory.yml`.

## Stav indexace

| Stav | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| zpracováno | 401 | 17 | **418** |
| zbývá | 186 | 12 | **198** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je sedm kolekcí; osmá je rozpracovaná:

| Kolekce | Obsahové | Technické | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | dokončeno |
| Články z Českého slova | 37 | 2 | 39 | dokončeno |
| Ochotníci rychvald | 61 | 2 | 63 | dokončeno |
| fotodokument/den po dešti | 8 | 2 | 10 | dokončeno |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | dokončeno |
| Historie Církve československé | 200 | 1 | 201 | dokončeno |
| Boj o náboženství v Rychvaldě | 3 | 1 | 4 | dokončeno |
| Fotografie knihy Rychvald včera a dnes | 54 z 54 | 0 z 1 | 54 z 55 | probíhá |

Pilot tvoří prvních pět kolekcí a nepředstavuje celý archiv. Audity pilotních cache
prokázaly 11 chybějících plných originálů dochovaných pouze jako náhledy.

## Rozpracovaná kolekce „Fotografie knihy Rychvald včera a dnes“

Kolekce obsahuje 54 JPEGů a jeden technický soubor `Thumbs.db`.

### Dávka 11 – soubory `50.jpg` až `53.jpg`

- zpracovány a Git-ověřeny: **4 obrazové položky**;
- obrazová část kolekce je dokončena: **54 z 54 JPEGů**;
- celkem v kolekci je zpracováno **54 z 55 položek**;
- všechny soubory dávky jsou binárně odlišné, neshodují se s dávkami 01 až 10 a přesně odpovídají Git blobům;
- `50.jpg` zachycuje rozsáhlý zemědělský nebo provozní areál s dlouhými halami, otevřenými přístřešky, manipulačními plochami a sklady, obklopený sklizenými poli a lesem;
- `51.jpg` zachycuje nízkou budovu u hlavní komunikace a boční ulice, s venkovním posezením, parkovací plochou a upravenou zahradou;
- `52.jpg` zachycuje rozsáhlou vícekřídlou budovu kolem otevřeného dvora, parkovací a příjezdové plochy a upravenou zahradu mezi poli;
- `53.jpg` zachycuje sídelní centrum s kostelní věží a vícepodlažními budovami za soustavou vodních ploch;
- přesné názvy lokalit, komunikací, vodních ploch, staveb a jejich funkce nebyly bez mapového nebo dokumentárního podkladu přiřazeny;
- EXIF uvádí Sony DSC-WX7 a data od 24. března 2012 do 30. srpna 2013;
- `50.jpg` a dříve zpracované `32.jpg` mají EXIF časy vzdálené 23 sekund a sdílejí stejné sklizené pole s balíky; jde o potvrzený prostorový překryv jedné fotografické sekvence;
- `53.jpg` se zřetelně prostorově překrývá s `43.jpg` a `44.jpg` v oblasti sídelního centra, kostelní věže a soustavy vodních ploch; fotografie mají odlišná data EXIF, kompozice a binární hashe;
- `52.jpg` a dříve zpracované `30.jpg` mají stejné datum EXIF a časy vzdálené 11 minut a 20 sekund, ale oba snímky zachycují denní světlo navzdory pozdně večerním hodinám a prostorový překryv nebyl potvrzen;
- software `Picasa` uvádí pouze `52.jpg`; ostatní tři soubory dávky tag software nemají;
- metadata nejsou nezávislým dokladem autorství, přesné lokace, použití v knize ani práv.

Existující otevřené ID `URB-U-0076` bylo rozšířeno o položky `051–054`. Samostatná
rešerše zůstává odložena do závěrečné fáze.

Pracovní soubory:

- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-overview.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-batch-11.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-inventory-11.csv`;
- `sources/index.d/urbanek-rychvald-vcera-dnes-11.yml`;
- `research/urbanek-archive/uncertainties/open-22.yml`.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| volné soubory přímo v kořeni | 6 | 0 | 6 |
| technický `Thumbs.db` kolekce Fotografie knihy Rychvald včera a dnes | 0 | 1 | 1 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **186** | **12** | **198** |

Adresář `fotodokument` je částečně zpracovaný: podsložka `den po dešti` je dokončena,
ale 43 položek přímo v nadřazeném adresáři zůstává nezpracovaných.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 41;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 76.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`;
workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 418 položek;
- zbývá 198 položek;
- obrazová část kolekce „Fotografie knihy Rychvald včera a dnes“ je zpracována v rozsahu 54 z 54 JPEGů;
- v kolekci zbývá pouze technický soubor `Thumbs.db`;
- registr používá součty 41/32/3/76;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Úplný soupis aktuálního Git snapshotu: `completed`.
- Zbývající položky: **198**.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Aktuální kolekce: `Fotografie knihy Rychvald včera a dnes`.
- Dokončené obrazové dávky: 01 až 11, položky `001–054`.
- Následující krok: technický audit souboru `Thumbs.db` a uzavření kolekce.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
