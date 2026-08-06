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
| zpracováno | 401 | 18 | **419** |
| zbývá | 186 | 11 | **197** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je osm kolekcí:

| Kolekce | Obsahové | Technické | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | dokončeno |
| Články z Českého slova | 37 | 2 | 39 | dokončeno |
| Ochotníci rychvald | 61 | 2 | 63 | dokončeno |
| fotodokument/den po dešti | 8 | 2 | 10 | dokončeno |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | dokončeno |
| Historie Církve československé | 200 | 1 | 201 | dokončeno |
| Boj o náboženství v Rychvaldě | 3 | 1 | 4 | dokončeno |
| Fotografie knihy Rychvald včera a dnes | 54 | 1 | 55 | dokončeno |

Pilot tvoří prvních pět kolekcí a nepředstavuje celý archiv. Audity pilotních cache
prokázaly 11 chybějících plných originálů dochovaných pouze jako náhledy.

## Dokončená kolekce „Fotografie knihy Rychvald včera a dnes“

Kolekce obsahuje 54 JPEGů a jeden technický soubor `Thumbs.db`; všech **55 z 55 položek** je zpracováno.

### Audit `Thumbs.db`

- Drive originál a Git soubor mají shodnou velikost **203 264 B** a shodný Git blob SHA `994155fade2d4f2472cb8b77976262b767ab38f4`;
- SHA-256 souboru je `86a9e6592075496d6302389198300e09623f104c3a74a593a93ffca2107d8ff8`;
- jde o platný CFB/OLE dokument s 512B sektory a 64B minisektory;
- katalog verze 7 obsahuje přesně **54 obrazových záznamů** a deklaruje cílový náhled 96 × 96 px;
- sada katalogových názvů přesně odpovídá `0 titulní stránka.jpg` a `1.jpg`–`53.jpg`;
- cache obsahuje přesně **54 datových streamů** s platnými JPEG náhledy o šířce 96 px;
- žádný stream nechybí, nepřebývá ani není binárně totožný s jiným náhledem;
- pro lokálně dostupných 34 originálů `20.jpg`–`53.jpg` byla navíc potvrzena jednoznačná obrazová shoda se stejně pojmenovaným náhledem;
- názvy nebo náhledy bez odpovídajícího plného souboru: **0**;
- chybějící plné originály doložené touto cache: **0**;
- další samostatný obrazový obsah: **nezjištěn**.

Katalogové časy a čas kořenového CFB záznamu jsou metadata cache, nikoli datace fotografovaných míst nebo historických událostí.

Audit je uložen v `research/urbanek-archive/reports/fotografie-knihy-rychvald-vcera-a-dnes-thumbs-audit.md`.
Otevřená provenienční otázka `URB-U-0076` zůstává beze změny: cache potvrzuje úplnost této sady souborů, nikoli autora, práva ani přesný vztah ke knize.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| volné soubory přímo v kořeni | 6 | 0 | 6 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **186** | **11** | **197** |

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
- zpracovaný rozsah je 419 položek;
- zbývá 197 položek;
- kolekce „Fotografie knihy Rychvald včera a dnes“ je dokončena v rozsahu 55 z 55 položek;
- cache nedokládá žádný chybějící plný originál;
- registr používá součty 41/32/3/76;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Úplný soupis aktuálního Git snapshotu: `completed`.
- Zbývající položky: **197**.
- Revize otevřených nejistot: `deferred_until_full_archive_index_complete`.
- Poslední dokončená kolekce: `Fotografie knihy Rychvald včera a dnes`.
- Následující skupina: volné soubory přímo v kořeni archivu.
- Následující dávka: `19.jpg`, `20Hlavička 27.10.1938.jpg`, `21zpráva 28.10.1938.jpg`, `9 X 1938 przed zajęciem Rychvaldu.png`, `IMG_0117 seznam bojůvkařů.jpg`.
- Po této dávce zůstane ve skupině `img237 německý četník.jpg`.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
