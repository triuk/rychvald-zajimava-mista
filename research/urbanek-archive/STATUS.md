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
| zpracováno | 437 | 18 | **455** |
| zbývá | 150 | 11 | **161** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je devět kolekcí. Kolekce `Noviny 1938 České slovo` je rozpracována v rozsahu 30 z 35 položek.

## Noviny 1938 České slovo – dávka 06

Zpracovány byly soubory `P1020299.JPG` až `P1020303.JPG`:

- `P1020299.JPG` – rozostřený výřez s bezpečně čitelným titulkem „Němci lepší než Poláci“;
- `P1020300.JPG` – články „Přeplněné přívozské nádraží“, „Nový správce polského konsulátu v Ostravě“ a „Vojenský dozor na šachtách na Těšínsku“;
- `P1020301.JPG` – těsnější záběr spodní části stejné strany s články o poslanci Sliwkovi, vojenském dozoru na šachtách a soupisu zaměstnanců v Ostravě;
- `P1020302.JPG` – rubrika „Zprávy z Těšínska“ s přímými zmínkami Orlové, Petřvaldu, Karvinska a Suché;
- `P1020303.JPG` – článek „Novorozeně ve vagoně“ s podtitulem „Radostná událost na nádraží v Orlové“.

`P1020300.JPG` a `P1020301.JPG` jsou překrývající se, ale binárně odlišné fotografie stejné strany. Na `P1020302.JPG` a `P1020303.JPG` se opakuje rubrikový nadpis „Zprávy z Těšínska“, ale bez dalšího se neurčují jako stejná fyzická strana nebo stejné vydání.

Na žádném snímku dávky není úplný masthead s datem, ročníkem a číslem vydání. Datace Praha 24. října a další časové údaje v textech patří jednotlivým zprávám a nejsou bez dalšího převáděny na datum vydání.

Všech pět JPEGů uvádí fotoaparát Panasonic DMC-TZ3 a EXIF DateTime 15. února 2013 mezi 16:05:07 a 16:08:37. `P1020302.JPG` a `P1020303.JPG` mají rozměry 2304 × 3072 px; ostatní tři snímky mají 3072 × 2304 px. Metadata jsou vedena jako údaje o fotografování archivních předloh, nikoli jako datum vydání novin.

Nejistota `URB-U-0081` byla rozšířena na položky 001–030. Mezi pěti soubory dávky není přesná binární duplicita.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Noviny 1938 České slovo – zbývá | 3 | 2 | 5 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **150** | **11** | **161** |

## Registr nejistot

- `open`: 46;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 81.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 455 položek;
- zbývá 161 položek;
- aktuální kolekce je zpracována v rozsahu 30 z 35 položek;
- všech pět Drive souborů přesně odpovídá Git blobům;
- mezi pěti soubory dávky není přesná binární duplicita;
- `P1020301.JPG` je těsnější, ale odlišný záběr stejné strany jako `P1020300.JPG`;
- registr používá součty 46/32/3/81;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další obsahová dávka: `P1020304.JPG`, `P1020305.JPG` a `P1020306.JPG`.
- Po zpracování posledních tří JPEGů zbude technický audit `Thumbs.db` a `ZbThumbnail.info`.
- `P1020282.JPG` v aktuálním Git ani Drive snapshotu není; z mezery v číslování se bez důkazu neodvozuje chybějící originál.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
