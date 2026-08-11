# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- PR #1 zůstává otevřený draft; sloučení nebylo vyžádáno.

## Stav indexace

| Stav | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| zpracováno | 532 | 24 | **556** |
| zbývá | 55 | 5 | **60** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **12 kolekcí**. Aktivní je kolekce `fotografie, které nebyl použité pro knihu ani kalendář`.

## fotografie, které nebyl použité pro knihu ani kalendář – dávka 04

Zpracovány byly `5048.jpg`, `7147.jpg`, `7185.JPG`, `73.jpg` a `74.tif`. Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Uvnitř dávky není přesná binární duplicita a žádný z pěti Git blob SHA nebyl nalezen v dosud indexovaných source záznamech.

`5048.jpg` zachycuje rozsáhlý zemní odkryv či prohlubeň s odkrytými svahy, hromadami materiálu a budovami na horním okraji; přesný účel, lokalita a datace nejsou určeny.

`7147.jpg` zobrazuje nízkou podlouhlou stavbu s krytým venkovním prostorem v prostředí vzrostlých stromů. EXIF uvádí Panasonic DMC-TZ3 a DateTimeOriginal `2010:10:28 15:22:55`; přesná funkce, název, vlastnictví a lokalita nejsou určeny.

`7185.JPG` zachycuje dvojici kamenných kruhových prvků s radiálními drážkami a středovými otvory. EXIF uvádí Panasonic DMC-TZ3 a DateTimeOriginal `2011:11:15 12:20:52`; přesná funkce, původ, stáří a vztah ke konkrétnímu provozu či stavbě nejsou určeny.

`73.jpg` a `74.tif` oba zachycují silně poškozené malované vrstvy na zdivu či omítce. `73.jpg` má EXIF Canon PowerShot G5 a DateTimeOriginal `2005:08:04 09:02:04`. `74.tif` je nekomprimovaný RGB TIFF 3463×3479 px s uloženým rozlišením 600 dpi a bez EXIF; pro vizuální kontrolu byla použita pouze lokální odvozená PNG kopie. Přesný vztah obou snímků, objekt, lokalita, námět, autorství a datace nejsou z podobnosti motivu ani z pořadí názvů dovozovány.

Nejistota `URB-U-0084` byla rozšířena na položky 001–020; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotografie, které nebyl použité pro knihu ani kalendář | 8 | 1 | 9 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **55** | **5** | **60** |

## Registr nejistot

- `open`: 49;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 84.

## Aktuální krok

Pátá dávka kolekce `fotografie, které nebyl použité pro knihu ani kalendář`:

- `75.tif`;
- `8205.jpg`;
- `8206.jpg`;
- `P1020271aaaaddd.jpg`;
- `ggg.tif`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
