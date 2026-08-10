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
| zpracováno | 501 | 22 | **523** |
| zbývá | 86 | 7 | **93** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **11 kolekcí**. Aktivní je kořenová část `fotodokument` mimo již dokončenou podsložku `den po dešti`.

## fotodokument – dávka 06

Zpracovány byly `img065.jpg`, `img066.jpg`, `img067.jpg`, `img068.jpg` a `img070.jpg`. Dávka obsahuje budovu s nápisem `SBĚRNA`, další neidentifikovanou větší zděnou budovu, pouliční průvod s vlajkami, veřejné shromáždění podél ulice a skupinový snímek na jevišti v kostýmech.

Všech pět raw souborů z kanonické Drive složky přesně odpovídá velikostem a Git blobům v repozitáři. Mezi pěti položkami není přesná binární duplicita. Žádný z pěti JPEGů neobsahuje použitelná EXIF metadata.

Na `img065.jpg` je bezpečně čitelné `SBĚRNA`; nápis dokládá dobové označení funkce, ale ne přesnou instituci, předmět sběru, provozovatele ani lokalitu. Na `img068.jpg` jsou na nejméně dvou vlajkách zřetelně viditelné symboly srpu a kladiva. Na směrové tabuli je čitelné číslo `5` a jen začátek názvu `OSTR…`; celý název není rekonstruován. Symbolika sama není používána k určení organizátora nebo příslušnosti účastníků.

`img067.jpg` a `img068.jpg` zachycují veřejné události s vlajkami a početnými skupinami osob, ale jejich přesný název, vzájemný vztah, datum a účastníci zůstávají neověřené. `img070.jpg` zachycuje skupinu na jevišti v kostýmech s hudebními nástroji; inscenace, soubor a osoby nejsou identifikovány.

Nejistota `URB-U-0083` byla rozšířena na položky 001–030; nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| fotodokument mimo `den po dešti` | 11 | 2 | 13 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **86** | **7** | **93** |

## Registr nejistot

- `open`: 48;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 83.

## Aktuální krok

Sedmá dávka kořenové části `fotodokument`:

- `img176.jpg`;
- `img178.jpg`;
- `img196.jpg`;
- `img197.jpg`;
- `img200.jpg`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
