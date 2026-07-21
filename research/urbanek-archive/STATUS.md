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

### Dokončená dávka 01

Protokol:

`research/urbanek-archive/collections/ochotnici-rychvald-visual-review-01.yml`

Stav `visually_verified` mají:

- `032–033` — program `Večer tříkrálový`;
- `013` — program celostátní soutěže;
- `023` — čestné uznání Sylvii Kravalové;
- `039` — program `Poslední noc v roce`;
- `042` — program `Slavnost lampiónů`;
- `047` — dopis o věcné ceně.

Celkem bylo vizuálně ověřeno **7 zdrojových položek v 6 textových výstupech**.

### Opravy a potvrzení

- U programu Večera tříkrálového bylo společné označení `ve službách vévodových` odděleno od Valentina a vedeno jako společný údaj Valentina a Curia.
- Na plakátu celostátní soutěže byl chybný přepis `KLÍPERA` opraven na tištěné `KLICPERA`.
- Dekorativní symboly mezi městy na čestném uznání jsou vedeny jako ornamenty, ne jako textové odrážky.
- Číslo jednací dopisu bylo potvrzeno jako `9272/60-sl.` a datum jako `23.6.1960`.
- Programy `Poslední noc v roce` a `Slavnost lampiónů` neobsahovaly textovou chybu prvního přepisu.
- Rukopisné podpisy na čestném uznání nebyly doplněny odhadem.

## Registr nejistot

- `open`: 22
- `deferred`: 3
- `resolved`: 5
- `not_actionable`: 1
- celkem: 31

Otevřené položky Ochotníků: `URB-U-0024` až `URB-U-0031` podle registru. Rozpor v obsazení Fabiana (`URB-U-0026`) zůstává otevřený.

## Následující krok

Provést druhou řádkovou kontrolu skupiny **Kroměříž 1960**:

1. `001` — `Vesničtí ochotníci ve finále`;
2. `004` — `Thálie držela palce`;
3. `010` — `Katka, Angelika a Viola v Kroměříži`, s `009` pouze jako kontrolním detailem;
4. `011` — první kroměřížská novinová stránka;
5. `012` — stránka s článkem `Rychvald a Shakespeare v Kroměříži`;
6. `014` — `Vesničtí ochotníci se představují`;
7. `027` — `Jaké jsou naše vesnické soubory?`.

Každý článek a každý fotografický popisek musí být porovnán se zdrojovým obrazem po řádcích. Stav `visually_verified` se přidá pouze po úplné kontrole.
