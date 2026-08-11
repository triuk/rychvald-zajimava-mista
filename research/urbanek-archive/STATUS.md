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
| zpracováno | 576 | 27 | **603** |
| zbývá | 11 | 2 | **13** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **14 kolekcí**. Aktivní je poslední kolekce `popopo`, zpracováno **20/33**.

## popopo – dávka 04

Zpracovány byly `P1010748a.jpg`, `P1010749.JPG`, `P1010752.JPG`, `P1010754.JPG` a `P1010755a.jpg`. Všechny raw soubory přesně odpovídají velikostem a Git blobům v repozitáři; v dosud indexovaných source záznamech nebyla nalezena předchozí shoda Git blob SHA.

Všech pět souborů uvádí Panasonic DMC-TZ3 a pouze obecný EXIF DateTime, nikoli DateTimeOriginal. Hodnoty sahají od 10. do 17. dubna 2012; žádný soubor nemá GPS. Tyto hodnoty jsou evidovány pouze jako technická metadata souboru.

`P1010748a.jpg` je přímým obrazovým srovnáním doložen jako alternativní záběr či upravená reprodukce stejného krucifixu jako `P1010747a.jpg`; čitelné je `I.N.R.I.`.

`P1010749.JPG` zobrazuje výrazný starý listnatý strom u komunikace a elektrického vedení. `P1010752.JPG` zachycuje okraj zástavby s několika vzrostlými stromy a budovami. Přesná lokalita, identita a status těchto objektů nejsou určeny.

`P1010754.JPG` zobrazuje větší budovu s restauračními nápisy a pamětní deskou; bezpečně čitelné jsou `RESTAURACE`, `PENZION` a `PIVNICE`. `P1010755a.jpg` je přímo doložený detail pamětní desky na této budově. Čitelné jsou `PAMÁTCE RODINY EICHENBAUMŮ`, `V TÉTO BUDOVĚ`, `19. LISTOPADU 1905`, `BYL ZALOŽEN`, `SOKOL RYCHVALD` a `1949`. Jde o znění pamětní desky; historické tvrzení není v této fázi nezávisle ověřeno.

Nejistota `URB-U-0087` byla rozšířena na položky 001–020; nová nejistota nevznikla.

## Zbývající položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| popopo | 11 | 2 | **13** |

## Registr nejistot

- `open`: 52;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 87.

## Aktuální krok

Pátá dávka `popopo`:

- `P1010764.JPG`;
- `P1010765a.jpg`;
- `P1010791.JPG`;
- `P1010791a.jpg`;
- `img129.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
