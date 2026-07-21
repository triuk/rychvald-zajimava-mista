# Reconciliace pilotního zpracování archivu Jaromíra Urbánka

## Rozsah pilotu

Původ: **Z osobního archivu p. Jaromíra Urbánka.**

| Kolekce | Obsahové soubory | Technické soubory | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | klasifikace a první OCR dokončeny |
| Články z Českého slova | 37 | 2 | 39 | OCR i druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | 61 | 2 | 63 | klasifikace, textový průchod i druhá kontrola dokončeny |
| fotodokument/den po dešti | 8 | 2 | 10 | audit a vizuální klasifikace dokončeny; OCR není potřebný |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | audit a vizuální klasifikace dokončeny; OCR není potřebný |
| **Celkem** | **144** | **15** | **159** | |

## Stav souborů ve větvi

- Všech **144 obsahových souborů** je ve větvi pod přesnou původní cestou a názvem.
- Z 15 technických souborů je ve větvi přítomno 6 a chybí 9 souborů `Thumbs.db`.
- Celkem je tedy ve větvi přítomno **150 z 159** položek evidovaných na Drivu.
- Chybějící technické soubory jsou zachovány na Google Drivu, byly auditovány přímo z originálu a jsou vedeny jako odložené položky registru nejistot.

### Chybějící technické cache

- 5× `Thumbs.db` v kolekci Rychvaldské větrné mlýny;
- 1× `Thumbs.db` v kolekci Články z Českého slova;
- 1× `Thumbs.db` v kolekci Ochotníci rychvald;
- 1× `Thumbs.db` v kolekci fotodokument/den po dešti;
- 1× `Thumbs.db` v kolekci Nálet na Ostravu 1944.

## Obrazy známé pouze z cache

Audity `Thumbs.db` zachytily plné originály, které v současných složkách nejsou:

| Kolekce | Počet unikátních chybějících obrazů | Poznámka |
|---|---:|---|
| Rychvaldské větrné mlýny | 1 | `P1010269.JPG` |
| Články z Českého slova | 8 | historické názvy a náhledy jsou v samostatném reportu |
| Ochotníci rychvald | 2 | `img387.jpg` a stránka `ochotnicke divadlo 2xxx.jpg` |
| fotodokument/den po dešti | 1 | `P1020841.JPG` |
| Nálet na Ostravu 1944 | 0 | čtyři další názvy jsou pouze alternativními verzemi dochovaných snímků |
| **Celkem** | **12** | náhledy nejsou náhradou plných originálů |

## Zpracování textu

### Články z Českého slova

- 37 obrazových položek bylo seskupeno podle fyzické sazby.
- První OCR a druhá řádková kontrola jsou dokončeny.
- Fyzické lakuny, chybějící výstřižky a neidentifikované fragmenty zůstávají v registru nejistot.

### Ochotníci rychvald

- Byly vytěženy všechny plánované dokumentové a scénické texty.
- Druhou vizuální kontrolou prošlo 29 zdrojových položek v pěti dávkách.
- Nativní DOC byl porovnán s vizuálním vykreslením.
- Rukopisná kronika a přehled Miroslava Neboráka byly znovu kontrolovány ve zvětšení.
- Otevřené věcné rozpory se nepovažují za chyby OCR a zůstávají v registru.

### Ostatní kolekce

- Rychvaldské větrné mlýny obsahují dva textové dokumenty s prvním přepisem; převážná část kolekce je fotografická.
- `den po dešti` a `Nálet na Ostravu 1944` neobsahují text vyžadující samostatný OCR.

## Registr nejistot

Po dokončení pilotních kolekcí:

- `open`: 23;
- `deferred`: 5;
- `resolved`: 6;
- `not_actionable`: 1;
- celkem: 35.

Otevřené položky jsou dohledatelné podle stabilních ID `URB-U-XXXX`. Nevyřešená skutečnost nesmí být v článku prezentována jako ověřená.

## Připravenost větve

Pilotní větev je připravena pro **draft pull request** s těmito výhradami:

1. devět technických souborů `Thumbs.db` není fyzicky ve větvi, ale je auditováno z Drivu;
2. dvanáct unikátních obrazů je známo pouze jako náhled bez plného originálu;
3. otevřené historické, identifikační a fyzické lakuny jsou vedeny v `uncertainties.yml`;
4. názvy složek a souborů nejsou samy o sobě považovány za nezávislý historický důkaz;
5. před použitím konkrétního tvrzení v článku je nutné citovat příslušný zdrojový soubor a případně další ověřovací pramen.

Doporučený stav: `ready_for_draft_pr_with_known_deferred_technical_files`.
