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
| zpracováno | 362 | 17 | **379** |
| zbývá | 225 | 12 | **237** |
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
| Fotografie knihy Rychvald včera a dnes | 15 z 54 | 0 z 1 | 15 z 55 | probíhá |

Pilot tvoří prvních pět kolekcí a nepředstavuje celý archiv. Audity pilotních cache
prokázaly 11 chybějících plných originálů dochovaných pouze jako náhledy.

## Rozpracovaná kolekce „Fotografie knihy Rychvald včera a dnes“

Kolekce obsahuje 54 JPEGů a jeden technický soubor `Thumbs.db`.

### Dávka 03 – soubory `10.jpg` až `14.jpg`

- zpracováno a Git-ověřeno: **5 obrazových položek**;
- celkem v kolekci: **15 z 55 položek**;
- všechny soubory dávky jsou binárně odlišné a přesně odpovídají Git blobům;
- `10.jpg` zachycuje provozní areál s několika obdélnými nádržemi, větší vodní plochou, silnicemi a železniční tratí;
- `11.jpg` zachycuje rozsáhlý dvůrový komplex, řady menších staveb, komunikaci, samostatné domy a bytový dům;
- `12.jpg` a `13.jpg` jsou překrývající se pohledy na vodní plochy oddělené železničním pásem a okolní sídelní krajinu;
- `14.jpg` zachycuje provozní haly, zpevněné plochy, obytnou nebo zahrádkářskou zástavbu, zeleň a vodní plochu;
- přesné názvy areálů, komunikací, železničního úseku a vodních ploch nejsou bez mapového nebo dokumentárního podkladu přiřazeny;
- EXIF uvádí Sony DSC-WX7 a data od 7. srpna do 28. září 2013;
- `12.jpg` a `13.jpg` mají časy vzdálené pět sekund a prostorově se překrývají, což podporuje jejich pracovní zařazení do jedné fotografické sekvence;
- soubory `10.jpg`, `11.jpg` a `13.jpg` obsahují EXIF tag software `Picasa`;
- metadata nejsou nezávislým dokladem autorství, přesné lokace, použití v knize ani práv.

Existující otevřené ID `URB-U-0076` bylo rozšířeno o položky `011–015`. Samostatná
rešerše zůstává odložena do závěrečné fáze.

Pracovní soubory:

- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-overview.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-batch-03.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-inventory-03.csv`;
- `sources/index.d/urbanek-rychvald-vcera-dnes-03.yml`;
- `research/urbanek-archive/uncertainties/open-22.yml`.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| volné soubory přímo v kořeni | 6 | 0 | 6 |
| zbytek kolekce Fotografie knihy Rychvald včera a dnes | 39 | 1 | 40 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **225** | **12** | **237** |

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
- zpracovaný rozsah je 379 položek;
- zbývá 237 položek;
- kolekce „Fotografie knihy Rychvald včera a dnes“ je zpracována v rozsahu 15 z 55 položek;
- registr používá součty 41/32/3/76;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Úplný soupis aktuálního Git snapshotu: `completed`.
- Zbývající položky: **237**.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Aktuální kolekce: `Fotografie knihy Rychvald včera a dnes`.
- Dokončené dávky: 01 až 03, položky `001–015`.
- Následující dávka: `15.jpg`, `16.jpg`, `17.jpg`, `18.jpg`, `19.jpg`.
- Technický `Thumbs.db` bude auditován až po dokončení všech 54 obrazových souborů.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
