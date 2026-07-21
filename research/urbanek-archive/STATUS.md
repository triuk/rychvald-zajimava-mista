# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdroj: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a plán příslušné kolekce.

## Etapy

| Kolekce / etapa | Stav |
|---|---|
| Rychvaldské větrné mlýny | klasifikace a první OCR dokončeny |
| Články z Českého slova | první OCR i druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | **první textový průchod dokončen; druhá kontrola probíhá** |
| fotodokument/den po dešti | čeká |
| Nálet na Ostravu 1944 | čeká |
| Pull request | čeká |

## Ochotníci rychvald

- Inventář: 63 položek — 60 JPEG, 1 DOC a 2 technické cache.
- Ve větvi je 62 položek; chybí pouze `Thumbs.db`.
- Všech 63 položek bylo klasifikováno nebo technicky auditováno.
- Plán: `research/urbanek-archive/collections/ochotnici-rychvald-processing-plan.yml`.

## Dokončený první textový průchod

Zpracovány byly všechny plánované textové zdroje:

- nativní DOC `061`;
- krátké programy, soutěžní program, čestné uznání a úřední dopis;
- kroměřížské články a tiskové recenze;
- dvoustránkový článek Bořivoje Pešky z časopisu Těšínsko;
- knižní strany 40–45;
- rukopisná kronika, strany 260–262;
- rukopisný přehled činnosti Miroslava Neboráka;
- scénický text fotografie divadelního kroužku z roku 1923;
- selektivní text dvou výstavních panelů.

## Druhá vizuální kontrola

### Dávka 01 — krátké strukturované dokumenty

Protokol:

`research/urbanek-archive/collections/ochotnici-rychvald-visual-review-01.yml`

Vizuálně ověřeno 7 zdrojových položek v 6 výstupech:

- `032–033` — program `Večer tříkrálový`;
- `013` — program celostátní soutěže;
- `023` — čestné uznání Sylvii Kravalové;
- `039` — program `Poslední noc v roce`;
- `042` — program `Slavnost lampiónů`;
- `047` — dopis o věcné ceně.

### Dávka 02 — skupina Kroměříž 1960

Protokol:

`research/urbanek-archive/collections/ochotnici-rychvald-visual-review-02.yml`

Zkontrolováno 8 zdrojových položek v 7 textových výstupech:

- `001` — `Vesničtí ochotníci ve finále`: `visually_verified`;
- `004` — `Thálie držela palce`: `visually_verified_with_lacuna`;
- `010` s kontrolním detailem `009` — `Katka, Angelika a Viola v Kroměříži`: `visually_verified`;
- `011` — první kroměřížská novinová stránka: `visually_verified`;
- `012` — `Rychvald a Shakespeare v Kroměříži`: `visually_verified`;
- `014` — `Vesničtí ochotníci se představují`: `visually_verified`;
- `027` — `Jaké jsou naše vesnické soubory?`: `visually_verified`.

### Opravy dávky 02

- `Rudolf Debnárik` → **`Rudolf Děbnárik`**.
- `zvýťazí` → **`zvíťazí`**.
- U `027` byl odstavec `Náš obrázek je…` odstraněn z duplicitní sekce popisku; zůstává jednou v hlavním textu, kam podle sazby patří.
- U `004` byl potvrzen veškerý zachovaný text, ale výsledkový blok končí mimo spodní okraj snímku. Chybějící pokračování je evidováno jako `URB-U-0032`.
- `001`, `010`, `011` a `014` byly potvrzeny bez textové změny.

Celkem druhou kontrolou prošlo **15 zdrojových položek**. Stav `visually_verified` má 13 položek, `004` má `visually_verified_with_lacuna` a `009` sloužilo pouze jako kontrolní detail.

## Registr nejistot

- `open`: 23
- `deferred`: 3
- `resolved`: 5
- `not_actionable`: 1
- celkem: 32

Otevřené položky Ochotníků: `URB-U-0024` až `URB-U-0032`. Nová `URB-U-0032` se týká oříznutého výsledkového bloku v článku `004`.

## Následující krok

Provést druhou kontrolu:

1. dvoustránkového článku z časopisu Těšínsko (`028` + `019`);
2. všech samostatných textových jednotek z knižních stran 40–45 (`017`, `016`, `015`);
3. nativně vytěženého dokumentu DOC `061` proti jeho vizuálnímu vykreslení.

Zachovat otevřené rozpory `URB-U-0028` a `URB-U-0029`; fyzické hranice článků neslučovat a stav nativního DOC změnit teprve po porovnání s vykreslenou stránkou.
