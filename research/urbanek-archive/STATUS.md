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
| zpracováno | 417 | 18 | **435** |
| zbývá | 170 | 11 | **181** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je devět kolekcí. Kolekce `Noviny 1938 České slovo` je rozpracována v rozsahu 10 z 35 položek.

## Noviny 1938 České slovo – dávka 02

Zpracovány byly soubory `P1020278.JPG`, `P1020279.JPG`, `P1020280.JPG`, `P1020281.JPG` a `P1020283.JPG`:

- `P1020278.JPG` – těsnější záběr článků „Československo odstoupí Polsku část Těšínska“ a „První lord admirality proti Chamberlainovi“; obsahově se překrývá s `P1020277.JPG`, ale soubory nejsou binárně totožné;
- `P1020279.JPG` – články „Má Polsko nároky na české obce?“, „Slovenský ministr Černák hrozí demisí“, „Mnoho otázek před berlínskou komisí“ a „Radiopřístroje budou vráceny“;
- `P1020280.JPG` – články „Jak bude proveden plebiscit“, „České Fryštátsko protestuje proti připojení k Polsku“ a „Horníkům a koksárům ostravsko-karvinského revíru“;
- `P1020281.JPG` – článek „Situace na polsko-čs. hranici na Těšínsku“;
- `P1020283.JPG` – články „Poláci pokračují v obsazování těšínského území“, „Francie zase ve finančních nesnázích“ a „Malhomme se vrátil na Těšínsko“.

Na žádném snímku dávky není úplný masthead s datem, ročníkem a číslem vydání. Viditelné datace 3. a 4. října jsou datace jednotlivých zpráv a nejsou bez dalšího převáděny na datum vydání.

Všech pět JPEGů má 3072 × 2304 px a uvádí fotoaparát Panasonic DMC-TZ3. `P1020278.JPG` až `P1020281.JPG` mají EXIF DateTime 15. února 2013 mezi 11:40:06 a 11:42:08; `P1020283.JPG` má čas 15:51:36. Metadata jsou vedena jako údaje o fotografování archivních předloh, nikoli jako datum vydání novin.

Nejistota `URB-U-0081` byla rozšířena na položky 001–010. Mezery v číslování a časový odstup před `P1020283.JPG` bez technického důkazu neprokazují chybějící archivní originál.

Pracovní soubory dávky:

- `research/urbanek-archive/collections/noviny-1938-ceske-slovo-batch-02.yml`;
- `research/urbanek-archive/collections/noviny-1938-ceske-slovo-inventory-02.csv`;
- `sources/index.d/urbanek-noviny-1938-ceske-slovo-02.yml`;
- aktualizovaný přehled kolekce a registr `open-24.yml`.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Noviny 1938 České slovo – zbývá | 23 | 2 | 25 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **170** | **11** | **181** |

## Registr nejistot

- `open`: 46;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 81.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 435 položek;
- zbývá 181 položek;
- aktuální kolekce je zpracována v rozsahu 10 z 35 položek;
- mezi pěti soubory dávky není přesná binární duplicita;
- `P1020278.JPG` a `P1020277.JPG` jsou překrývající se, ale odlišné fotografie stejné části stránky;
- registr používá součty 46/32/3/81;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `P1020284.JPG`, `P1020285.JPG`, `P1020286.JPG`, `P1020287.JPG` a `P1020288.JPG`.
- `P1020282.JPG` v aktuálním Git ani Drive snapshotu není; z mezery v číslování se bez důkazu neodvozuje chybějící originál.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
