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
| zpracováno | **587** | **29** | **616** |
| zbývá | 0 | 0 | **0** |
| celý aktuální snapshot | **587** | **29** | **616** |

**Všech 15 kolekcí aktuálního Git snapshotu je zpracováno.** Kolekce `popopo` je dokončena 33/33. Tím je první úplný inventární a indexační průchod aktuálním snapshotem uzavřen.

## popopo – závěrečná dávka 07

Zpracovány byly `mlyn_0001a.jpg`, `Thumbs.db` a `ZbThumbnail.info`. Všechny tři raw soubory mají přesně stejnou velikost a přepočtený Git blob SHA jako příslušné cesty v repozitáři.

`mlyn_0001a.jpg` je digitální reprodukce archivní fotografie většího stavebního komplexu. EXIF uvádí Canon MP610 series, MP Navigator EX 1.0 a obecný DateTime `2012:04:18 09:02:04`; DateTimeOriginal ani GPS nejsou přítomny. Název souboru je pouze archivní atribuce a sám o sobě nedokládá, že zobrazený objekt je mlýn.

`Thumbs.db` je OLE/Compound File cache. Její Catalog obsahuje 57 názvů JPEGů plus jeden zvláštní GUID-like záznam; všech 31 současných JPEGů kolekce je zastoupeno. **26 názvů nemá v aktuální složce samostatný plný soubor.** Přímým porovnáním thumbnailů je 10 těchto názvů variantou stejného podkladového obrazu, který je v kolekci dochován pod jiným názvem. Po jejich odečtení cache dokládá **16 odlišných obrazových obsahů, jejichž plný originál v aktuálním snapshotu chybí**.

`ZbThumbnail.info` začíná `zbex`, obsahuje všech 57 názvů JPEGů známých z `Thumbs.db` a 57 přímo dekódovatelných JPEG/JFIF proudů. Nález chybějících názvů je tedy podpořen dvěma různými technickými cache soubory.

Pro 16 chybějících plných originálů byla založena nová nejistota `URB-U-0088`. Cache-only odkazy nejsou připočítány k 616 položkám aktuálního snapshotu.

## Registr nejistot

- `open`: 53;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 88.

## Další fáze

Úplná indexace aktuálního snapshotu je dokončena. Následujícím krokem je závěrečná kontrola registru nejistot, prioritizace a teprve poté jejich systematické řešení. Automaticky je nyní neuzavírám ani neslučuji.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
