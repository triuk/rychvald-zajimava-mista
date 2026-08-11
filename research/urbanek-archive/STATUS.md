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
| zpracováno | 517 | 24 | **541** |
| zbývá | 70 | 5 | **75** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **12 kolekcí**. Aktivní je kolekce `fotografie, které nebyl použité pro knihu ani kalendář`.

## fotografie, které nebyl použité pro knihu ani kalendář – dávka 01

Zpracovány byly `045.jpg`, `093.JPG`, `134.jpg`, `164.jpg` a `2011cIsenburgové z Birsteinu.jpg`. Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Mezi pěti položkami není přesná binární duplicita.

`045.jpg` je digitální reprodukce starší kreslené mapy s německými a latinskými popisky; bezpečně čitelné jsou mimo jiné `Mähren` a `Oder Fluvius`. Přesný název, autor a historická datace mapy nejsou z obrazu určeny. EXIF DateTimeOriginal `2010:12:13 05:58:19` je evidován jako technické metadata digitální reprodukce, nikoli jako datum mapy.

`093.JPG` zobrazuje vysokou věž stavby se sakrální architekturou, ciferníky hodin, štíhlou červenou střechou a křížem. EXIF uvádí Panasonic DMC-TZ3 a DateTimeOriginal `2010:10:27 15:22:13`; přesná stavba, denominace a lokalita nejsou určeny.

`134.jpg` zobrazuje hřbitov s centrálním kamenným křížem a několika návštěvníky. EXIF uvádí Panasonic DMC-FZ7 a DateTimeOriginal `2009:11:02 14:10:36`. `164.jpg` zachycuje početné venkovní shromáždění kolem hořící hranice z polen; EXIF uvádí výrobce Canon a DateTimeOriginal `2012:03:15 09:39:23`. Přesný hřbitov, monument, událost, místo ani osoby nejsou z obrazů samotných určeny.

`2011cIsenburgové z Birsteinu.jpg` je heraldické vyobrazení korunovaného štítu s modrým středovým polem a žlutým lvem. Část názvu souboru `Isenburgové z Birsteinu` je evidována pouze jako archivní atribuce; obraz sám bez dalšího pramene identitu držitele erbu nepotvrzuje. Tento JPEG neobsahuje EXIF. Žádný z pěti souborů dávky neobsahuje GPS údaje.

Pro kolekci vznikla nová nejistota `URB-U-0084`; systematické určování staveb, mapy, události, heraldického motivu a osob zůstává podle workflow odloženo do závěrečné fáze.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotografie, které nebyl použité pro knihu ani kalendář | 23 | 1 | 24 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **70** | **5** | **75** |

## Registr nejistot

- `open`: 49;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 84.

## Aktuální krok

Druhá dávka kolekce `fotografie, které nebyl použité pro knihu ani kalendář`:

- `2061.JPG`;
- `2063.JPG`;
- `2069.jpg`;
- `209.jpg`;
- `327a.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
