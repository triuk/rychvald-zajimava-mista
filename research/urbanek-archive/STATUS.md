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
| zpracováno | 377 | 17 | **394** |
| zbývá | 210 | 12 | **222** |
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
| Fotografie knihy Rychvald včera a dnes | 30 z 54 | 0 z 1 | 30 z 55 | probíhá |

Pilot tvoří prvních pět kolekcí a nepředstavuje celý archiv. Audity pilotních cache
prokázaly 11 chybějících plných originálů dochovaných pouze jako náhledy.

## Rozpracovaná kolekce „Fotografie knihy Rychvald včera a dnes“

Kolekce obsahuje 54 JPEGů a jeden technický soubor `Thumbs.db`.

### Dávka 06 – soubory `25.jpg` až `29.jpg`

- zpracováno a Git-ověřeno: **5 obrazových položek**;
- celkem v kolekci: **30 z 55 položek**;
- všechny soubory dávky jsou binárně odlišné, neshodují se s dávkami 01 až 05 a přesně odpovídají Git blobům;
- `25.jpg` zachycuje rozptýlenou obytnou zástavbu mezi zahradami, loukami a poli, s místní cestou v popředí a vzdáleným sídelním a průmyslovým panoramatem;
- `26.jpg` zachycuje rozptýlenou obytnou oblast s místními komunikacemi, rodinnými domy, zahradami, menšími obdělávanými plochami a travnatým pásem;
- `27.jpg` zachycuje velké zemědělské plochy oddělené pásy stromů, navazující obytnou zástavbu, místní komunikace a několik vodních ploch na okraji záběru;
- `28.jpg` zachycuje obytnou část podél průjezdní komunikace a vedlejších cest, sousedící s rozsáhlým lesním porostem;
- `29.jpg` zachycuje silniční křižovatku u pásu lesa, okolní rodinné domy, zahrady, louky a vzdálené průmyslové a obytné panorama;
- přesné názvy lokalit, komunikací, budov, vodních ploch a vzdálených panoramat nebyly bez mapového nebo dokumentárního podkladu přiřazeny;
- EXIF uvádí Sony DSC-WX7 a data 25. dubna a 28. září 2013;
- `26.jpg`, `28.jpg` a `29.jpg` mají EXIF časy v rozsahu dvě minuty a 41 sekund; pracovní zařazení do jedné fotografické relace je možné, ale jednoznačný prostorový překryv nebyl zjištěn;
- `25.jpg` a `27.jpg` mají shodné datum EXIF a časy vzdálené sedm minut a 50 sekund, což samo neprokazuje bezprostřední obrazovou sekvenci;
- pouze `28.jpg` obsahuje EXIF tag software `Picasa`;
- metadata nejsou nezávislým dokladem autorství, přesné lokace, použití v knize ani práv.

Existující otevřené ID `URB-U-0076` bylo rozšířeno o položky `026–030`. Samostatná
rešerše zůstává odložena do závěrečné fáze.

Pracovní soubory:

- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-overview.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-batch-06.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-inventory-06.csv`;
- `sources/index.d/urbanek-rychvald-vcera-dnes-06.yml`;
- `research/urbanek-archive/uncertainties/open-22.yml`.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| volné soubory přímo v kořeni | 6 | 0 | 6 |
| zbytek kolekce Fotografie knihy Rychvald včera a dnes | 24 | 1 | 25 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **210** | **12** | **222** |

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
- zpracovaný rozsah je 394 položek;
- zbývá 222 položek;
- kolekce „Fotografie knihy Rychvald včera a dnes“ je zpracována v rozsahu 30 z 55 položek;
- registr používá součty 41/32/3/76;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Úplný soupis aktuálního Git snapshotu: `completed`.
- Zbývající položky: **222**.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Aktuální kolekce: `Fotografie knihy Rychvald včera a dnes`.
- Dokončené dávky: 01 až 06, položky `001–030`.
- Následující dávka: `30.jpg`, `31.jpg`, `32.jpg`, `33.jpg`, `34.jpg`.
- Technický `Thumbs.db` bude auditován až po dokončení všech 54 obrazových souborů.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
