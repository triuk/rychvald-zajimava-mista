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
| zpracováno | 367 | 17 | **384** |
| zbývá | 220 | 12 | **232** |
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
| Fotografie knihy Rychvald včera a dnes | 20 z 54 | 0 z 1 | 20 z 55 | probíhá |

Pilot tvoří prvních pět kolekcí a nepředstavuje celý archiv. Audity pilotních cache
prokázaly 11 chybějících plných originálů dochovaných pouze jako náhledy.

## Rozpracovaná kolekce „Fotografie knihy Rychvald včera a dnes“

Kolekce obsahuje 54 JPEGů a jeden technický soubor `Thumbs.db`.

### Dávka 04 – soubory `15.jpg` až `19.jpg`

- zpracováno a Git-ověřeno: **5 obrazových položek**;
- celkem v kolekci: **20 z 55 položek**;
- všechny soubory dávky jsou binárně odlišné a přesně odpovídají Git blobům;
- `15.jpg` zachycuje obytnou čtvrť s hlavní komunikací, několika podobně řešenými bytovými domy, rodinnou zástavbou, zahradami a poli;
- `16.jpg` zachycuje hlavní komunikaci, obytnou zástavbu, výraznou budovu s hranolovou věží, vysoký bytový dům a vodní plochu v pozadí;
- `17.jpg` zachycuje silniční křižovatku s dlouhou světlou budovou, užitkovými vozidly, rodinnými domy a zahradami;
- `18.jpg` zachycuje rozptýlenou obytnou zástavbu, několik komunikací a křižovatek, zahrady, louky a pole;
- `19.jpg` zachycuje průjezdní komunikaci, rozsáhlou odstavnou nebo parkovací plochu s mnoha automobily, provozní budovy, louky a lesní pás;
- přesné názvy komunikací, staveb, vodní plochy a funkce areálů nejsou bez mapového nebo dokumentárního podkladu přiřazeny;
- EXIF uvádí Sony DSC-WX7 a data od 30. června 2012 do 30. srpna 2013;
- `15.jpg` a `17.jpg` mají EXIF časy vzdálené 37 sekund a oba tag `PMB`, ale jednoznačný prostorový překryv nebyl zjištěn;
- `19.jpg` viditelně zachycuje denní světlo, přestože EXIF uvádí čas `23:39:36`; časová metadata proto nejsou spolehlivým dokladem okamžiku expozice;
- `18.jpg` obsahuje EXIF tag software `Picasa`;
- metadata nejsou nezávislým dokladem autorství, přesné lokace, použití v knize ani práv.

Existující otevřené ID `URB-U-0076` bylo rozšířeno o položky `016–020`. Samostatná
rešerše zůstává odložena do závěrečné fáze.

Pracovní soubory:

- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-overview.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-batch-04.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-inventory-04.csv`;
- `sources/index.d/urbanek-rychvald-vcera-dnes-04.yml`;
- `research/urbanek-archive/uncertainties/open-22.yml`.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| volné soubory přímo v kořeni | 6 | 0 | 6 |
| zbytek kolekce Fotografie knihy Rychvald včera a dnes | 34 | 1 | 35 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **220** | **12** | **232** |

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
- zpracovaný rozsah je 384 položek;
- zbývá 232 položek;
- kolekce „Fotografie knihy Rychvald včera a dnes“ je zpracována v rozsahu 20 z 55 položek;
- registr používá součty 41/32/3/76;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Úplný soupis aktuálního Git snapshotu: `completed`.
- Zbývající položky: **232**.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Aktuální kolekce: `Fotografie knihy Rychvald včera a dnes`.
- Dokončené dávky: 01 až 04, položky `001–020`.
- Následující dávka: `20.jpg`, `21.jpg`, `22.jpg`, `23.jpg`, `24.jpg`.
- Technický `Thumbs.db` bude auditován až po dokončení všech 54 obrazových souborů.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
