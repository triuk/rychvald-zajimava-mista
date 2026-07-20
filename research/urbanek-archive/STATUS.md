# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: commit `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený pracovní checkpoint: commit `5370e74957ce61a6fe701892c91e707984a07bb7`
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
| Ruční import originálů | dokončeno s nesrovnalostmi | Obrazový obsah pilotní kolekce je přítomen; chybí některé technické cache. |
| Zachování technických cache | probíhá | `ZbThumbnail.info` jsou zachovány; v první kolekci chybí 5 souborů `Thumbs.db`. |
| Pravidla OCR včetně textu ve scéně | dokončeno | Doplněno do `AGENTS.md` v commitu `62486dcb…`. |
| Technický audit importu | probíhá | Kolekce větrných mlýnů má dokončené porovnání Drivu a GitHubu. |
| Hlavní inventář | probíhá | První kolekce má 39 řádků, stav cest a Git blob SHA. |
| Pilotní klasifikace | čeká | Začne po doplnění nebo výslovném odložení chybějících technických cache. |
| OCR | čeká | Až po základním inventáři a klasifikaci. |
| Draft pull request | čeká | Až po dokončení pilotu. |

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – 39 souborů na Drivu; 34 v GitHubu, 5 chybějících `Thumbs.db`.
2. `Články z Českého slova` – čeká.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Dosavadní zjištění auditu

- Pilotní větev byla po importu o tři commity před `main` a nebyla za `main` pozadu.
- Importní commit zachovává původní názvy včetně diakritiky, mezer a původní hierarchie.
- Dříve vytvořená cesta s normalizovanými názvy `clanky-z-ceskeho-slova/` už na větvi nebyla nalezena.
- Kolekce `Rychvaldské větrné mlýny` byla rekurzivně sepsána z Google Drivu do `inventory.csv`.
- Na Drivu obsahuje 39 položek: 31 obrazových souborů a 8 technických cache.
- Všech 31 obrazových souborů bylo jednotlivě potvrzeno ve větvi pod přesnými původními cestami.
- Ve větvi jsou všechny 3 soubory `ZbThumbnail.info` z této kolekce.
- Ve větvi chybí všech 5 očekávaných souborů `Thumbs.db`:
  - `Rychvaldské větrné mlýny/Thumbs.db`
  - `Rychvaldské větrné mlýny/větrný mlýn u hebdy/Thumbs.db`
  - `Rychvaldské větrné mlýny/Mlýn u Kakalů/Thumbs.db`
  - `Rychvaldské větrné mlýny/mlýnské kameny a ruční mlýny/Thumbs.db`
  - `Rychvaldské větrné mlýny/Mlýn u domku č. pop. 339/Thumbs.db`
- Inventář nyní obsahuje Git blob SHA všech 34 přítomných souborů a stav `drive_listed_repo_missing` u pěti chybějících cache.
- Potvrzené přesné binární duplicity:
  - `urbanek-mlyny-011` = `urbanek-mlyny-021`;
  - `urbanek-mlyny-012` = `urbanek-mlyny-022` = `urbanek-mlyny-039`.
- Stejně pojmenované soubory `P1010445`, `P1010446` a `P1010447` v kořeni a v podsložce `větrný mlýn u hebdy` mají
  rozdílné blob SHA a nejsou přesnými binárními duplicitami.

## Následující přesný krok

Doplnit pět chybějících souborů `Thumbs.db` z Google Drivu do přesných původních cest ve větvi. Poté znovu ověřit jejich blob
SHA, změnit pět stavů v `inventory.csv` na `repo_verified` a aktualizovat tento soubor a `state.yml`. Teprve potom zahájit
obsahovou klasifikaci 31 obrazových souborů kolekce `Rychvaldské větrné mlýny`, včetně posouzení kandidátů na `document_text`
a `scene_text` OCR.

## Instrukce pro nový chat

Nový chat musí:

1. načíst `AGENTS.md`, `sources/README.md`, tento `STATUS.md` a `state.yml`;
2. ověřit větev `agent/import-urbanek-pilot` a její aktuální hlavu;
3. neměnit originální archivní soubory;
4. pokračovat pouze krokem uvedeným v části **Následující přesný krok**;
5. po malé dokončené dávce commitnout výstupy a aktualizovat oba stavové soubory.
