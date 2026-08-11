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
| zpracováno | 511 | 22 | **533** |
| zbývá | 76 | 7 | **83** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **11 kolekcí**. Aktivní je kořenová část `fotodokument` mimo již dokončenou podsložku `den po dešti`.

## fotodokument – dávka 08

Zpracovány byly `img201.jpg`, `img202.jpg`, `img203.jpg`, `img206.jpg` a `img216.jpg`. Dávka obsahuje skupinu před větší budovou s koňským povozem, skupinu před dřevěnou budovou s pivním nápisem, detail odznaku či znaku se stuhami a dva snímky poškozených nebo rozebíraných mostově působících konstrukcí.

Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Mezi pěti položkami není přesná binární duplicita. Žádný z pěti JPEGů neobsahuje použitelná EXIF metadata.

Na `img202.jpg` je bezpečně čitelný nápis `Českobudějovické akciové pivo`. Je evidován jako viditelný text pramene; bez dalšího podkladu z něj není určována přesná provozovna, provozovatel, lokalita ani datum.

Na `img203.jpg` jsou bezpečně čitelné texty `ČESKÝ ČL. SPOLEK`, `VLASTIMIL` a `V RYCHVALDĚ 1893`. Zkratka `ČL.` není rozepisována a rok `1893` není bez dalšího pramene vykládán jako datum výroby předmětu ani datum pořízení fotografie.

Na `img201.jpg` není úzký nápis nad vstupem bezpečně čitelný. `img206.jpg` a `img216.jpg` zachycují mostově působící konstrukce se sutí či poškozením; jejich přesná identita, lokalita, důvod stavu, datace a vzájemný vztah nejsou z fotografií samotných určeny.

Nejistota `URB-U-0083` byla rozšířena na položky 001–040; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotodokument mimo `den po dešti` | 1 | 2 | 3 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **76** | **7** | **83** |

## Registr nejistot

- `open`: 48;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 83.

## Aktuální krok

Devátá a závěrečná dávka kořenové části `fotodokument`:

- `img343.jpg`;
- `Thumbs.db`;
- `ZbThumbnail.info`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
