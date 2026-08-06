# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový kořen: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt bylo potvrzeno.
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Autoritativním pracovním úložištěm je Git repozitář.

## Draft pull request

- PR: [#1 – Index and classify Jaromír Urbánek archive (in progress)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

## Stav indexace

| Stav | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| zpracováno | 440 | 18 | **458** |
| zbývá | 147 | 11 | **158** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je devět kolekcí. V kolekci `Noviny 1938 České slovo` je zpracováno všech 33 obsahových JPEGů; zbývají dva technické soubory.

## Noviny 1938 České slovo – dávka 07

Zpracovány byly poslední tři obsahové soubory `P1020304.JPG` až `P1020306.JPG`:

- `P1020304.JPG` – portrétní detail rubriky „Zprávy z Těšínska“ s několika krátkými zprávami vztahujícími se k Doubravě;
- `P1020305.JPG` – články „Které sňatky na Těšínsku musí býti znovu provedeny“ a „Nový jízdní řád autobusů ČSD Ostrava-Val. Meziříčí“;
- `P1020306.JPG` – články „Protest uprchlíků z Petřvaldu“, „Žádají plebiscit v českých obcích, zabraných Poláky“ a „České obce se dožadují práva sebeurčení“.

Mezi třemi soubory dávky není přesná binární duplicita. `P1020304.JPG` opakuje rubrikový nadpis „Zprávy z Těšínska“, který se objevuje i na položkách 029 a 030; samotné opakování rubriky však nedokládá stejnou fyzickou stranu nebo vydání.

Na žádném snímku dávky není úplný masthead s datem, ročníkem a číslem vydání. Datum vydání se proto neodvozuje z obsahu ani z pořadí fotografií.

Všechny tři JPEGy uvádějí fotoaparát Panasonic DMC-TZ3 a EXIF DateTime 15. února 2013 mezi 16:08:51 a 16:10:53. `P1020304.JPG` má rozměry 2304 × 3072 px; `P1020305.JPG` a `P1020306.JPG` mají 3072 × 2304 px. Metadata jsou vedena jako údaje o fotografování archivních předloh, nikoli jako datum vydání novin.

Nejistota `URB-U-0081` byla rozšířena na položky 001–033. Počet nejistot se nezměnil.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Noviny 1938 České slovo – technický audit | 0 | 2 | 2 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **147** | **11** | **158** |

## Registr nejistot

- `open`: 46;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 81.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 458 položek;
- zbývá 158 položek;
- aktuální kolekce je zpracována v rozsahu 33 z 35 položek;
- všechny tři Drive soubory přesně odpovídají Git blobům;
- mezi třemi soubory dávky není přesná binární duplicita;
- všech 33 obsahových JPEGů kolekce je Git-ověřeno, vizuálně klasifikováno a zdrojově indexováno;
- registr používá součty 46/32/3/81;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další krok: technický audit `Thumbs.db` a `ZbThumbnail.info`.
- `P1020282.JPG` v aktuálním Git ani Drive snapshotu není; z mezery v číslování se bez důkazu neodvozuje chybějící originál.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
