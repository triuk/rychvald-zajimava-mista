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
| zpracováno | 512 | 24 | **536** |
| zbývá | 75 | 5 | **80** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **12 kolekcí**. Kořenová část `fotodokument` mimo již dříve dokončenou podsložku `den po dešti` je po dávce 09 kompletně zpracována.

## fotodokument – dávka 09 a dokončení kolekce

Zpracovány byly `img343.jpg`, `Thumbs.db` a `ZbThumbnail.info`. Tím je kořenová část `fotodokument` dokončena na **43 z 43 položek**: 41 obsahových JPEGů a dva technické cache soubory.

Všechny tři raw soubory z kanonické Drive složky přesně odpovídají velikostem a Git blobům v repozitáři.

`img343.jpg` zachycuje viditelně poškozenou či zřícenou mostově působící konstrukci nad menším vodním tokem nebo příkopem. Přesná identita, lokalita, příčina stavu, datace a vztah k `img206.jpg` nebo `img216.jpg` nejsou z fotografie samotné určeny. JPEG neobsahuje použitelná EXIF metadata.

`Thumbs.db` byl ověřen jako technická OLE/Compound Document cache s odkazy na názvy archivních JPEGů a s vloženými JPEGovými obrazovými daty. Obsahuje 54 různých odkazů `imgNNN.jpg`: 39 odpovídá aktuálním kořenovým JPEGům a 15 názvů v aktuálním kořenovém Git snapshotu není. Tento rozdíl se neeviduje jako důkaz přesunu či smazání souborů.

`ZbThumbnail.info` je technická binární cache s 41 různými odkazy `imgNNN.jpg`, které přesně odpovídají aktuálním 41 kořenovým JPEGům, a se 41 přímo dekódovatelnými JPEGovými obrazovými proudy. Oba cache soubory jsou evidovány jako odvozené technické položky, nikoli jako další nezávislé historické obrazové prameny.

Nejistota `URB-U-0083` byla rozšířena na obsahovou položku 041; technické položky 042–043 do historické nejistoty přidány nebyly. Nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **75** | **5** | **80** |

## Registr nejistot

- `open`: 48;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 83.

## Aktuální krok

Zahájit kolekci `fotografie, které nebyl použité pro knihu ani kalendář`:

- 28 obsahových souborů;
- 1 technický soubor;
- Drive složka `17EbJ7_kXjp1NJA4FOZYKQUYbwBdd2s2g`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
