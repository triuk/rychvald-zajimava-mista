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
| zpracováno | 450 | 20 | **470** |
| zbývá | 137 | 9 | **146** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je deset kolekcí. Kolekce `Rychvald` je rozpracována v rozsahu 10 z 33 položek.

## Rychvald – dávka 02

Zpracovány byly soubory `Cudlín 041.jpg`, `Kopie - Budova úřadu 005.jpg`, `P1010066.JPG`, `P1010067.JPG` a `P1010068.JPG`:

- `Cudlín 041.jpg` zachycuje interiér sakrální stavby s uličkou mezi lavicemi zdobenými bílými květy a stuhami, oltářem, krucifixem a nástěnnými malbami;
- `Kopie - Budova úřadu 005.jpg` je podle SHA-256 i Git blob SHA přesná binární kopie položky 002 a nepředstavuje další nezávislý obrazový důkaz;
- `P1010066.JPG` je moderní reprodukce starší černobílé fotografie či pohlednice s formální veřejnou scénou před sakrální stavbou, uniformovanými řadami, prapory a davem;
- `P1010067.JPG` je reprodukce skupinového snímku dětí a dospělých před provozovnami; čitelné jsou nápisy „Baťa a.s.“, „RESTAURACE“, „TEPLÁ A STUDENÁ JÍDLA“ a „PIVO“;
- `P1010068.JPG` zachycuje desku se dvěma snímky školních budov, rokem „1909“ a popiskem „ŠKOLY U.M.Š. V RYCHVALDĚ.“.

Všech pět souborů přesně odpovídá Drive i Git blobům. `Cudlín 041.jpg` uvádí Panasonic DMC-FZ7 a čas 28. srpna 2009 15:59:46. Přesná kopie úřadu zachovává metadata 2. září 2008. Soubory `P1010066.JPG` až `P1010068.JPG` uvádějí Panasonic DMC-TZ3 a časy 28. února 2010 mezi 12:34:50 a 12:37:29.

Viditelný rok a popisek škol jsou evidovány doslovně. Bez dalšího neprokazují význam zkratky U.M.Š., datum obou fotografií ani přesnou identitu budov. Osoby, konkrétní události a historická data nejsou určovány pouze podle vzhledu, uniforem, krojů, praporů nebo architektury.

Nejistota `URB-U-0082` byla rozšířena na položky 001–010. Nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvald – zbývá | 21 | 2 | 23 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **137** | **9** | **146** |

## Registr nejistot

- `open`: 47;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 82.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 470 položek;
- zbývá 146 položek;
- kolekce `Rychvald` je zpracována v rozsahu 10 z 33 položek;
- všech pět Drive souborů přesně odpovídá Git blobům;
- v dávce není přesná binární duplicita mezi pěti vybranými cestami;
- položka 007 je potvrzený přesný duplikát položky 002;
- registr používá součty 47/32/3/82;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `P1010069.JPG`, `P1010070.JPG`, `P1010071.JPG`, `P1010072.JPG` a `P1010114.JPG`.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
