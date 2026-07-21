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
- První textový průchod všech plánovaných zdrojů je dokončen.
- Plán: `research/urbanek-archive/collections/ochotnici-rychvald-processing-plan.yml`.

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

Opravy: `Rudolf Debnárik` → `Rudolf Děbnárik`, `zvýťazí` → `zvíťazí` a odstranění strukturální duplicity u `027`. Lakuna výsledkového bloku `004` zůstává jako `URB-U-0032`.

### Dávka 03 — Těšínsko, knižní strany 40–45 a DOC

Protokol:

`research/urbanek-archive/collections/ochotnici-rychvald-visual-review-03.yml`

Zkontrolováno 6 zdrojových položek v 6 textových výstupech:

- `028` + `019` — `Z dějin ochotnického divadla v Rychvaldě`: `visually_verified`;
- `017` — `Založení tělocvičné jednoty „Sokol“ v Rychvaldě`: `visually_verified`;
- `017` + `016` + `015` — `Vzpomínky na Rychvald za války`: `visually_verified`;
- `015` — `Episody při sčítání lidu 1910`: `visually_verified`;
- `015` — začátek `Hospodářského přehledu`: `visually_verified_with_lacuna`;
- `061` — nativní DOC `112 let ochotnických souborů v Rychvaldu`: `native_extracted_visually_verified`.

Opravy a potvrzení dávky 03:

- `Třasořítka` → **`Třasořitka`**;
- `maskování` → **`maskovaní`**;
- doplněny závěrečné tečky dvou vytištěných nadpisů;
- nativní DOC se ve slovech a interpunkci shoduje s vykreslenou stránkou; normalizovány byly pouze technické vícenásobné mezery;
- LibreOffice vykreslil jednu obsahovou a jednu prázdnou stránku, přestože metadata uvádějí jednu stranu;
- tištěná podoba `Ofélie` zůstává v rozporu s programovou `Olivií` (`URB-U-0028`);
- chybějící strana pokračování `Hospodářského přehledu` zůstává `URB-U-0029`.

Celkem druhou kontrolou prošlo **21 zdrojových položek**.

## Registr nejistot

- `open`: 23
- `deferred`: 3
- `resolved`: 5
- `not_actionable`: 1
- celkem: 32

Otevřené položky Ochotníků: `URB-U-0024` až `URB-U-0032`.

## Následující krok

Provést zvětšenou druhou kontrolu rukopisných zdrojů:

1. kronikové strany 260–262 (`008`, `007`, `006`; `005` pouze jako kontrolní detail strany 262);
2. obě části rukopisného přehledu Miroslava Neboráka (`003`).

Řešit pouze podoby doložené rukopisem nebo dalším archivním dokumentem. Opravdově nečitelné výrazy a rozpor mezi datací listu a položkami roku 1961 ponechat otevřené jako `URB-U-0030` a `URB-U-0031`.
