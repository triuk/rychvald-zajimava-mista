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
| zpracováno | 481 | 22 | **503** |
| zbývá | 106 | 7 | **113** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **11 kolekcí**. Aktivní je kořenová část `fotodokument` mimo již dokončenou podsložku `den po dešti`.

## fotodokument – dávka 02

Zpracovány byly `img041.jpg` až `img045.jpg`. Dávka obsahuje tři exteriéry různých staveb, skupinový portrét před budovou a exteriér stavby se sakrální architekturou.

Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Mezi pěti položkami není přesná binární duplicita. Žádný z pěti JPEGů neobsahuje použitelná EXIF metadata.

Na `img044.jpg` je bezpečně čitelný banner **„VÝSTAVA 60 let školy V RYCHVALDĚ NA PODLESÍ“**. Spodní údaje banneru nejsou dostatečně čitelné pro spolehlivou dataci a nejsou rekonstruovány. Osoby na skupinovém snímku nejsou identifikovány. Na `img042.jpg` je fasádní znak a tabulka, ale její text není bezpečně čitelný.

Nejistota `URB-U-0083` byla rozšířena na položky 001–010 a nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotodokument mimo `den po dešti` | 31 | 2 | 33 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **106** | **7** | **113** |

## Registr nejistot

- `open`: 48;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 83.

## Aktuální krok

Třetí dávka kořenové části `fotodokument`:

- `img047.jpg`;
- `img048.jpg`;
- `img049.jpg`;
- `img050.jpg`;
- `img052.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
