# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdroj: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a `reports/pilot-reconciliation.md`.

## Stav pilotu

| Kolekce | Stav |
|---|---|
| Rychvaldské větrné mlýny | klasifikace a první OCR dokončeny |
| Články z Českého slova | první OCR i druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | první textový průchod i druhá vizuální kontrola dokončeny |
| fotodokument/den po dešti | technický audit a vizuální klasifikace dokončeny |
| Nálet na Ostravu 1944 | technický audit a vizuální klasifikace dokončeny |
| Reconciliace pilotu | dokončena |
| Draft pull request | **otevřen jako PR #1** |

## Draft pull request

- PR: [#1 – Import and classify Jaromír Urbánek archive pilot](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

PR slouží ke kontrole rozsahu pilotu, struktury metadat, OCR výstupů, auditů cache a evidence nejistot.

## Celkové součty

- Pilotní kolekce: **5**.
- Obsahové soubory na Drivu: **144**.
- Technické soubory na Drivu: **15**.
- Celkem evidovaných položek: **159**.
- Obsahové soubory přítomné ve větvi: **144 ze 144**.
- Technické soubory přítomné ve větvi: **6 z 15**.
- Ve větvi je celkem **150 z 159** položek.
- Chybí devět souborů `Thumbs.db`; všechny byly auditovány přímo z originálů na Drivu.

Souhrnný report:

`research/urbanek-archive/reports/pilot-reconciliation.md`

## Obrazy známé pouze z cache

Audity technických cache odhalily **12 unikátních obrazů**, jejichž plné originály nebyly nalezeny:

- 1 v kolekci Rychvaldské větrné mlýny;
- 8 v kolekci Články z Českého slova;
- 2 v kolekci Ochotníci rychvald;
- 1 v kolekci `den po dešti`;
- 0 v kolekci Nálet na Ostravu 1944.

Náhledy nejsou náhradou plných originálů.

## fotodokument/den po dešti

- 8 JPEGů a 2 technické cache, bez podsložek.
- Všech osm JPEGů je ve větvi; chybí `Thumbs.db`.
- EXIF potvrzuje tři časově oddělené celky:
  - 5. srpna 2014;
  - série 24. srpna 2014;
  - samostatný kontext odvodnění 18. března 2015.
- `P1020841.JPG` chybí jako plný originál; cache jej řadí bezprostředně před `P1020842.JPG`.
- Kolekce nevyžaduje OCR.

Soubory:

- `collections/den-po-desti-inventory.csv`;
- `collections/den-po-desti-verification.yml`;
- `collections/den-po-desti-classification.yml`;
- `reports/den-po-desti-thumbnail-cache.md`.

## Nálet na Ostravu 1944

- 7 JPEGů a jeden `Thumbs.db`, bez podsložek.
- Všech sedm JPEGů je ve větvi; chybí pouze technická cache.
- Cache obsahuje čtyři další pracovní názvy, ale jejich náhledy odpovídají dochovaným fotografiím; žádný nový unikátní výjev nechybí.
- Šest snímků dokumentuje těžce poškozené budovy a městské bloky.
- Jeden snímek zachycuje velký válcovitý předmět připomínající munici; přesný typ není z fotografie ověřen.
- Označení události a roku pochází z názvu archivní složky a není samo o sobě nezávislým historickým důkazem.
- Kolekce nevyžaduje OCR.

Soubory:

- `collections/nalet-na-ostravu-1944-inventory.csv`;
- `collections/nalet-na-ostravu-1944-verification.yml`;
- `collections/nalet-na-ostravu-1944-classification.yml`;
- `reports/nalet-na-ostravu-1944-thumbnail-cache.md`.

## Registr nejistot

- `open`: 23;
- `deferred`: 5;
- `resolved`: 6;
- `not_actionable`: 1;
- celkem: 35.

Nové položky:

- `URB-U-0033` — chybějící technický `Thumbs.db` kolekce `den po dešti`;
- `URB-U-0034` — plný originál `P1020841.JPG` známý pouze z cache;
- `URB-U-0035` — chybějící technický `Thumbs.db` kolekce Nálet na Ostravu 1944.

## Aktuální krok

Stav pilotu:

`draft_pr_open_with_known_deferred_technical_files`

Další práce má probíhat kontrolou draft PR #1. PR nemá být označen jako připravený ani sloučen, dokud nebude přijat rozsah pilotu a způsob zacházení s chybějícími technickými cache.
