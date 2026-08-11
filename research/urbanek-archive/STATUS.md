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
| zpracováno | 581 | 27 | **608** |
| zbývá | 6 | 2 | **8** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **14 kolekcí**. Aktivní je poslední kolekce `popopo`, zpracováno **25/33**.

## popopo – dávka 05

Zpracovány byly `P1010764.JPG`, `P1010765a.jpg`, `P1010791.JPG`, `P1010791a.jpg` a `img129.jpg`. Všechny raw soubory přesně odpovídají velikostem a Git blobům v repozitáři; předchozí shoda blob SHA v indexovaných source záznamech nebyla nalezena.

`P1010764.JPG` zobrazuje památník s čitelnými nápisy `PAMÁTCE OBĚTEM NĚMECKÉ PERSEKUCE 1939–1945`, `PADLÝM BRATŘÍM 1914–1918`, `VAŠÍ PAMÁTCE VĚRNI ZŮSTANEME!` a viditelným `1948`. Jde o text objektu; historická a biografická tvrzení desky nejsou v této fázi nezávisle ověřena.

`P1010765a.jpg` je reprodukce historické fotografie otevřeného dřevěného altánu; přesná lokalita, funkce a datum nejsou určeny.

`P1010791.JPG` a `P1010791a.jpg` jsou přímo obrazově ověřené dvě různě zpracované reprezentace stejné rukopisné stránky `-272-`. Nejsou binárně totožné, ale nepředstavují dva různé rukopisné obsahy. Viditelné jsou mimo jiné `1. IX. 1912`, `170 dětí` a `40.000 K`; jde o obsah rukopisu, ne samostatně ověřené historické skutečnosti.

`img129.jpg` je historická fotografie nízké budovy se strmou střechou a dvěma komíny; přesná identita, funkce, lokalita a datum nejsou určeny.

Čtyři soubory dávky obsahují pouze obecný EXIF DateTime z 22.–23. dubna 2012, nikoli DateTimeOriginal; `img129.jpg` EXIF nemá. Žádný z pěti nemá GPS.

Nejistota `URB-U-0087` byla rozšířena na položky 001–025; nová nejistota nevznikla.

## Zbývající položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| popopo | 6 | 2 | **8** |

## Registr nejistot

- `open`: 52;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 87.

## Aktuální krok

Šestá dávka `popopo`:

- `img178a.jpg`;
- `img267.jpg`;
- `img678.jpg`;
- `img691.jpg`;
- `img698a.jpg`.

Poté zbude závěrečná trojice `mlyn_0001a.jpg`, `Thumbs.db`, `ZbThumbnail.info`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
