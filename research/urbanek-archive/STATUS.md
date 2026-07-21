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
| Ochotníci rychvald | **první textový průchod i druhá vizuální kontrola dokončeny** |
| fotodokument/den po dešti | následuje inventář |
| Nálet na Ostravu 1944 | čeká |
| Pull request | čeká |

## Ochotníci rychvald – uzavřený stav zpracování

- Inventář: 63 položek — 60 JPEG, 1 DOC a 2 technické cache.
- Ve větvi je 62 položek; chybí pouze technický `Thumbs.db`.
- Všech 63 položek bylo klasifikováno nebo technicky auditováno.
- První textový průchod všech plánovaných zdrojů je dokončen.
- Druhou vizuální kontrolou prošlo **29 zdrojových položek** v pěti dávkách.
- Protokoly: `ochotnici-rychvald-visual-review-01.yml` až `05.yml`.
- Plán: `research/urbanek-archive/collections/ochotnici-rychvald-processing-plan.yml`.

### Dávka 01 — krátké strukturované dokumenty

Ověřeny programy `Večer tříkrálový`, celostátní soutěž, `Poslední noc v roce`, `Slavnost lampiónů`, čestné uznání a úřední dopis. Důležité opravy: `KLICPERA`, číslo jednací `9272/60-sl.` a správné strukturální přiřazení údaje `ve službách vévodových`.

### Dávka 02 — Kroměříž 1960

Ověřeno sedm textových výstupů. Opravy: `Rudolf Děbnárik`, `zvíťazí` a odstranění strukturální duplicity u `027`. Článek `004` zůstává `visually_verified_with_lacuna`, protože výsledkový blok je oříznut.

### Dávka 03 — Těšínsko, knižní strany 40–45 a DOC

Opravy `Třasořitka` a `maskovaní`; ověřeny všechny samostatné textové jednotky i nativní DOC. Rozpor `Ofélie/Olivie` a chybějící pokračování `Hospodářského přehledu` zůstávají v registru.

### Dávka 04 — rukopisná kronika a přehled Miroslava Neboráka

Kronikové strany 260–262 mají stav `visually_verified_handwriting`. Druhá kontrola určila mimo jiné podoby:

- `z okna přesunovány`;
- `zkusil své štěstí`;
- `rojili se`;
- `Wölflovy`;
- `Šílec`;
- `Otílie Bayerová (prov. Hlausová)`;
- `Löwenberger`.

`URB-U-0030` je vyřešena.

U přehledu Miroslava Neboráka byly ověřeny názvy, autoři, role, součty 38 her a 110 představení i podpis `M. Neborák`. Otevřený zůstává pouze rozpor `URB-U-0031`: list je datován 29. února 1960, ale obsahuje dva řádky označené rokem 1961.

### Dávka 05 — scénický text

Historická fotografie z roku 1923:

- `DIV-KROUŽEK`;
- `I. odb.`;
- `S.M.O.L.`;
- `v Rychvaldě`;
- `1923`;
- `ATELIER KRIŠKOVSKÝ / RADVANICE.`

Na festivalovém plakátu byly opraveny podoby:

- `II. FESTIVAL` → **`I. FESTIVAL`**;
- `ZK Dolu Dolní Suchá` → **`ZK Dukla, Dolní Suchá`**.

Zakrytý text za kovovými nosníky nebyl rekonstruován a vložené články nebyly duplicitně OCRovány.

## Registr nejistot

- `open`: 22
- `deferred`: 3
- `resolved`: 6
- `not_actionable`: 1
- celkem: 32

Otevřené položky kolekce Ochotníci: `URB-U-0024`, `0025`, `0026`, `0027`, `0028`, `0029`, `0031` a `0032`. Jde o chybějící soubory, věcné rozpory, dataci nebo fyzické lakuny — nikoli o nedokončenou druhou kontrolu OCR.

## Následující přesný krok

Zahájit kolekci `fotodokument/den po dešti`:

1. vypsat všechny přímé položky a podsložky na Google Drivu;
2. přiřadit stabilní ID;
3. označit technické cache;
4. ověřit přesné cesty ve větvi;
5. nezahajovat OCR ani výběr fotografií, dokud není známá struktura kolekce.
