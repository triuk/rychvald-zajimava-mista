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

Pro aktuální Git snapshot byl dokončen úplný soupis cest pod
`sources/osobni-archiv-jaromira-urbanka/`.

- 13 adresářů nejvyšší úrovně;
- 6 volných souborů přímo v kořeni;
- **587 obsahových souborů**;
- **29 technických souborů**;
- **616 položek celkem**.

Soupis je autoritativní pro soubory přítomné na aktuální pracovní větvi. Neprokazuje,
že mimo Git neexistují další dosud nepřidané archivní soubory.

Podrobný přehled:

- `research/urbanek-archive/archive-root-inventory.yml`

## Stav indexace

| Stav | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| dokončeno | 344 | 16 | **360** |
| zbývá | 243 | 13 | **256** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je šest kolekcí:

| Kolekce | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvaldské větrné mlýny | 31 | 8 | 39 |
| Články z Českého slova | 37 | 2 | 39 |
| Ochotníci rychvald | 61 | 2 | 63 |
| fotodokument/den po dešti | 8 | 2 | 10 |
| Nálet na Ostravu 1944 | 7 | 1 | 8 |
| Historie Církve československé | 200 | 1 | 201 |
| **Celkem** | **344** | **16** | **360** |

Pilot tvoří prvních pět kolekcí a nepředstavuje celý archiv. Audity pilotních cache
prokázaly 11 chybějících plných originálů dochovaných pouze jako náhledy.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| volné soubory přímo v kořeni | 6 | 0 | 6 |
| Boj o náboženství v Rychvaldě | 3 | 1 | 4 |
| Fotografie knihy Rychvald včera a dnes | 54 | 1 | 55 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **243** | **13** | **256** |

Adresář `fotodokument` je tedy částečně zpracovaný: podsložka `den po dešti`
je dokončena, ale 43 položek přímo v nadřazeném adresáři zůstává nezpracovaných.

## Kolekce historie Církve československé

Kolekce `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`
je dokončena v rozsahu 201 z 201 položek:

- 200 obrazů vizuálně klasifikováno;
- 201 položek Git-ověřeno a zdrojově indexováno;
- dokončeno 40 obrazových dávek;
- audit `Thumbs.db` nedoložil žádný chybějící plný originál.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 39;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 74.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají
`open`; workflow odložení je nepřevádí do stavu `deferred`.

Během indexace se provádí jen úzké ověření nutné pro správné zařazení souboru,
rozlišení technického souboru, binárního duplikátu, chybějícího originálu nebo
ochranu provenience.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- dokončený rozsah je 360 položek;
- zbývá 256 položek;
- pilot a kolekce CČS jsou vedeny odděleně;
- registr používá součty 39/32/3/74;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Úplný soupis aktuálního Git snapshotu: `completed`.
- Zbývající položky: **256**.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Další kolekce: `Boj o náboženství v Rychvaldě`.
- Rozsah další kolekce: 3 obrazové soubory + 1 `Thumbs.db` = 4 položky.
- Důvod výběru: první souvislá nezpracovaná složka ve stabilním pořadí po již dokončené číselné kolekci CČS a vhodný malý rozsah pro ověření nového workflow.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
