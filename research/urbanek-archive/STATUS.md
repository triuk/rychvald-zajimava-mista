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
| zpracováno | 545 | 25 | **570** |
| zbývá | 42 | 4 | **46** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **13 kolekcí**. Aktivní je kolekce `novinové články 1903 - 1925`.

## novinové články 1903 - 1925 – dávka 01

Zpracovány byly `img970.jpg`, `img971.jpg`, `img972.jpg`, `img975.jpg` a `img976.jpg`. Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Uvnitř dávky není přesná binární duplicita.

`img970.jpg` reprodukuje `OBRANA SLEZSKA`, číslo 17, `V Orlové, 26. dubna 1912.`, `III. ročník.` a začátek článku `Naše stanovisko.`, `III.`, `3. Školství.`. Viditelný text se zabývá školskými a národnostními otázkami a zmiňuje mimo jiné Rychvald. `img971.jpg` se tištěným textem přímo překrývá s koncem textu na `img970.jpg` a dále v témže článkovém textu pokračuje.

`img972.jpg` reprodukuje masthead `OBRANA SLEZSKA`, číslo 30, `V Orlové, 26. července 1912.`, `III. ročník.`. `img976.jpg` reprodukuje číslo 40 téhož periodika s datací `V Orlové, 4. října 1912.` a `III. ročník.`.

`img975.jpg` je novinový výřez s bezpečně čitelným záhlavím `Z Rychvaldu.`. Viditelný text se věnuje otázce české školy a obecní správy, ale masthead, číslo a datum vydání v tomto výřezu nejsou zachyceny. Tištěná historická tvrzení článku jsou evidována jako obsah dobového pramene, nikoli jako nezávisle ověřené skutečnosti.

`img971.jpg`, `img972.jpg` a `img976.jpg` obsahují obecný EXIF DateTime z 29. května 2013, nikoli DateTimeOriginal; tato metadata nejsou používána jako data historických novinových čísel. Žádný z pěti souborů nemá GPS údaje.

Pro kolekci vznikla nová nejistota `URB-U-0085`; systematické bibliografické doplnění, návaznosti výřezů a nezávislé ověřování historických tvrzení zůstává podle workflow odloženo do závěrečné fáze.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| novinové články 1903 - 1925 | 11 | 2 | 13 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **42** | **4** | **46** |

## Registr nejistot

- `open`: 50;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 85.

## Aktuální krok

Druhá dávka kolekce `novinové články 1903 - 1925`:

- `img979.jpg`;
- `img983.jpg`;
- `img984.jpg`;
- `img985.jpg`;
- `img987.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
