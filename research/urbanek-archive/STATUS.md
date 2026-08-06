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
| zpracováno | 432 | 18 | **450** |
| zbývá | 155 | 11 | **166** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je devět kolekcí. Kolekce `Noviny 1938 České slovo` je rozpracována v rozsahu 25 z 35 položek.

## Noviny 1938 České slovo – dávka 05

Zpracovány byly soubory `P1020294.JPG` až `P1020298.JPG`:

- `P1020294.JPG` – těsnější záběr stejné strany jako `P1020293.JPG` s titulkem „Fryštát s okolím zabrán“;
- `P1020295.JPG` – strana s částečným označením „ČESKÉ SLOVO“ a titulkem „Předposlední den polské okupace“;
- `P1020296.JPG` – článek „Poslední den polského záboru na Těšínsku“ se samostatným mezititulkem „Jak se rozloučil Rychvald“;
- `P1020297.JPG` – články „Sta lidí vypovídáno z Těšínska“, „Konsulární atašé v Ostravě“ a „Italie sleduje vývoj ve střední Evropě“;
- `P1020298.JPG` – detail článku „Péče o uprchlíky z obsazeného území“.

`P1020294.JPG` a `P1020293.JPG` jsou překrývající se, ale binárně odlišné fotografie stejné strany. U ostatních snímků nebyl bezpečně stanoven překryv stejné fyzické stránky.

`P1020295.JPG` ukazuje částečné označení listu, ale nikoli úplné datum, ročník a číslo vydání. Datace Mor. Ostrava 10. října a Praha 14. října patří jednotlivým zprávám a nejsou bez dalšího převáděny na datum vydání.

Všech pět JPEGů uvádí fotoaparát Panasonic DMC-TZ3 a EXIF DateTime 15. února 2013 mezi 15:58:01 a 16:01:54. `P1020295.JPG` má rozměry 2304 × 3072 px; ostatní snímky mají 3072 × 2304 px. Metadata jsou vedena jako údaje o fotografování archivních předloh, nikoli jako datum vydání novin.

Nejistota `URB-U-0081` byla rozšířena na položky 001–025. Mezi pěti soubory dávky není přesná binární duplicita.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Noviny 1938 České slovo – zbývá | 8 | 2 | 10 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **155** | **11** | **166** |

## Registr nejistot

- `open`: 46;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 81.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 450 položek;
- zbývá 166 položek;
- aktuální kolekce je zpracována v rozsahu 25 z 35 položek;
- všech pět Drive souborů přesně odpovídá Git blobům;
- mezi pěti soubory dávky není přesná binární duplicita;
- `P1020294.JPG` je překrývající se, ale odlišný záběr stejné strany jako `P1020293.JPG`;
- registr používá součty 46/32/3/81;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `P1020299.JPG` až `P1020303.JPG`.
- `P1020282.JPG` v aktuálním Git ani Drive snapshotu není; z mezery v číslování se bez důkazu neodvozuje chybějící originál.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
