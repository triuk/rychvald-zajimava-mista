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
| zpracováno | 540 | 25 | **565** |
| zbývá | 47 | 4 | **51** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **13 kolekcí**. Kolekce `fotografie, které nebyl použité pro knihu ani kalendář` je po šesté dávce kompletně zpracována.

## fotografie, které nebyl použité pro knihu ani kalendář – dávka 06 a dokončení kolekce

Zpracovány byly `img010aa.jpg`, `img037.jpg`, `img724.jpg` a `Thumbs.db`. Tím je kolekce dokončena na **29 z 29 položek**: 28 obsahových souborů a jeden technický cache soubor. Všechny čtyři raw soubory z kanonické Drive složky přesně odpovídají velikostem a Git blobům v repozitáři.

`img010aa.jpg` je dekorativní koláž několika mužských portrétů. Bezpečně čitelné je motto `Bližnímu k ochraně, vlasti k oslavě!`; EXIF uvádí Canon a DateTimeOriginal `2013:06:28 09:55:14`. Přesná organizace, období původních portrétů a osoby nejsou určeny.

`img037.jpg` zobrazuje drobnou bílou sloupkovou sakrálně působící stavbu s červenou stříškou a křížovým prvkem u komunikace. Přesný typ, zasvěcení, lokalita, stáří a historie objektu nejsou určeny.

`img724.jpg` zachycuje skupinu osob postupujících po komunikaci v řadách. Přesný název a účel průvodu či události, organizace, lokalita, datum a osoby nejsou určeny.

`Thumbs.db` byl auditován jako OLE/Compound Document thumbnail cache. Odkazuje na všech 28 současných obsahových názvů kolekce a obsahuje 28 datových streamů s JPEG náhledy; všech 28 vložených JPEGů bylo přímo dekódováno. Cache je evidována jako odvozená technická položka, nikoli jako dalších 28 nezávislých historických obrazových pramenů.

Nejistota `URB-U-0084` nyní pokrývá všech 28 obsahových položek kolekce; technický `Thumbs.db` do historické nejistoty přidán nebyl. Nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| novinové články 1903 - 1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **47** | **4** | **51** |

## Registr nejistot

- `open`: 49;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 84.

## Aktuální krok

Zahájit kolekci `novinové články 1903 - 1925`:

- 16 obsahových souborů;
- 2 technické soubory;
- Drive složka `1OOe829hkaoHoNRs0HyajQROhknLD_aeg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
