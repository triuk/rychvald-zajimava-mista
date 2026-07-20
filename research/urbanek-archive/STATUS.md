# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Import originálů: commit `8c6e63be838f5b22ca8eed90e7cc9127352ebe5f`
- Poslední dokončený pracovní checkpoint: commit `f58f21e6b65a5fab8e6eefd821d660158f0c2a83`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt: potvrzeno uživatelem.

Tento soubor a `state.yml` jsou autoritativním předávacím bodem mezi chaty. Nový chat musí nejdříve načíst pravidla repozitáře, tento soubor a `state.yml` a ověřit aktuální hlavu větve.

## Neměnná rozhodnutí

- Originální soubory nepřejmenovávat, nepřesouvat ani neupravovat.
- Zachovat původní strukturu složek a názvy souborů.
- `Thumbs.db` a `ZbThumbnail.info` ponechat pro případnou další analýzu.
- Technické cache evidovat jako `technical_thumbnail_cache`; nezahrnovat je do běžné klasifikace ani OCR fotografií.
- Normalizované názvy používat pouze v inventáři nebo u odvozených pracovních výstupů.
- Fotografie zatím nevybírat do konkrétních článků.
- Každou dokončenou dávku commitnout a aktualizovat stavové soubory.

## OCR

OCR se vede odděleně jako:

1. `document_text` – články, dokumenty, popisky, titulní strany a podobné předlohy;
2. `scene_text` – nápisy na budovách, cedule, uliční tabule, pamětní desky, vývěsní štíty, plakáty, transparenty a další text zachycený ve scéně.

Strojový výstup má stav `machine_unverified`. Nečitelná místa se nedoplňují odhadem.

## Stav etap

| Etapa | Stav | Poznámka |
|---|---|---|
| Ruční import originálů | dokončeno s nesrovnalostmi | V první kolekci chybí v GitHubu pět technických cache, všechny obrazové soubory jsou přítomné. |
| Zachování technických cache | odloženo, zdokumentováno | Pět `Thumbs.db` zůstává na Drivu; jejich obsah byl analyzován. |
| Pravidla OCR včetně textu ve scéně | dokončeno | Zapsáno v `AGENTS.md`. |
| Technický audit importu | probíhá | První pilotní kolekce uzavřena, další čekají. |
| Hlavní inventář | probíhá | První kolekce má 39 úplných řádků. |
| Pilotní klasifikace | probíhá | Kolekce větrných mlýnů dokončena. |
| OCR | probíhá | U první kolekce dokončeny dva dokumentové přepisy a jeden krátký scénický nápis. |
| Draft pull request | čeká | Až po dokončení všech pěti pilotních kolekcí. |

## Pilotní kolekce

1. `Rychvaldské větrné mlýny` – **klasifikace a první OCR dokončeny**.
2. `Články z Českého slova` – následující kolekce, čeká inventář.
3. `Ochotníci rychvald` – čeká.
4. `fotodokument/den po dešti` – čeká.
5. `Nálet na Ostravu 1944` – čeká.

## Rychvaldské větrné mlýny – souhrn

- Na Drivu: 39 položek, z toho 31 obrazových a 8 technických cache.
- V GitHubu: všech 31 obrazových souborů a 3 `ZbThumbnail.info`; chybí 5 `Thumbs.db`.
- Všech 31 obrazových souborů bylo jednotlivě ověřeno a klasifikováno.
- Klasifikace je rozdělena do tří souborů v `research/urbanek-archive/collections/`.
- Hlavní inventář obsahuje stav klasifikace, Git blob SHA a skutečný stav obou kategorií OCR.
- Potvrzené přesné binární duplicity:
  - `urbanek-mlyny-011` = `urbanek-mlyny-021`;
  - `urbanek-mlyny-012` = `urbanek-mlyny-022` = `urbanek-mlyny-039`.
- Položky `urbanek-mlyny-013` až `015` jsou pravděpodobné zdrojové verze s vyšším rozlišením pro upravené položky `004` až `006`.
- `urbanek-mlyny-018` zachycuje interiér kostela a je pravděpodobně ve složce mlýnů omylem; originál nebyl přesunut.
- `urbanek-mlyny-039` je kopie obrázku označeného „Kakalův mlýn“ ve složce domu č. 339; vztah není vysvětlen.

## OCR první kolekce

- `urbanek-mlyny-024`: přepis informačního listu **Kouzlo větrných mlýnů**, Jan Doubek; položka `023` je detail stejného listu.
- `urbanek-mlyny-036`: přepis ručního náčrtu mlýnku za domem č. 339 včetně rozměrů.
- `urbanek-mlyny-028`: bezpečně čitelný scénický nadpis **„Výroba mouky z obilí“**.
- U položek `025` a `030` je text v pozadí příliš malý; u `026` je panel oříznutý. Text nebyl domýšlen.

## Audit `Thumbs.db`

Všech pět chybějících cache bylo analyzováno přímo z Drivu. Čtyři neobsahují názvy dalších fotografií. Kořenový `Thumbs.db` navíc eviduje chybějící `P1010269.JPG`; z cache byl obnoven platný náhled 72 × 96 px. Jde pouze o odvozený nález, nikoli náhradu originálu. Podrobnosti a kontrolní součty jsou v:

`research/urbanek-archive/reports/rychvaldske-vetrne-mlyny-thumbnail-cache.md`

Pět binárních cache se nepodařilo bezpečně připojit ke stromu větve přes dostupný konektor. Zůstávají proto na Drivu a v inventáři se stavem `drive_listed_repo_missing`. Tato technická odchylka neblokuje další kolekce.

## Následující přesný krok

Vytvořit úplný rekurzivní inventář kolekce `Články z Českého slova`, přidělit stabilní ID s novým prefixem, odlišit obrazové soubory od technických cache a ověřit jejich přesné cesty ve větvi. Teprve potom seskupovat stránky článků a zahájit OCR.

## Instrukce pro nový chat

1. Načíst `AGENTS.md`, `sources/README.md`, tento `STATUS.md` a `state.yml`.
2. Ověřit větev `agent/import-urbanek-pilot` a její aktuální hlavu.
3. Neměnit originální archivní soubory.
4. Pokračovat pouze krokem uvedeným v části **Následující přesný krok**.
5. Po malé dokončené dávce commitnout výstupy a aktualizovat oba stavové soubory.
