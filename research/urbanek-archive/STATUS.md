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
| zpracováno | 460 | 20 | **480** |
| zbývá | 127 | 9 | **136** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je deset kolekcí. Kolekce `Rychvald` je rozpracována v rozsahu 20 z 33 položek.

## Rychvald – dávka 04

Zpracovány byly soubory `P1010115.JPG`, `P1010116.JPG`, `P1010117.JPG`, `Rychvald2009 003.jpg` a `Rychvald2009 004.jpg`:

- `P1010115.JPG` je fotografovaná rukopisná stránka s číslem „- 26 -“ a časovými rozsahy od 1715–1719 po 1894–1903; úplný kurzivní přepis a historická správnost údajů nejsou v této fázi ověřeny;
- `P1010116.JPG` je fotografovaná rukopisná stránka s chronologicky řazenými místními událostmi a bezpečně čitelnými datovanými položkami z let 1920 až 1923; jednotlivé zápisy jsou evidovány jako obsah předlohy, nikoli jako nezávisle ověřené historické skutečnosti;
- `P1010117.JPG` je fotografovaná rukopisná stránka s číslem „- 197 -“ a nadpisem „Škola živnostenská pokračovací.“; viditelné jsou mimo jiné roky 1912 a 1920;
- `Rychvald2009 003.jpg` a `Rychvald2009 004.jpg` jsou dva odlišné barevné snímky téhož kamenného hřbitovního kříže s figurální výzdobou, pořízené z mírně odlišného záběru s odstupem 13 sekund. Slabý nápis či datace na podstavci nejsou bezpečně čitelné.

Všech pět souborů přesně odpovídá raw souborům z Drive a Git blobům. `P1010115.JPG` až `P1010117.JPG` uvádějí Panasonic DMC-TZ3 a časy 1. září 2010 15:18:04 až 15:27:38. `Rychvald2009 003.jpg` a `Rychvald2009 004.jpg` uvádějí Panasonic DMC-FZ7 a časy 1. září 2009 09:15:37 a 09:15:50. Tyto časy jsou metadata moderního zachycení, nikoli data historických událostí nebo vzniku rukopisných předloh.

Mezi pěti položkami dávky 04 není přesná binární duplicita. Hřbitovní dvojice je evidována jako dva samostatné, téměř po sobě pořízené záběry stejného objektu.

Nejistota `URB-U-0082` byla rozšířena na položky 001–020. Nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvald – zbývá | 11 | 2 | 13 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **127** | **9** | **136** |

## Registr nejistot

- `open`: 47;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 82.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 480 položek;
- zbývá 136 položek;
- kolekce `Rychvald` je zpracována v rozsahu 20 z 33 položek;
- všech pět raw Drive souborů dávky 04 přesně odpovídá Git blobům;
- v dávce 04 není přesná binární duplicita mezi pěti vybranými cestami;
- položky 019 a 020 jsou dva rozdílné snímky stejného objektu, nikoli binární kopie;
- dříve potvrzená položka 007 zůstává přesným duplikátem položky 002;
- registr používá součty 47/32/3/82;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `Rychvald2009 005.jpg`, `Rychvald2009 008.jpg`, `Zp0707 090.jpg`, `Zp1109 005.jpg` a `Zp1109 082.jpg`.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
