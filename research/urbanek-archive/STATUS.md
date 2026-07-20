# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml` a `uncertainties.yml`.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Technický audit a inventář | probíhá po kolekcích |
| Rychvaldské větrné mlýny | klasifikace a první OCR dokončeny |
| Články z Českého slova | první OCR i druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | inventář dokončen, ověřování cest probíhá |
| Ostatní dvě pilotní kolekce | čekají |
| Pull request | čeká |

## Registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

- `open`: 15
- `in_progress`: 0
- `deferred`: 2
- `resolved`: 5
- `not_actionable`: 1
- celkem: 23

Otevřené fyzické mezery OCR Českého slova zůstávají `URB-U-0020`, `URB-U-0021` a `URB-U-0022`.

## Články z Českého slova – uzavřený výsledek

- 37 obrazových položek bylo ověřeno, seskupeno a přepsáno.
- Druhou kontrolou prošlo všech 56 textových a scénických jednotek.
- `URB-U-0018` byla uzavřena jako dokončená kontrolní etapa.
- Chybějící text nebyl nikde rekonstruován odhadem.

## Ochotníci rychvald – inventář

Google Drive obsahuje **63 přímých položek** a žádné podsložky:

- 60 souborů JPEG;
- 1 původní dokument DOC (`112 let ochotnických souborů v.doc`);
- 2 technické cache (`Thumbs.db` a `ZbThumbnail.info`).

Inventář:

`research/urbanek-archive/collections/ochotnici-rychvald-inventory.csv`

Stabilní ID: `urbanek-ochotnici-001` až `urbanek-ochotnici-063`.

### Ověření GitHub cest

- `001–010`: ověřeno, 10 přítomných, 0 chybějících.
- `011–020`: ověřeno, 10 přítomných, 0 chybějících.
- Celkem: **20 z 63 položek ověřeno**, bez zjištěného přejmenování nebo chybějícího souboru.

Kontrolní soubory:

- `research/urbanek-archive/collections/ochotnici-rychvald-verification-01.yml`
- `research/urbanek-archive/collections/ochotnici-rychvald-verification-02.yml`

Obsahová klasifikace ani OCR této kolekce zatím nebyly zahájeny. JPEGy jsou v inventáři předběžně vedeny jako `image_or_document_scan_pending`, aby se jejich typ neurčoval pouze podle názvu souboru.

## Následující přesný krok

Ověřit přesné GitHub cesty a blob SHA položek `urbanek-ochotnici-021` až `urbanek-ochotnici-030`.

Pořadí práce:

1. dokončit ověření všech 63 cest;
2. zkontrolovat technické cache;
3. teprve potom vizuálně rozlišit fotografie, dokumentové skeny, programy, výstřižky a případný scénický text;
4. OCR zahájit až po klasifikaci a seskupení souvisejících dokumentů.

## Instrukce pro nový chat

1. Načíst autoritativní soubory.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat dávkou `021–030`.
5. Po malé dokončené dávce aktualizovat checkpoint.
