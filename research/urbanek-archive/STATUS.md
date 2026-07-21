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
| Ochotníci rychvald | **inventář, audit a klasifikace dokončeny; zpracování textu zahájeno** |
| Ostatní dvě pilotní kolekce | čekají |
| Pull request | čeká |

## Registr nejistot

Soubor: `research/urbanek-archive/uncertainties.yml`

- `open`: 17
- `in_progress`: 0
- `deferred`: 3
- `resolved`: 5
- `not_actionable`: 1
- celkem: 26

Nejistoty kolekce Ochotníci:

- `URB-U-0024`: případné doplnění chybějícího `Thumbs.db` do pilotní větve.
- `URB-U-0025`: hledání plných originálů `img387.jpg` a `ochotnicke divadlo 2xxx.jpg`, známých pouze z cache.
- `URB-U-0026`: program uvádí Fabiana jako Radomíra Jurdina, ale název fotografie `Fabiano - Václav Válek.jpg` uvádí Václava Válka. Rozpor se nesmí rozhodnout podle tváře na fotografii.

## Články z Českého slova – uzavřený výsledek

- 37 obrazových položek bylo ověřeno, seskupeno a přepsáno.
- Druhou kontrolou prošlo všech 56 textových a scénických jednotek.
- Chybějící text nebyl nikde rekonstruován odhadem.

## Ochotníci rychvald – technický audit

- 63 položek na Drivu: 60 JPEG, 1 DOC a 2 technické cache.
- 62 položek je ve větvi pod přesnou původní cestou; chybí pouze `Thumbs.db`.
- Cache potvrdila všech 60 současných JPEGů a obsahuje dva další unikátní náhledy bez plných originálů.
- Report: `research/urbanek-archive/reports/ochotnici-rychvald-thumbnail-cache.md`.

## Ochotníci rychvald – klasifikace

Všech **63 inventárních položek** bylo klasifikováno nebo technicky auditováno:

- 60 obrazových souborů;
- 1 původní dokument DOC;
- 2 technické cache.

Klasifikace je rozdělena do šesti souborů:

- `ochotnici-rychvald-classification-01.yml` až `ochotnici-rychvald-classification-06.yml`.

Souhrnný plán textového zpracování:

`research/urbanek-archive/collections/ochotnici-rychvald-processing-plan.yml`

### Hlavní skupiny

- celostátní přehlídka v Kroměříži roku 1960;
- program, obsazení, ocenění a fotografie Večera tříkrálového;
- programy Poslední noci v roce a Slavnosti lampiónů;
- článek Bořivoje Pešky z časopisu Těšínsko, potvrzený jako dvě přímo navazující strany;
- knižní dvoustrany 40–45 s pokračujícími a překrývajícími se články;
- rukopisné kronikové strany 260–262;
- rukopisný přehled činnosti Miroslava Neboráka;
- historická fotografie divadelního kroužku z roku 1923;
- jevištní fotografie, u nichž jsou jména a role vedeny jako archivní popisky, nikoli jako identifikace podle tváří.

### Důležitá zjištění

- `P1020771.JPG` je primární úplnější záběr kronikové strany 262; `P1020772.JPG` je kontrolní detail.
- `P1020599.JPG` je primární záběr článku „Katka, Angelika a Viola v Kroměříži“; `P1020600.JPG` je detail.
- `Článek v čas. Těšínsko I.jpg` a `Článek v čas. Těšínsko.jpg` tvoří jeden dvoustránkový článek.
- `img356.jpg` je samostatná reprodukce stejné fotografie, která je vložena na kronikové straně 261 a označena popiskem `Bohuš Koci`.
- Výstavní panely se nebudou plně OCRovat, pokud existují kvalitnější samostatné reprodukce vložených dokumentů.

## Zahájené textové zpracování

1. `urbanek-ochotnici-061`: nativně extrahován text DOC `112 let ochotnických souborů v Rychvaldu` přes LibreOffice se zachovanou českou diakritikou.
   - výstup: `research/urbanek-archive/ocr/urbanek-ochotnici-061-document-text.md`
   - stav: `native_extracted_unverified`
2. `urbanek-ochotnici-033` + `032`: přepsána titulní strana a úplné obsazení programu Večera tříkrálového.
   - výstup: `research/urbanek-archive/ocr/urbanek-ochotnici-032-033-document-text.md`
   - stav: `machine_unverified`

## Následující přesný krok

Přepsat `urbanek-ochotnici-013`, program **Celostátní soutěže vesnických divadelních souborů, 13.–19. května 1960**. Zachovat chronologické členění, názvy souborů, autory a tituly her.

Poté samostatně zpracovat:

1. `urbanek-ochotnici-023` – čestné uznání Sylvii Kravalové;
2. `urbanek-ochotnici-039` – program `Poslední noc v roce`;
3. `urbanek-ochotnici-042` – program `Slavnost lampiónů`;
4. `urbanek-ochotnici-047` – úřední oznámení o věcné ceně.

## Instrukce pro nový chat

1. Načíst autoritativní soubory a processing plan.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat OCR položkou `013`.
5. Každý samostatný dokument commitnout zvlášť a novou podstatnou nejistotu zapsat do registru.
