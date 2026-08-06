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
| zpracováno | 427 | 18 | **445** |
| zbývá | 160 | 11 | **171** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je devět kolekcí. Kolekce `Noviny 1938 České slovo` je rozpracována v rozsahu 20 z 35 položek.

## Noviny 1938 České slovo – dávka 04

Zpracovány byly soubory `P1020289.JPG` až `P1020293.JPG`:

- `P1020289.JPG` – těsnější záběr článků „V sobotu se zahájí obsazování Fryštátska“ a „Zůstanou na Těšínsku české školy?“;
- `P1020290.JPG` – články „Fryštát už má polského starostu“ a „V Anglii nebude povinná vojenská služba“;
- `P1020291.JPG` – články „Jak přijal Londýn odstoupení presidenta“, „Zůstanou na Těšínsku české školy?“ a „Generál Syrový poděkoval Cooperovi“;
- `P1020292.JPG` – téměř celá druhá strana listu s titulky „První část fryštátského okresu obsazena“ a „Měsíc osvobození měsícem bolesti národa“; v těle textu je přímo uveden Rychvald;
- `P1020293.JPG` – téměř celá strana s titulkem „Fryštát s okolím zabrán“ a mezititulkem „Vojsko ustupuje z Fryštátu“.

`P1020289.JPG` a `P1020290.JPG` pokračují v překrývajících se detailech stránky fotografované v předchozí dávce. `P1020291.JPG` opakuje článek o českých školách, ale má jiné sousední texty; bez dalšího se neurčuje jako stejná fyzická strana nebo stejné vydání. `P1020292.JPG` a `P1020293.JPG` jsou dvě odlišné celostránkové fotografie.

Pouze `P1020292.JPG` ukazuje označení „ČESKÉ SLOVO“ a „Strana 2.“, avšak datum, ročník ani číslo vydání nejsou viditelné. Datace Londýn 6. října patří jednotlivým zprávám a není bez dalšího převáděna na datum vydání.

Všech pět JPEGů má 3072 × 2304 px, uvádí fotoaparát Panasonic DMC-TZ3 a EXIF DateTime 15. února 2013 mezi 15:54:52 a 15:57:48. Metadata jsou vedena jako údaje o fotografování archivních předloh, nikoli jako datum vydání novin.

Nejistota `URB-U-0081` byla rozšířena na položky 001–020. Mezi pěti soubory dávky není přesná binární duplicita.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Noviny 1938 České slovo – zbývá | 13 | 2 | 15 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **160** | **11** | **171** |

## Registr nejistot

- `open`: 46;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 81.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 445 položek;
- zbývá 171 položek;
- aktuální kolekce je zpracována v rozsahu 20 z 35 položek;
- všech pět Drive souborů přesně odpovídá Git blobům;
- mezi pěti soubory dávky není přesná binární duplicita;
- `P1020289.JPG` a `P1020290.JPG` navazují překrývajícími se detaily na předchozí dávku;
- registr používá součty 46/32/3/81;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `P1020294.JPG` až `P1020298.JPG`.
- `P1020282.JPG` v aktuálním Git ani Drive snapshotu není; z mezery v číslování se bez důkazu neodvozuje chybějící originál.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
