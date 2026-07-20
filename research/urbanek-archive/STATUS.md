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
| Ochotníci rychvald | **inventář, ověření cest a audit cache dokončeny** |
| Ostatní dvě pilotní kolekce | čekají |
| Pull request | čeká |

## Registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

- `open`: 16
- `in_progress`: 0
- `deferred`: 3
- `resolved`: 5
- `not_actionable`: 1
- celkem: 25

Nově:

- `URB-U-0024`: případné doplnění chybějícího `Thumbs.db` do pilotní větve.
- `URB-U-0025`: hledání plných originálů `img387.jpg` a `ochotnicke divadlo 2xxx.jpg`, známých pouze z cache.

## Články z Českého slova – uzavřený výsledek

- 37 obrazových položek bylo ověřeno, seskupeno a přepsáno.
- Druhou kontrolou prošlo všech 56 textových a scénických jednotek.
- Chybějící text nebyl nikde rekonstruován odhadem.

## Ochotníci rychvald – technický audit

Google Drive obsahuje **63 přímých položek** a žádné podsložky:

- 60 souborů JPEG;
- 1 původní dokument DOC (`112 let ochotnických souborů v.doc`);
- 2 technické cache (`Thumbs.db` a `ZbThumbnail.info`).

Inventář:

`research/urbanek-archive/collections/ochotnici-rychvald-inventory.csv`

Stabilní ID: `urbanek-ochotnici-001` až `urbanek-ochotnici-063`.

### Ověření GitHub cest

- zkontrolováno všech **63** položek;
- **62** souborů je přítomných pod přesným původním názvem a cestou;
- chybí pouze technický `Thumbs.db` (`urbanek-ochotnici-036`);
- všech 60 JPEGů, dokument DOC a `ZbThumbnail.info` jsou přítomné;
- kontrolní blob SHA jsou rozděleny do sedmi souborů `ochotnici-rychvald-verification-01.yml` až `07.yml`.

### Audit `Thumbs.db`

Report:

`research/urbanek-archive/reports/ochotnici-rychvald-thumbnail-cache.md`

Výsledek:

- SHA-256 cache: `61a49eda18010a9b66e9bf43a5f039d81cedb3ff8e44597306c75b1b54fa5ecd`;
- 93 katalogových záznamů, z toho 92 názvů obrazů a jedna systémová koláž složky;
- všech 60 současných JPEGů je v cache zastoupeno;
- 29 starších názvů jsou přejmenování nebo meziverze současných souborů;
- cache obsahuje dva další unikátní obrazy bez nalezeného plného originálu:
  - `img387.jpg` – historická skupinová fotografie;
  - `ochotnicke divadlo 2xxx.jpg` / `ochotnicke divadlo 2xxxaa.jpg` – reprodukce tištěné stránky s fotografií a textem.

Náhledy mají pouze přibližně 96 px a nejsou náhradou originálů ani podkladem pro spolehlivé OCR.

## Následující přesný krok

Vizuálně klasifikovat položky `urbanek-ochotnici-001` až `010`:

1. rozlišit dokumentové skeny, výstavní panely, fotografie a jiné textové předlohy;
2. označit kandidáty `document_text` a `scene_text`;
3. určit, které fotografie nebo stránky tvoří společné série;
4. OCR nezahajovat, dokud nebudou související dokumenty seskupeny.

## Instrukce pro nový chat

1. Načíst autoritativní soubory.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat klasifikací `001–010`.
5. Po malé dokončené dávce aktualizovat checkpoint.
