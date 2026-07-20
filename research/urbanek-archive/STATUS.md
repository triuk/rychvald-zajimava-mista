# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: commit `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený pracovní checkpoint: commit `8362cdc4b2d79f64dff3507bc133e98f9b21768b`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt: potvrzeno uživatelem.

Tento soubor a `state.yml` jsou autoritativním předávacím bodem mezi chaty. Nový chat nesmí rekonstruovat stav pouze z historie
konverzace; nejdříve musí načíst pravidla repozitáře, tento soubor a `state.yml` a ověřit aktuální hlavu větve.

## Neměnná rozhodnutí

- Originální soubory v archivním adresáři nepřejmenovávat, nepřesouvat a neupravovat.
- Zachovat původní strukturu složek a názvy souborů.
- `Thumbs.db` a `ZbThumbnail.info` ponechat pro případnou další analýzu.
- Technické cache evidovat jako `technical_thumbnail_cache`; nezahrnovat je do běžného OCR ani klasifikace fotografií.
- Normalizované názvy používat pouze v inventáři nebo u odvozených pracovních výstupů.
- Fotografie zatím nevybírat do konkrétních článků.
- Každou dokončenou dávku ihned commitnout a aktualizovat tento stav.

## OCR

OCR zahrnuje dvě oddělené kategorie:

1. `document_text` – články, dokumenty, popisky, titulní strany a jiné textové předlohy;
2. `scene_text` – nápisy na budovách, cedule, uliční tabule, pamětní desky, vývěsní štíty, plakáty, transparenty a další text
   zachycený přímo ve fotografované scéně.

Text ve scéně se má využít jako vodítko k identifikaci nebo upřesnění obsahu fotografie. Strojový výstup musí být označen
`machine_unverified`; nečitelná místa se nesmějí domýšlet. Podrobné pravidlo je v `AGENTS.md`.

## Stav etap

| Etapa | Stav | Poznámka |
|---|---|---|
| Ruční import originálů | dokončeno | Import je viditelný na pilotní větvi. |
| Zachování technických cache | dokončeno | `Thumbs.db` a `ZbThumbnail.info` zůstávají. |
| Pravidla OCR včetně textu ve scéně | dokončeno | Doplněno do `AGENTS.md` v commitu `62486dcb…`. |
| Technický audit importu | probíhá | Audit je dělen po kolekcích. |
| Hlavní inventář | probíhá | Založen `inventory.csv`; první kolekce má 39 řádků. |
| Pilotní klasifikace | čeká | Začne po ověření cest první kolekce v GitHub stromu. |
| OCR | čeká | Až po základním inventáři a klasifikaci. |
| Draft pull request | čeká | Až po dokončení pilotu. |

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – seznam z Drivu dokončen: 39 souborů, z toho 31 obrazových a 8 technických cache.
2. `Články z Českého slova` – čeká.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Dosavadní zjištění auditu

- Pilotní větev byla po importu o tři commity před `main` a nebyla za `main` pozadu.
- Importní commit zachovává původní názvy včetně diakritiky, mezer a původní hierarchie.
- Dříve vytvořená cesta s normalizovanými názvy `clanky-z-ceskeho-slova/` už na větvi nebyla nalezena.
- Technické cache se zachovávají a jsou v inventáři odděleny od obrazového materiálu.
- Kolekce `Rychvaldské větrné mlýny` byla rekurzivně sepsána z Google Drivu do `inventory.csv` v commitu `8362cdc4…`.
- Její inventář obsahuje 39 položek: 31 obrazových souborů a 8 technických cache.
- U všech 31 obrazových položek jsou samostatně připraveny stavy OCR pro `document_text` a `scene_text`.
- Stav řádků je zatím `drive_listed_repo_path_pending`: seznam je úplný podle Drivu, ale každá cesta ještě nebyla jednotlivě
  potvrzena v GitHub stromu.
- Rozsah celého importu je příliš velký pro jediný úplný výpis přes GitHub konektor; kontrola proto pokračuje po kolekcích.
- Kontrolní součty a analýza přesných či vizuálních duplicit ještě nejsou dokončeny.

## Následující přesný krok

Ověřit všech 39 cest kolekce `Rychvaldské větrné mlýny` proti větvi `agent/import-urbanek-pilot`. Po ověření změnit stav řádků
z `drive_listed_repo_path_pending` na `repo_verified`, zapsat případné chybějící nebo přebývající soubory a aktualizovat tento
soubor a `state.yml`. Teprve poté začít obsahovou klasifikaci a OCR kandidátů této kolekce.

## Instrukce pro nový chat

Nový chat musí:

1. načíst `AGENTS.md`, `sources/README.md`, tento `STATUS.md` a `state.yml`;
2. ověřit větev `agent/import-urbanek-pilot` a její aktuální hlavu;
3. neměnit originální archivní soubory;
4. pokračovat pouze krokem uvedeným v části **Následující přesný krok**;
5. po malé dokončené dávce commitnout výstupy a aktualizovat oba stavové soubory.
