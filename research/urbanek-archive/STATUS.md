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
| zpracováno | 527 | 24 | **551** |
| zbývá | 60 | 5 | **65** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **12 kolekcí**. Aktivní je kolekce `fotografie, které nebyl použité pro knihu ani kalendář`.

## fotografie, které nebyl použité pro knihu ani kalendář – dávka 03

Zpracovány byly `333.jpg`, `367.jpg`, `369.jpg`, `5005a.jpg` a `5011b.jpg`. Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Uvnitř dávky není přesná binární duplicita a žádný z pěti Git blob SHA nebyl nalezen v dosud indexovaných source záznamech.

`333.jpg` zachycuje starší přízemní budovu se sedlovou střechou, plotem a stromy; přesná identita, funkce, vlastnictví, lokalita a datace nejsou určeny. `367.jpg` zobrazuje upravený obdélný venkovní areál s cestami, stromy a budovou v pozadí; přesný druh a účel areálu nejsou určeny.

`369.jpg` je široká tónovaná archivní reprodukce dřevěného domu se skupinou osob, zahradními či hospodářskými konstrukcemi, vodní plochou nebo zaplavenou prohlubní a malým větrným kolem. Obsahuje obecný EXIF `DateTime` `2012:05:30 10:40:00` a údaj `Adobe Photoshop 7.0 CE`, ale ne DateTimeOriginal; údaj proto není používán jako historická datace scény.

Na `5005a.jpg` je na tabuli bezpečně čitelné `Pětitřídní škola v Rychvaldě`. EXIF DateTimeOriginal je `2012:03:15 16:52:47`; jde o technická metadata digitálního souboru, nikoli automaticky o datum zobrazené historické scény. Osoby, přesná budova, ročník a okolnosti nejsou určeny.

Na `5011b.jpg` je nad skupinou bezpečně čitelný zápis `1928/29`. Je evidován jako viditelný údaj pramene; bez dalšího podkladu není automaticky považován za technicky ověřené datum expozice fotografie. Identity a role osob nejsou určeny.

Nejistota `URB-U-0084` byla rozšířena na položky 001–015; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotografie, které nebyl použité pro knihu ani kalendář | 13 | 1 | 14 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **60** | **5** | **65** |

## Registr nejistot

- `open`: 49;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 84.

## Aktuální krok

Čtvrtá dávka kolekce `fotografie, které nebyl použité pro knihu ani kalendář`:

- `5048.jpg`;
- `7147.jpg`;
- `7185.JPG`;
- `73.jpg`;
- `74.tif`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
