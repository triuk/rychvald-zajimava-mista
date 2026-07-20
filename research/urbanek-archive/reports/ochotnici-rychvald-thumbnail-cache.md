# Audit `Thumbs.db` – Ochotníci rychvald

## Zdroj a metoda

- Původní cesta na Google Drivu: `Ochotníci rychvald/Thumbs.db`
- Velikost: 366 080 B
- SHA-256: `61a49eda18010a9b66e9bf43a5f039d81cedb3ff8e44597306c75b1b54fa5ecd`
- Stav v GitHubu: `drive_listed_repo_missing`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**

Soubor byl načten jako Microsoft Compound File Binary. Katalogové záznamy byly propojeny s jednotlivými streamy a JPEG náhledy byly porovnány podle dekódovaných obrazových pixelů, nikoli pouze podle názvu souboru.

## Souhrn

- katalogových záznamů: **93**;
- z toho názvů obrazových souborů: **92**;
- systémových záznamů složky: **1**;
- současných JPEGů v kolekci: **60**;
- současných JPEGů nalezených také v cache: **60**;
- unikátních dekódovaných náhledů: **63**;
- unikátních náhledů odpovídajících současným JPEGům: **60**;
- systémových koláží složky: **1**;
- dodatečných unikátních obrazů bez současného plného souboru: **2**.

Cache tedy potvrzuje všechny současné JPEGy. Jeden název se liší pouze velikostí písmene ve slově `Jaromír` / `jaromír`. Dalších 29 historických nebo pracovních názvů sdílí přesně stejný dekódovaný náhled s některým současným souborem a představuje převážně přejmenování nebo meziverze.

## Dodatečné unikátní obrazy

| Historický název | Rozměr náhledu | JPEG SHA-256 | Bezpečný vizuální popis |
|---|---:|---|---|
| `img387.jpg` | 96 × 66 | `a73484c26a7e6b516a7c09d14d299b7f1962c6e731e5c8a50f47f2d79498753a` | Historická skupinová fotografie dospělých a dětí, pravděpodobně před budovou nebo stěnou. Osoby, událost a datum nelze z malého náhledu bezpečně určit. |
| `ochotnicke divadlo 2xxx.jpg`; `ochotnicke divadlo 2xxxaa.jpg` | 94 × 96 | `eb6411aaa981b3a4a7b72ee0f7423ae8f1e6b3890570933bf18d5fe7e19bff23` | Reprodukce tištěné stránky nebo článku s několika textovými bloky a fotografií účinkujících. Oba názvy mají totožný náhled. Rozlišení nestačí k spolehlivému OCR. |

## Systémový záznam

Záznam `{A42CD7B6-E9B9-4D02-B7A6-288B71AD28BA}` obsahuje náhledovou koláž několika fotografií na ikoně složky. Nejde o samostatnou archivní fotografii a není započítán mezi chybějící originály.

## Příklady potvrzených přejmenování

- `img070.jpg` → `Divadelní soubor Osvět. besedy.jpg`
- `img071.jpg` → `Zabloudil Pešková.jpg`
- `img231.jpg` → `Zabloudil.jpg`
- `img232.jpg` → `Peška.jpg`
- `img233.jpg` → `Zabloudil Suider.jpg`
- `P1020782.JPG`, `P1020782aaa.jpg` a `Z výstavky v kulturáku.jpg` → `Z výstavky v kulturáku 1.jpg`
- `P1020783.JPG` a `P1020783aa.jpg` → `Z výstavky 2.jpg`
- `ocenenixxxaaaa.jpg` → `ocenění.jpg`
- `uznanixxxx.jpg` → `četné uznání.jpg`
- `album.jpg` a `albumxxxxaaaa.jpg` → `Z danního tisku.jpg`
- `clen souboruxxxx.jpg` → `Seznam her v nichž hrál M. Neborák.jpg`
- `posledni noc v rocexxxaaa.jpg` → `posledni noc  program.jpg`

Úplné mapování je možné kdykoli znovu odvodit z cache podle pixelových hashů; v tomto reportu jsou uvedeny pouze reprezentativní příklady.

## Důsledky pro další práci

- `Thumbs.db` nesmí být smazán z původního archivu. Je jediným známým nosičem dvou dodatečných unikátních obrazů.
- Náhledy nejsou náhradou originálních souborů a nebudou použity k plnohodnotnému OCR ani k definitivní identifikaci osob.
- Při pozdějším hledání v dalších složkách nebo zálohách použít názvy `img387.jpg` a `ochotnicke divadlo 2xxx.jpg` a zároveň obrazovou podobnost.
- Chybějící binární cache v GitHubu neblokuje klasifikaci 60 současných JPEGů ani dokumentu DOC, protože audit byl proveden přímo z originálu na Drivu.
