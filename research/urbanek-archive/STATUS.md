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
| zpracováno | 537 | 24 | **561** |
| zbývá | 50 | 5 | **55** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **12 kolekcí**. Aktivní je kolekce `fotografie, které nebyl použité pro knihu ani kalendář`.

## fotografie, které nebyl použité pro knihu ani kalendář – dávka 05

Zpracovány byly `75.tif`, `8205.jpg`, `8206.jpg`, `P1020271aaaaddd.jpg` a `ggg.tif`. Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Uvnitř dávky není přesná binární duplicita a žádný z pěti Git blob SHA nebyl nalezen v dosud indexovaných source záznamech.

`75.tif` je nekomprimovaný RGB TIFF 3507×3507 px s uloženým rozlišením 600 dpi. Zachycuje silně poškozenou nástěnnou malbu s dochovanými motivy koňského povozu a architektury. Přesný námět, objekt, lokalita, autorství, datace a vztah k `73.jpg` a `74.tif` nejsou určeny.

Na `8205.jpg` jsou bezpečně čitelné `STRANA NÁR. SOCIALISTICKÁ`, `RYCHVALD` a rok `1929`. EXIF DateTimeOriginal je `2012:04:17 11:42:56`. Osoby, přesný organizační a událostní kontext a vztah k jiným snímkům se stejnou formulací nejsou z obrazu samotného určeny.

Na `8206.jpg` je bezpečně čitelné `1910–1930` a z horního organizačního nápisu pouze závěr `… V RYCHVALDĚ`; celý nápis není rekonstruován. EXIF DateTimeOriginal je `2012:04:23 10:06:03`. Viditelné datumové údaje jsou evidovány jako obsah pramene, nikoli automaticky jako technická data expozice.

`P1020271aaaaddd.jpg` zobrazuje architektonický detail s obloukovou nikou; z rytého nápisu je bezpečně čitelné pouze `ANNO`. EXIF uvádí Panasonic DMC-TZ3 a DateTimeOriginal `2012:11:20 12:05:04`. Další znaky nápisu nejsou rekonstruovány.

`ggg.tif` zobrazuje rozsáhlou podlouhlou vícepodlažní budovu s mnoha pravidelnými okny a vysokou valbovou střechou. Obsahuje obecný DateTime `2010:11:26 09:44:21` a software `Microsoft Windows Photo Gallery 6.0.6000.16386`, ale ne DateTimeOriginal; tato metadata nejsou používána jako historická datace budovy.

Nejistota `URB-U-0084` byla rozšířena na položky 001–025; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotografie, které nebyl použité pro knihu ani kalendář | 3 | 1 | 4 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **50** | **5** | **55** |

## Registr nejistot

- `open`: 49;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 84.

## Aktuální krok

Šestá a závěrečná dávka kolekce `fotografie, které nebyl použité pro knihu ani kalendář`:

- `img010aa.jpg`;
- `img037.jpg`;
- `img724.jpg`;
- `Thumbs.db`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
