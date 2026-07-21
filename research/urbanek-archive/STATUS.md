# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdroj: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Pro další práci je autoritativní obsah pilotní větve v Git repozitáři.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties/index.yml` včetně odkazovaných shard souborů a `reports/pilot-reconciliation.md`.

## Stav pilotu

| Kolekce | Stav |
|---|---|
| Rychvaldské větrné mlýny | klasifikace a první OCR dokončeny |
| Články z Českého slova | první OCR i druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | první textový průchod i druhá vizuální kontrola dokončeny |
| fotodokument/den po dešti | technický audit a vizuální klasifikace dokončeny |
| Nálet na Ostravu 1944 | technický audit a vizuální klasifikace dokončeny |
| Reconciliace pilotu | dokončena |
| Úplnost pilotních souborů | **159 z 159 položek přítomno** |
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
- Obsahové soubory: **144 z 144 přítomno**.
- Technické soubory: **15 z 15 přítomno**.
- Celkem: **159 z 159 evidovaných položek přítomno**.
- Osmnáct souborů `Thumbs.db` v celém archivním stromu bylo doplněno commitem `7e6483d1bcb92034bea6eddd43fd55869dedce9c`.
- Z toho devět souborů uzavírá dříve chybějící technické položky pěti pilotních kolekcí.

Souhrnný report:

`research/urbanek-archive/reports/pilot-reconciliation.md`

## Chybějící plné originály

Audity technických cache prokázaly **11 chybějících plných originálů**. V repozitáři nejsou jako samostatné soubory; zachovány jsou pouze jejich náhledy v `Thumbs.db`:

- 0 v kolekci Rychvaldské větrné mlýny;
- 8 v kolekci Články z Českého slova;
- 2 v kolekci Ochotníci rychvald;
- 1 v kolekci `den po dešti`;
- 0 v kolekci Nálet na Ostravu 1944.

Náhledy v `Thumbs.db` nejsou samostatné zdrojové obrazy ani náhrada plných originálů. Pokud se však přesným obrazovým porovnáním prokáže, že náhled odpovídá plnému souboru dochovanému pod jiným názvem, nejde o chybějící obrazový obsah.

## fotodokument/den po dešti

- 8 JPEGů a 2 technické cache, bez podsložek.
- Všech deset evidovaných položek je ve větvi pod původními cestami.
- EXIF potvrzuje tři časově oddělené celky:
  - 5. srpna 2014;
  - série 24. srpna 2014;
  - samostatný kontext odvodnění 18. března 2015.
- Plný originál `P1020841.JPG` chybí; v `Thumbs.db` je zachován pouze jeho náhled.
- Kolekce nevyžaduje OCR.

Soubory:

- `collections/den-po-desti-inventory.csv`;
- `collections/den-po-desti-verification.yml`;
- `collections/den-po-desti-classification.yml`;
- `reports/den-po-desti-thumbnail-cache.md`.

## Nálet na Ostravu 1944

- 7 JPEGů a jeden `Thumbs.db`, bez podsložek.
- Všech osm evidovaných položek je ve větvi pod původními cestami.
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

- Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.
- `open`: 15;
- `deferred`: 0;
- `resolved`: 19;
- `not_actionable`: 1;
- celkem: 35.

Technické položky `URB-U-0001`, `URB-U-0024`, `URB-U-0033` a `URB-U-0035` byly uzavřeny doplněním příslušných souborů `Thumbs.db`.

Položky `URB-U-0012`, `URB-U-0025` a `URB-U-0034` byly uzavřeny konstatováním, že příslušné plné obrazy skutečně chybějí.

`URB-U-0002` a `URB-U-0003` byly zpřesněny: soubor pod názvem `P1010269.JPG` chybí, ale jeho plný obrazový obsah je dochován jako `mlýn na podlesí.JPG`; náhled v cache je duplicitní.

`URB-U-0004` byla ověřena databází Povětrník jako záznam 176, katalogové číslo mlýnek 49, na adrese Potoční 564. Databázová fotografie je oříznutou verzí archivního snímku; identita a lokalizace jsou `verified`.

`URB-U-0005` byla ověřena databází Povětrník jako záznam 175, katalogové číslo mlýnek 48, na adrese U Skučáku 54. Databázová fotografie se přesně shoduje s archivním záběrem stožáru; identita, lokalizace a funkční celek jsou `verified`. Dřívější inference Polní 1275 je překonaná.

`URB-U-0006` byla ověřena databází Povětrník jako záznam 229 na adrese U Školky 344. Databázová fotografie zachycuje stejný objekt jako archivní `mlýn na podlesí.JPG`.

`URB-U-0007` byla uzavřena potvrzením uživatele, že historický obraz zachycuje Kakalův mlýn. Veřejný web ani databáze Povětrník neposkytly adresu, dataci, vlastníka nebo technické údaje; tyto atributy zůstávají neověřené.

Původní `research/urbanek-archive/uncertainties.yml` je zachován jako historický snapshot a pro aktuální stav se nepoužívá. Další rychvaldské větrné mlýny se mají před uzavřením porovnat také s databází Povětrník.

## Aktuální krok

Stav pilotu:

`draft_pr_open_with_complete_pilot_file_set`

Další práce má probíhat kontrolou draft PR #1 a postupným řešením věcných nejistot. Technické soubory již nejsou překážkou.
