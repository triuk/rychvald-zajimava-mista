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
| zpracováno | 412 | 18 | **430** |
| zbývá | 175 | 11 | **186** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je devět kolekcí. Kolekce `Noviny 1938 České slovo` je rozpracována v rozsahu 5 z 35 položek.

## Noviny 1938 České slovo – dávka 01

Zpracovány byly soubory `P1020273.JPG` až `P1020277.JPG`:

- `P1020273.JPG` – ručně popsaná rozřaďovací cedulka s texty „Poláci“, „České slovo“ a „1938“;
- `P1020274.JPG` – novinová strana s nadpisem „Zněmčelá území máme odevzdat do 10. října“ a textem podmínek mnichovské dohody;
- `P1020275.JPG` – titulní strana deníku *České slovo*, sobota 1. října 1938, ročník X, číslo 271, s hlavním titulkem „Povedeme národ do nového života“;
- `P1020276.JPG` – druhý, těsnější záběr stejné části strany jako `P1020274.JPG`; soubory nejsou binárně totožné;
- `P1020277.JPG` – články „Československo odstoupí Polsku část Těšínska“ a „První lord admirality proti Chamberlainovi“.

Všech pět JPEGů má 3072 × 2304 px, uvádí fotoaparát Panasonic DMC-TZ3 a EXIF DateTime 15. února 2013 mezi 11:36:52 a 11:39:25. Metadata jsou vedena jako údaje o fotografování archivních novinových předloh, nikoli jako datum vydání.

Nově je vedena nejistota `URB-U-0081` pro provenienci fyzických novin, úplnost vydání a stran, význam rozřaďovací cedulky, mezeru v pozdější filename posloupnosti, okolnosti digitalizace a práva.

Pracovní soubory kolekce:

- `research/urbanek-archive/collections/noviny-1938-ceske-slovo-overview.yml`;
- `research/urbanek-archive/collections/noviny-1938-ceske-slovo-batch-01.yml`;
- `research/urbanek-archive/collections/noviny-1938-ceske-slovo-inventory-01.csv`;
- `sources/index.d/urbanek-noviny-1938-ceske-slovo-01.yml`;
- `research/urbanek-archive/uncertainties/open-24.yml`.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Noviny 1938 České slovo – zbývá | 28 | 2 | 30 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **175** | **11** | **186** |

## Registr nejistot

- `open`: 46;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 81.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 430 položek;
- zbývá 186 položek;
- aktuální kolekce je zpracována v rozsahu 5 z 35 položek;
- mezi pěti soubory dávky není přesná binární duplicita;
- `P1020274.JPG` a `P1020276.JPG` jsou překrývající se, ale odlišné fotografie stejné stránky;
- registr používá součty 46/32/3/81;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `P1020278.JPG`, `P1020279.JPG`, `P1020280.JPG`, `P1020281.JPG` a `P1020283.JPG`.
- `P1020282.JPG` v aktuálním Git ani Drive snapshotu není; z mezery v číslování se bez důkazu neodvozuje chybějící originál.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
