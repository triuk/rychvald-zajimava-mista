# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: commit `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený checkpoint při založení tohoto souboru: commit `62486dcbdfd7c63188720dc1d5e359a9b203ac79`
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
| Zachování technických cache | rozhodnuto | `Thumbs.db` a `ZbThumbnail.info` zůstávají. |
| Pravidla OCR včetně textu ve scéně | dokončeno | Doplněno do `AGENTS.md` v commitu `62486dcb…`. |
| Technický audit importu | probíhá | Úvodní audit přes GitHub konektor; úplný inventář ještě nevytvořen. |
| Hlavní inventář | čeká | Bude vytvořen po uzavření technického auditu. |
| Pilotní klasifikace | čeká | Pět kolekcí uvedených níže. |
| OCR | čeká | Až po základním inventáři a klasifikaci. |
| Draft pull request | čeká | Až po dokončení pilotu. |

## Pilotní kolekce

1. `Rychvaldské větrné mlýny`
2. `Články z Českého slova`
3. `Ochotníci rychvald`
4. `fotodokument/den po dešti`
5. `Nálet na Ostravu 1944`

## Dosavadní zjištění auditu

- Pilotní větev byla po importu o tři commity před `main` a nebyla za `main` pozadu.
- Importní commit zachovává původní názvy včetně diakritiky, mezer a původní hierarchie.
- Dříve vytvořená cesta s normalizovanými názvy `clanky-z-ceskeho-slova/` už na větvi nebyla nalezena.
- V archivu je alespoň jeden `ZbThumbnail.info` pod `Noviny 1938 České slovo/`; podle rozhodnutí uživatele se ponechává.
- Rozsah změn je příliš velký pro jediný úplný výpis přes GitHub konektor; konektor dlouhé seznamy zkracuje. Audit proto musí být
  uzavírán po složkách a každý výsledek průběžně ukládán do repozitáře.
- Úplný počet souborů, kontrolní součty a seznam potenciálních duplicit zatím nejsou spolehlivě dokončeny.

## Následující přesný krok

Dokončit technický audit po kořenových kolekcích a vytvořit `research/urbanek-archive/inventory.csv` alespoň se sloupci:

`id,original_path,filename,extension,collection,file_role,ocr_document_text,ocr_scene_text,rights,attribution,status,notes`

První zpracovanou pilotní kolekcí má být `Rychvaldské větrné mlýny`. Před jejím obsahovým hodnocením je nutné vytvořit úplný
seznam jejích souborů a zapsat checkpoint do tohoto souboru a `state.yml`.

## Instrukce pro nový chat

Nový chat musí:

1. načíst `AGENTS.md`, `sources/README.md`, tento `STATUS.md` a `state.yml`;
2. ověřit větev `agent/import-urbanek-pilot` a její aktuální hlavu;
3. neměnit originální archivní soubory;
4. pokračovat pouze krokem uvedeným v části **Následující přesný krok**;
5. po malé dokončené dávce commitnout výstupy a aktualizovat oba stavové soubory.
