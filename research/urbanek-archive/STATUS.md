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
| zpracováno | 392 | 17 | **409** |
| zbývá | 195 | 12 | **207** |
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
| Fotografie knihy Rychvald včera a dnes | 45 z 54 | 0 z 1 | 45 z 55 | probíhá |

Pilot tvoří prvních pět kolekcí a nepředstavuje celý archiv. Audity pilotních cache
prokázaly 11 chybějících plných originálů dochovaných pouze jako náhledy.

## Rozpracovaná kolekce „Fotografie knihy Rychvald včera a dnes“

Kolekce obsahuje 54 JPEGů a jeden technický soubor `Thumbs.db`.

### Dávka 09 – soubory `40.jpg` až `44.jpg`

- zpracováno a Git-ověřeno: **5 obrazových položek**;
- celkem v kolekci: **45 z 55 položek**;
- všechny soubory dávky jsou binárně odlišné, neshodují se s dávkami 01 až 08 a přesně odpovídají Git blobům;
- `40.jpg` zachycuje rozsáhlou vodní plochu se zalesněnými ostrůvky nebo poloostrovy, pobřežní vegetací, mokřadními plochami a navazující rozptýlenou zástavbou;
- `41.jpg` zachycuje venkovní veřejnou akci s hustým davem, stánky, přístřešky, pódiem nebo platformou a vozidly; na sousední obchodní budově je čitelný nápis `Hruška`;
- `42.jpg` zachycuje hlavní komunikaci podél velké vodní plochy, přilehlý provozní nebo servisní areál, rodinné domy a železniční trať křížící komunikaci;
- `43.jpg` zachycuje širší sídelní centrum s komunikacemi, většími veřejnými nebo občanskými budovami, bytovými domy, kostelními stavbami a vodními plochami;
- `44.jpg` zachycuje kostelní stavbu s věží, zakřivenou komunikaci, křižovatku, rodinné domy a soustavu vodních ploch;
- přesné názvy lokalit, komunikací, vodních ploch, staveb, obchodní pobočky a veřejné akce nebyly bez mapového nebo dokumentárního podkladu přiřazeny;
- EXIF uvádí Sony DSC-WX7 a data od 10. listopadu 2012 do 5. října 2013;
- `40.jpg` a `42.jpg` mají shodné datum, oba uvádějí software `Picasa` a jejich EXIF časy se liší o devět sekund; to podporuje jednu fotografickou sekvenci, ale prostorový překryv nebyl spolehlivě potvrzen;
- `41.jpg` a dříve zpracované `33.jpg` mají EXIF časy vzdálené dvě minuty a 27 sekund, zachycují však odlišné areály a časová blízkost sama neprokazuje shodnou lokaci;
- `43.jpg` a `44.jpg` se zřetelně prostorově překrývají, mají odlišné kompozice a binární hashe a jejich EXIF časy se liší o šest minut a 52 sekund;
- oba překrývajícì se snímky `43.jpg` a `44.jpg` zachycují denní světlo navzdory hodinovým údajům kolem 23:40; hodinová složka proto není vedena jako spolehlivý čas expozice;
- `40.jpg` a `42.jpg` uvádějí software `Picasa`; `41.jpg`, `43.jpg` a `44.jpg` tag software nemají;
- nápis `Hruška` je veden jako text v obraze, nikoli jako důkaz přesné pobočky, lokace, názvu akce, použití v knize nebo autorství;
- metadata nejsou nezávislým dokladem autorství, přesné lokace, použití v knize ani práv.

Existující otevřené ID `URB-U-0076` bylo rozšířeno o položky `041–045`. Samostatná
rešerše zůstává odložena do závěrečné fáze.

Pracovní soubory:

- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-overview.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-batch-09.yml`;
- `research/urbanek-archive/collections/fotografie-knihy-rychvald-vcera-a-dnes-inventory-09.csv`;
- `sources/index.d/urbanek-rychvald-vcera-dnes-09.yml`;
- `research/urbanek-archive/uncertainties/open-22.yml`.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| volné soubory přímo v kořeni | 6 | 0 | 6 |
| zbytek kolekce Fotografie knihy Rychvald včera a dnes | 9 | 1 | 10 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **195** | **12** | **207** |

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
- zpracovaný rozsah je 409 položek;
- zbývá 207 položek;
- kolekce „Fotografie knihy Rychvald včera a dnes“ je zpracována v rozsahu 45 z 55 položek;
- registr používá součty 41/32/3/76;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Úplný soupis aktuálního Git snapshotu: `completed`.
- Zbývající položky: **207**.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Aktuální kolekce: `Fotografie knihy Rychvald včera a dnes`.
- Dokončené dávky: 01 až 09, položky `001–045`.
- Následující dávka: `45.jpg`, `46.jpg`, `47.jpg`, `48.jpg`, `49.jpg`.
- Technický `Thumbs.db` bude auditován až po dokončení všech 54 obrazových souborů.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
