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
| zpracováno | 556 | 27 | **583** |
| zbývá | 31 | 2 | **33** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je **14 kolekcí**. Kolekce `novinové články 1903 - 1925` je kompletně zpracována **18/18**. Zbývá jediná skupina `popopo`.

## novinové články 1903 - 1925 – dávka 04 a dokončení kolekce

Zpracovány byly `img995.jpg`, `Thumbs.db` a `ZbThumbnail.info`. Všechny tři raw soubory přesně odpovídají velikostem a Git blobům v repozitáři.

`img995.jpg` nemá EXIF ani GPS. Přímý vizuální a textový překryv s `img993.jpg` dokládá, že zachycuje stejnou stránku/sekci `OSTRAVSKÝ DENNÍK` s článkem `Boj—česko-polský.`, pouze ve větším vertikálním rozsahu.

`Thumbs.db` je OLE/Compound Document. Katalog obsahuje 34 pojmenovaných `.jpg` záznamů a jeden zvláštní GUID záznam; všech 35 thumbnail datových streamů obsahuje přímo dekódovatelné JPEG obrázky. V katalogu jsou všechna současná jména 16 samostatných JPEGů, ale také **18 názvů bez samostatného plného souboru**.

Šest z těchto 18 chybějících názvů má pixelově identický náhled s některým dochovaným JPEGem. U zbývajících jsou tři dvojice navzájem identických náhledů. Po odečtení těchto duplicit cache dokládá **9 odlišných obrazových obsahů bez samostatného plného souboru**.

`ZbThumbnail.info` začíná `zbex` a obsahuje 26 unikátních `.jpg` referencí: všech 16 současných názvů a deset chybějících názvů. Tyto reference nezávisle pokrývají stejných 9 odlišných chybějících obsahů. Kvůli rozdílné interní struktuře se u tohoto souboru nezapisuje silnější tvrzení o přesném počtu samostatně dekódovatelných vložených JPEGů.

Pro tento archivní deficit vznikla samostatná nejistota `URB-U-0086`. Nejistota `URB-U-0085` byla rozšířena na poslední obsahovou položku `img995.jpg`.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| popopo | 31 | 2 | **33** |

## Registr nejistot

- `open`: 51;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 86.

## Aktuální krok

Zahájit poslední kolekci `popopo`:

- 31 obsahových souborů;
- 2 technické soubory;
- Drive složka `1VPkXS5bIfelSjVOKfbxAurfcrigB7QLR`.

PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
