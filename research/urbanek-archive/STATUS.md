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
| zpracováno | 486 | 22 | **508** |
| zbývá | 101 | 7 | **108** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **11 kolekcí**. Aktivní je kořenová část `fotodokument` mimo již dokončenou podsložku `den po dešti`.

## fotodokument – dávka 03

Zpracovány byly `img047.jpg`, `img048.jpg`, `img049.jpg`, `img050.jpg` a `img052.jpg`. Dávka obsahuje obchodní budovu s česko-polskými nápisy, dva další neidentifikované stavební exteriéry, budovu označenou nápisem `KULTURNÍ DŮM` a detail bohatě zdobeného průjezdního portálu.

Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Mezi pěti položkami není přesná binární duplicita. Žádný z pěti JPEGů neobsahuje použitelná EXIF metadata.

Na `img047.jpg` jsou bezpečně čitelné `OVOCE-ZELENINA / OWOCE-JARZYNY`, `MLÉKÁRNA / MLECZARNIA`, české `POTRAVINY-LAHŮDKY` a číslo `70`. Nečitelná polská řádka pod pravým nápisem není rekonstruována.

Na `img050.jpg` je bezpečně čitelné `KULTURNÍ DŮM` a na jednom emblému písmena `ROH`. Nápis dokládá označení/funkci budovy jako kulturního domu v okamžiku zachycení; přesná lokalita, oficiální název instituce, provozovatel a datace nejsou z fotografie samotné určeny.

Nejistota `URB-U-0083` byla rozšířena na položky 001–015; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotodokument mimo `den po dešti` | 26 | 2 | 28 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **101** | **7** | **108** |

## Registr nejistot

- `open`: 48;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 83.

## Aktuální krok

Čtvrtá dávka kořenové části `fotodokument`:

- `img053.jpg`;
- `img054.jpg`;
- `img057.jpg`;
- `img058.jpg`;
- `img059.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
