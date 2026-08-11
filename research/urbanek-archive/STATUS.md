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
| zpracováno | 522 | 24 | **546** |
| zbývá | 65 | 5 | **70** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **12 kolekcí**. Aktivní je kolekce `fotografie, které nebyl použité pro knihu ani kalendář`.

## fotografie, které nebyl použité pro knihu ani kalendář – dávka 02

Zpracovány byly `2061.JPG`, `2063.JPG`, `2069.jpg`, `209.jpg` a `327a.jpg`. Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Mezi pěti položkami není přesná binární duplicita uvnitř dávky.

`2061.JPG` zobrazuje zděné schodiště do podzemního či suterénního prostoru; EXIF uvádí Canon EOS 400D DIGITAL a DateTimeOriginal `2012:01:16 08:41:32`. `2063.JPG` zobrazuje odlomené barevně upravené fragmenty s částečnými znaky; stejný model fotoaparátu a DateTimeOriginal `2012:01:16 08:59:13`. Přesná stavba, lokalita, funkce schodiště, materiál, původ, stáří a význam fragmentů nejsou určeny.

`2069.jpg` je digitální reprodukce situačního plánu. Bezpečně čitelné jsou mimo jiné `Vodovod pro velkostatek v Rychvaldě.`, `Situace.`, měřítko `1:2880`, `Ing. M. Rosický, Orlová.`, místní popisky `Heřmanice` a `Rychvald`, označení `Závod pro stavbu vodovodů ING. MIROSLAV ROSICKÝ ORLOVA` a datace `Orlová, v červnu 1934.`. Viditelná datace je údaj samotného plánu; EXIF DateTimeOriginal `2012:03:11 10:37:36` je evidován odděleně jako metadata digitálního snímku/reprodukce.

`209.jpg` zachycuje několik osob provádějících zemní práce s nástroji kolem velkého zaobleného kamene; přesná činnost, událost, lokalita, datum a osoby nejsou určeny.

`327a.jpg` je přesná binární duplicita dříve indexovaného `fotodokument/img041.jpg` (`urbanek-fotodokument-root-006`): shoduje se velikost, Git blob SHA `1d9cc6086818160982d6854da7b6d6857292019b` i SHA-256 `a20b389ac31ff0c253a0e9be238961a9173cbf5cd994d1e1bce5d6967d2ba922`. Obě archivní cesty se zachovávají, ale obraz se nepovažuje za dva nezávislé důkazy.

Nejistota `URB-U-0084` byla rozšířena na položky 001–010; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotografie, které nebyl použité pro knihu ani kalendář | 18 | 1 | 19 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **65** | **5** | **70** |

## Registr nejistot

- `open`: 49;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 84.

## Aktuální krok

Třetí dávka kolekce `fotografie, které nebyl použité pro knihu ani kalendář`:

- `333.jpg`;
- `367.jpg`;
- `369.jpg`;
- `5005a.jpg`;
- `5011b.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
