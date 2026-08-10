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
| zpracováno | 471 | 22 | **493** |
| zbývá | 116 | 7 | **123** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **11 kolekcí**. Kolekce `Rychvald` je dokončena v rozsahu **33 z 33 položek**.

## Rychvald – dokončení kolekce

V sedmi obsahových dávkách bylo zpracováno všech 31 JPEGů. Následný technický audit uzavřel také `Thumbs.db` a `ZbThumbnail.info`.

`Thumbs.db` je CFB/OLE cache s katalogem verze 7. Obsahuje 31 pojmenovaných náhledů plných JPEGů a jednu položku náhledu složky. `ZbThumbnail.info` se signaturou `zbex` obsahuje 31 JPEG náhledů a názvy všech 31 plných obrazových souborů. Ani jedna cache nedokládá další nebo chybějící plný originál.

V obou cache se projevuje známá binární duplicita položek 002 a 007 (`Budova úřadu 005.jpg` a `Kopie - Budova úřadu 005.jpg`). Nejde o nový samostatný obrazový pramen.

Technické soubory byly ověřeny proti Drive i Git blobům. Podrobný audit je v `research/urbanek-archive/reports/rychvald-technical-audit.md`.

Nejistota `URB-U-0082` zůstává otevřená pro provenienci, autorství, lokalizaci, původní účel sady a práva; technický audit nevytvořil novou nejistotu.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **116** | **7** | **123** |

## Registr nejistot

- `open`: 47;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 82.

## Aktuální krok

Další skupinou je `fotodokument` mimo již dokončenou podsložku `den po dešti`. První dávku tvoří v deterministickém pořadí:

- `img036.jpg`;
- `img037.jpg`;
- `img038.jpg`;
- `img039.jpg`;
- `img040.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
