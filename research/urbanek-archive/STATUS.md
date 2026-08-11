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
| zpracováno | 506 | 22 | **528** |
| zbývá | 81 | 7 | **88** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **11 kolekcí**. Aktivní je kořenová část `fotodokument` mimo již dokončenou podsložku `den po dešti`.

## fotodokument – dávka 07

Zpracovány byly `img176.jpg`, `img178.jpg`, `img196.jpg`, `img197.jpg` a `img200.jpg`. Dávka obsahuje dva starší domovní exteriéry, skupinový snímek s organizačním praporem, skupinu před školní budovou a skupinu před budovou s částečným německým nápisem.

Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Mezi pěti položkami není přesná binární duplicita. Žádný z pěti JPEGů neobsahuje použitelná EXIF metadata.

Na `img178.jpg` jsou bezpečně čitelné texty `STRANA NÁR. SOCIALISTICKÁ`, `RYCHVALD` a rok `1929`. Rok je evidován jako viditelný údaj pramene; bez dalšího podkladu není automaticky ztotožněn s datem expozice fotografie. Osoby nejsou identifikovány.

Na `img197.jpg` je bezpečně čitelný nápis `NÁRODNÍ ŠKOLA`, který dokládá dobové označení školní funkce budovy, ne však přesnou školu či lokalitu. Na `img200.jpg` je z oříznutého německého nápisu bezpečně čitelné slovo `Gastwirtschaft`; předcházející část názvu není rekonstruována. Uniformní oděv jedné osoby není používán k určení složky, hodnosti ani příslušnosti.

Nejistota `URB-U-0083` byla rozšířena na položky 001–035; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotodokument mimo `den po dešti` | 6 | 2 | 8 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **81** | **7** | **88** |

## Registr nejistot

- `open`: 48;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 83.

## Aktuální krok

Osmá dávka kořenové části `fotodokument`:

- `img201.jpg`;
- `img202.jpg`;
- `img203.jpg`;
- `img206.jpg`;
- `img216.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
