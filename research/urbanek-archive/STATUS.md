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
| dokončeno | 347 | 17 | **364** |
| zbývá | 240 | 12 | **252** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je sedm kolekcí:

| Kolekce | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvaldské větrné mlýny | 31 | 8 | 39 |
| Články z Českého slova | 37 | 2 | 39 |
| Ochotníci rychvald | 61 | 2 | 63 |
| fotodokument/den po dešti | 8 | 2 | 10 |
| Nálet na Ostravu 1944 | 7 | 1 | 8 |
| Historie Církve československé | 200 | 1 | 201 |
| Boj o náboženství v Rychvaldě | 3 | 1 | 4 |
| **Celkem** | **347** | **17** | **364** |

Pilot tvoří prvních pět kolekcí a nepředstavuje celý archiv. Audity pilotních cache
prokázaly 11 chybějících plných originálů dochovaných pouze jako náhledy.

## Dokončená kolekce „Boj o náboženství v Rychvaldě“

Kolekce obsahuje tři po sobě jdoucí fotografie rukopisných stran a jeden technický
soubor `Thumbs.db`.

- viditelný nadpis: **„Náboženský převrat v Rychvaldě“**;
- fotografie mají rozměr 2304 × 3072 px, režim RGB a odlišné Git blob SHA;
- EXIF uvádí fotoaparát Panasonic DMC-TZ3 a časy 4. června 2012 od 11:05:40 do 11:06:36;
- časy slouží k potvrzení pořadí fotografování, nikoli jako data historických událostí;
- rukopisný text pojednává o sporu o českou výuku náboženství, faráři Ferdinandu Němcovi,
  jednáních v letech 1919–1920 a příchodu Karla Vodičky;
- uvedená jména, data a události jsou evidována jako obsah rukopisného pramene,
  nikoli jako nezávisle ověřené historické skutečnosti.

Audit `Thumbs.db` zjistil přesně tři katalogové názvy a tři dekódovatelné náhledy.
Všechny odpovídají přítomným plným JPEGům; cache nedokládá žádný chybějící originál.

Nové otevřené ID `URB-U-0075` eviduje neznámý přesný svazek, autora, čísla stran
a úplnost fotografovaného oddílu. Samostatné řešení je odloženo do závěrečné fáze.

Pracovní soubory:

- `research/urbanek-archive/collections/boj-o-nabozenstvi-inventory.csv`;
- `research/urbanek-archive/collections/boj-o-nabozenstvi.yml`;
- `research/urbanek-archive/ocr/boj-o-nabozenstvi-visible-text.md`;
- `research/urbanek-archive/reports/boj-o-nabozenstvi-thumbs-audit.md`;
- `sources/index.d/urbanek-boj-o-nabozenstvi.yml`;
- `research/urbanek-archive/uncertainties/open-21.yml`.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| volné soubory přímo v kořeni | 6 | 0 | 6 |
| Fotografie knihy Rychvald včera a dnes | 54 | 1 | 55 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **240** | **12** | **252** |

Adresář `fotodokument` je částečně zpracovaný: podsložka `den po dešti` je dokončena,
ale 43 položek přímo v nadřazeném adresáři zůstává nezpracovaných.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 40;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 75.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`;
workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- dokončený rozsah je 364 položek;
- zbývá 252 položek;
- cache kolekce „Boj o náboženství“ dokládá 0 chybějících plných originálů;
- registr používá součty 40/32/3/75;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Úplný soupis aktuálního Git snapshotu: `completed`.
- Zbývající položky: **252**.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Další kolekce: `Fotografie knihy Rychvald včera a dnes`.
- Rozsah: 54 obrazových souborů + 1 technický soubor = 55 položek.
- Zpracování bude rozděleno do omezených obrazových dávek a uzavřeno auditem technické cache.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
