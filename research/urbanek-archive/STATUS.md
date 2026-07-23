# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdroj: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Pro další práci je autoritativní obsah pracovní větve v Git repozitáři.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties/index.yml` včetně odkazovaných shard souborů, `reports/pilot-reconciliation.md` a přehledy nových archivních dávek v `collections/`.

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

PR obsahuje dokončený pilot a nově také rozpracovanou následující archivní dávku. Pilotní součty se nemění; nová dávka se eviduje odděleně, dokud nebude kompletně zpracována a zrevidována.

## Celkové součty pilotu

- Pilotní kolekce: **5**.
- Obsahové soubory: **144 z 144 přítomno**.
- Technické soubory: **15 z 15 přítomno**.
- Celkem: **159 z 159 evidovaných položek přítomno**.
- Osmnáct souborů `Thumbs.db` v celém archivním stromu bylo doplněno commitem `7e6483d1bcb92034bea6eddd43fd55869dedce9c`.
- Z toho devět souborů uzavírá dříve chybějící technické položky pěti pilotních kolekcí.

Souhrnný report:

`research/urbanek-archive/reports/pilot-reconciliation.md`

## Nová archivní dávka – historie Církve československé

- Archivní složka: `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`.
- Struktura: **10 tematických podsložek**.
- Obsahové soubory: **200 JPEGů**.
- Technické soubory: **1× Thumbs.db** v podsložce `10 Kalendář 2015`.
- Celkem: **201 položek**.
- Původní soubory jsou ve větvi pod původními cestami; úplná položková kontrola Git blob SHA probíhá postupně po dávkách.
- První dávka pěti snímků dokumentujících položení základního kamene a výstavbu byla vizuálně zkontrolována, položkově inventarizována a propojena s Git blob SHA.
- Dočasné exportní a fragmentové soubory použité při kontrole `URB-U-0032` byly z větve odstraněny.

Pracovní soubory:

- `collections/historie-cirkve-ceskoslovenske-overview.yml`;
- `collections/historie-cirkve-ceskoslovenske-inventory-01.csv`;
- `collections/historie-cirkve-ceskoslovenske-batch-01.yml`.

## Chybějící plné originály pilotu

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
- `open`: 4;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 38.

Technické položky `URB-U-0001`, `URB-U-0024`, `URB-U-0033` a `URB-U-0035` byly uzavřeny doplněním příslušných souborů `Thumbs.db`.

Položky `URB-U-0012`, `URB-U-0025` a `URB-U-0034` byly uzavřeny konstatováním, že příslušné plné obrazy skutečně chybějí.

`URB-U-0002` a `URB-U-0003` byly zpřesněny: soubor pod názvem `P1010269.JPG` chybí, ale jeho plný obrazový obsah je dochován jako `mlýn na podlesí.JPG`; náhled v cache je duplicitní.

`URB-U-0004` byla ověřena databází Povětrník jako záznam 176, katalogové číslo mlýnek 49, na adrese Potoční 564. Databázová fotografie je oříznutou verzí archivního snímku; identita a lokalizace jsou `verified`.

`URB-U-0005` byla ověřena databází Povětrník jako záznam 175, katalogové číslo mlýnek 48, na adrese U Skučáku 54. Databázová fotografie se přesně shoduje s archivním záběrem stožáru; identita, lokalizace a funkční celek jsou `verified`. Dřívější inference Polní 1275 je překonaná.

`URB-U-0006` byla ověřena databází Povětrník jako záznam 229 na adrese U Školky 344. Databázová fotografie zachycuje stejný objekt jako archivní `mlýn na podlesí.JPG`.

`URB-U-0007` byla uzavřena pouze v rozsahu identity obrazu: historický snímek zachycuje Kakalův mlýn. Přesná poloha, číslo domu, vlastník, datace a technologie jsou vedeny jako samostatná otevřená položka `URB-U-0036`.

`URB-U-0036` se musí znovu prověřit po zpracování každé další relevantní dávky archivu, nového OCR, mapového nebo adresního pramene. Současný negativní výsledek internetového hledání není důvodem k jejímu uzavření.

`URB-U-0009` byla uzavřena pouze pro identifikaci snímku jako interiéru kostela sv. Anny v Rychvaldě. Význam čísla `304` a důvod uložení ve složce Kakalova mlýna zůstávají otevřeny jako `URB-U-0037`.

`URB-U-0010` byla uzavřena pro vztah náčrtu a dvou fotografií k jednomu mlýnku označenému jako zařízení za domem č. 339. Přesná historická poloha, kontinuita čísla domu, vlastník a datace zůstávají otevřeny jako `URB-U-0038`; dnešní Bohumínská 339 je pouze kandidát.

`URB-U-0011` byla uzavřena jako chybně zařazená přesná kopie obrazu Kakalova mlýna ve složce domu č. 339. Jde o jiný objekt a soubor se nepoužívá jako doklad k mlýnku u č.p. 339; původní archivní cesta se zachovává.

`URB-U-0017` byla označena jako `not_actionable`: úzký proužek nad článkem v souboru `9.jpg` je pouze spodní okraj předchozího článku zachycený na fotografii navíc. Není součástí cílového výstřižku ani samostatným předmětem OCR či identifikace.

`URB-U-0020` byla uzavřena jako známá, ale nepodstatná fyzická lakuna v článku „Zprávy z Těšínska“. Veškerý dochovaný text je přepsán; chybějící úsek zůstává výslovně označen a nesmí být rekonstruován odhadem.

`URB-U-0021` byla uzavřena jako známá ořezová lakuna článku „Polský zábor českých obcí dokončen“. Fotografie zachycuje pouze horní část novinové strany; chybějící spodní části sloupců zůstávají označeny a nesmějí být rekonstruovány odhadem.

`URB-U-0022` byla uzavřena jako známá fyzická lakuna ve výstřižku `33.jpg`. Několik zničených řádků zůstává výslovně označeno a nesmí být rekonstruováno odhadem.

`URB-U-0023` byla označena jako `not_actionable`: horní proužek v souboru `18.jpg` je pouze spodní okraj předchozího článku zachycený na fotografii navíc. Není součástí cílového výstřižku ani samostatným předmětem OCR či identifikace.

`URB-U-0026` byla uzavřena jako potvrzená alternace role Fabiana. Tištěný program uvádí Radomíra Jurdina; Václav Válek jej v roli alternoval. Obě archivní fotografie jsou proto správně pojmenované. Přesné rozdělení jednotlivých repríz mezi oba herce není doloženo.

`URB-U-0027` byla uzavřena: oba články popisují tutéž soutěž. Hodnota 3915 je přesný počet přihlášených scén; formulace „na 3960“ je pouze dobové přibližné zaokrouhlení.

`URB-U-0028` byla uzavřena: Eva Močkořová hrála Olivii. Podoba „Ofélie“ v retrospektivním článku Bořivoje Pešky je autorský nebo tiskový omyl; v doslovném přepisu zůstává zachována s výslovnou opravnou poznámkou.

`URB-U-0032` byla uzavřena jako známá ořezová lakuna bez dalšího hledání. Veškerý dochovaný text výsledkového bloku je přepsán; pokračování odříznuté dolním okrajem snímku zůstává výslovně označeno a nesmí být rekonstruováno odhadem.

Původní `research/urbanek-archive/uncertainties.yml` je zachován jako historický snapshot a pro aktuální stav se nepoužívá. Další rychvaldské větrné mlýny se mají před uzavřením porovnat také s databází Povětrník.

## Aktuální krok

Stav pilotu:

`draft_pr_open_with_complete_pilot_file_set`

Stav nové dávky:

`ccs_history_batch_processing_in_progress`

Pokračovat položkami 6–10 první podsložky, poté v dávkách po 5–10 souborech. Každá zpracovaná položka musí mít vizuální klasifikaci, `repo_status`, Git blob SHA, stav práv a oddělený `document_text`/`scene_text`. Čtyři dřívější otevřené položky registru zůstávají aktivní a mají se znovu prověřit pouze tehdy, přinese-li nová dávka relevantní důkaz.