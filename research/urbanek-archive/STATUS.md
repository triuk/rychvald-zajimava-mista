# Stav zpracování archivu Jaromíra Urbánka

## Autoritativní kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový adresář: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.

Autoritativní předání mezi chaty tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a plán zpracování příslušné kolekce.

## Stav etap

| Etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Technický audit a inventář | probíhá po kolekcích |
| Rychvaldské větrné mlýny | klasifikace a první OCR dokončeny |
| Články z Českého slova | první OCR i druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | inventář, audit a klasifikace dokončeny; zpracování textu probíhá |
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
- `URB-U-0026`: rozpor v obsazení Fabiana — program a fotografie `025` uvádějí Radomíra Jurdina, název fotografie `051` uvádí Václava Válka. Rozpor se nesmí rozhodnout podle tváře.

## Články z Českého slova – uzavřený výsledek

- 37 obrazových položek bylo ověřeno, seskupeno a přepsáno.
- Druhou kontrolou prošlo všech 56 textových a scénických jednotek.
- Chybějící text nebyl nikde rekonstruován odhadem.

## Ochotníci rychvald – audit a klasifikace

- 63 položek na Drivu: 60 JPEG, 1 DOC a 2 technické cache.
- 62 položek je ve větvi pod přesnou původní cestou; chybí pouze `Thumbs.db`.
- Cache potvrdila všech 60 současných JPEGů a dva další unikátní náhledy bez plných originálů.
- Všech 63 položek bylo klasifikováno nebo technicky auditováno.
- Klasifikace: `research/urbanek-archive/collections/ochotnici-rychvald-classification-01.yml` až `06.yml`.
- Plán zpracování: `research/urbanek-archive/collections/ochotnici-rychvald-processing-plan.yml`.

## Dokončené textové výstupy Ochotníků

### Nativní extrakce

- `urbanek-ochotnici-061` — `112 let ochotnických souborů v Rychvaldu`.
  - Výstup: `research/urbanek-archive/ocr/urbanek-ochotnici-061-document-text.md`
  - Stav: `native_extracted_unverified`

### První průchod OCR

- `032–033` — titulní strana a obsazení programu `Večer tříkrálový`.
- `013` — program Celostátní soutěže vesnických divadelních souborů, 13.–19. května 1960.
- `023` — čestné uznání Sylvii Kravalové.
- `039` — program `Poslední noc v roce`.
- `042` — program `Slavnost lampiónů`.
- `047` — úřední dopis o věcné ceně 500 Kčs Sylvii Kravalové.
- `001` — úplný článek Petra Grimma `Vesničtí ochotníci ve finále`.

Všechny obrazové přepisy mají zatím stav `machine_unverified`. U článku `001` nebyl k fotografii doplněn popisek, protože na stránce žádný viditelný samostatný popisek není.

## Následující přesný krok

Přepsat `urbanek-ochotnici-004`, článek **„Thálie držela palce“**, včetně všech viditelných fotografických popisků vedených jako samostatné bloky.

Poté zpracovat primární zdroj `urbanek-ochotnici-010`, článek **„Katka, Angelika a Viola v Kroměříži“**; položku `009` použít jen jako kontrolní detail stejné stránky.

## Instrukce pro nový chat

1. Načíst autoritativní soubory a processing plan.
2. Ověřit aktuální hlavu větve.
3. Neměnit originály.
4. Pokračovat OCR položkou `004`.
5. Každý samostatný dokument commitnout zvlášť a novou podstatnou nejistotu zapsat do registru.
