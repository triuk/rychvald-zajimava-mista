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
| zpracováno | 496 | 22 | **518** |
| zbývá | 91 | 7 | **98** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **11 kolekcí**. Aktivní je kořenová část `fotodokument` mimo již dokončenou podsložku `den po dešti`.

## fotodokument – dávka 05

Zpracovány byly `img060.jpg` až `img064.jpg`. Dávka obsahuje venkovský stavební celek ve svahu, nízkou utilitárně působící stavbu, podlouhlou starší budovu a dva širší krajinné pohledy na rozptýlenou zástavbu.

Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Mezi pěti položkami není přesná binární duplicita. Žádný z pěti JPEGů neobsahuje použitelná EXIF metadata.

U `img061.jpg` je evidován pouze utilitární vzhled nízké stavby, nikoli konkrétní provozní funkce. Na `img063.jpg` je výrazná lineární trasa se sloupy, ale bez dalšího podkladu není přiřazena konkrétnímu druhu infrastruktury. Přesné lokality a historická datace nejsou z krajinného nebo architektonického vzhledu dovozovány.

Nejistota `URB-U-0083` byla rozšířena na položky 001–025; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotodokument mimo `den po dešti` | 16 | 2 | 18 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **91** | **7** | **98** |

## Registr nejistot

- `open`: 48;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 83.

## Aktuální krok

Šestá dávka kořenové části `fotodokument`:

- `img065.jpg`;
- `img066.jpg`;
- `img067.jpg`;
- `img068.jpg`;
- `img070.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
