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
| **Celkem** | **144** | **15** | **159** | **všechny položky přítomny** |

## Stav souborů ve větvi

- Všech **144 obsahových souborů** je ve větvi pod přesnou původní cestou a názvem.
- Všech **15 technických souborů** je ve větvi pod přesnou původní cestou a názvem.
- Celkem je ve větvi přítomno **159 z 159** evidovaných položek.
- Commit `7e6483d1bcb92034bea6eddd43fd55869dedce9c` doplnil chybějící technické cache a odstranil jejich ignorování.
- U devíti dříve chybějících pilotních položek byla po commitu ověřena přesná cesta a Git blob SHA.

### Doplněné technické cache

- 5× `Thumbs.db` v kolekci Rychvaldské větrné mlýny;
- 1× `Thumbs.db` v kolekci Články z Českého slova;
- 1× `Thumbs.db` v kolekci Ochotníci rychvald;
- 1× `Thumbs.db` v kolekci fotodokument/den po dešti;
- 1× `Thumbs.db` v kolekci Nálet na Ostravu 1944.

## Chybějící plné originály

Audity `Thumbs.db` prokázaly **11 chybějících plných originálů**. Příslušné samostatné soubory v repozitáři nejsou; zachovány jsou pouze jejich náhledy v cache:

| Kolekce | Počet chybějících plných originálů | Poznámka |
|---|---:|---|
| Rychvaldské větrné mlýny | 0 | `P1010269.JPG` je duplicitní náhled dochovaného souboru |
| Články z Českého slova | 8 | historické názvy a náhledy jsou v samostatném reportu |
| Ochotníci rychvald | 2 | `img387.jpg` a stránka `ochotnicke divadlo 2xxx.jpg` |
| fotodokument/den po dešti | 1 | `P1020841.JPG` |
| Nálet na Ostravu 1944 | 0 | čtyři další názvy jsou pouze alternativními verzemi dochovaných snímků |
| **Celkem** | **11** | náhledy nejsou náhradou plných originálů |

Absence samostatného plného souboru je evidenční výsledek, nikoli otevřená otázka. Samostatně mohou zůstat otevřené pouze otázky identifikace, datace, lokalizace nebo interpretace zachovaného náhledu.

## Zpracování textu

### Články z Českého slova

- 37 obrazových položek bylo seskupeno podle fyzické sazby.
- První OCR a druhá řádková kontrola jsou dokončeny.
- Fyzické a ořezové lakuny jsou výslovně označeny; pouze ty, u nichž zůstává aktivní badatelský úkol, se vedou jako otevřené nejistoty.

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

Autoritativní index je `research/urbanek-archive/uncertainties/index.yml`; úplné záznamy jsou v odkazovaných shard souborech. Původní `research/urbanek-archive/uncertainties.yml` je pouze historický snapshot.

- `open`: 12;
- `deferred`: 0;
- `resolved`: 24;
- `not_actionable`: 2;
- celkem: 38.

Technické položky `URB-U-0001`, `URB-U-0024`, `URB-U-0033` a `URB-U-0035` jsou uzavřeny. Položky `URB-U-0002`, `URB-U-0012`, `URB-U-0025` a `URB-U-0034` jsou rovněž uzavřeny: příslušné plné originály chybějí.

`URB-U-0004` je uzavřena jako `verified`: databáze Povětrník záznam 176 (mlýnek 49) uvádí Potoční 564 a její základní fotografie je oříznutou verzí archivního souboru `Potoční 564.jpg`.

`URB-U-0005` je uzavřena jako `verified`: databáze Povětrník záznam 175 (mlýnek 48) uvádí U Skučáku 54 a její základní fotografie zachycuje stejný stožár, budovu a okolí jako archivní snímky. Dřívější inference Polní 1275 je překonaná.

`URB-U-0007` je uzavřena pouze pro identitu historického obrazu jako Kakalův mlýn. Přesná poloha, číslo domu, vlastník, datace a technologie jsou vedeny v propojené otevřené položce `URB-U-0036`, která se musí znovu prověřovat po zpracování dalších relevantních pramenů.

`URB-U-0009` je uzavřena pro identitu fotografie jako interiér kostela sv. Anny v Rychvaldě. Význam čísla `304` a vztah ke složce Kakalova mlýna jsou vedeny v propojené otevřené položce `URB-U-0037`.

`URB-U-0010` je uzavřena pro dokumentační vztah náčrtu a fotografií k jednomu zařízení. Přesná historická poloha mlýnku označeného jako zařízení za domem č. 339 zůstává v propojené otevřené položce `URB-U-0038`.

`URB-U-0011` je uzavřena jako chybně zařazená přesná kopie obrazu Kakalova mlýna. Nezachycuje mlýnek za domem č. 339 a soubor se nepoužívá jako doklad k tomuto zařízení; původní archivní cesta zůstává zachována.

`URB-U-0017` je `not_actionable`: spodní okraj předchozího článku je na fotografii `9.jpg` pouze vedlejším obsahem mimo rozsah cílového výstřižku a dále se neidentifikuje ani nepřepisuje.

`URB-U-0020` je uzavřena jako známá fyzická lakuna bez dalšího badatelského úkolu. Veškerý zachovaný text byl přepsán a chybějící úsek zůstává výslovně označen bez odhadované rekonstrukce.

`URB-U-0021` je uzavřena jako známá ořezová lakuna. Archivní fotografie zachycuje pouze horní část novinové strany; chybějící spodní části sloupců zůstávají výslovně označeny a nejsou rekonstruovány.

## Připravenost větve

Pilotní větev má kompletní evidovanou souborovou sadu. Zbývají tyto věcné výhrady:

1. jedenáct plných originálů chybí; v `Thumbs.db` jsou zachovány pouze jejich náhledy;
2. otevřené historické, identifikační a fyzické lakuny jsou vedeny v aktuálním registru;
3. názvy složek a souborů nejsou samy o sobě považovány za nezávislý historický důkaz;
4. před použitím konkrétního tvrzení v článku je nutné citovat příslušný zdrojový soubor a případně další ověřovací pramen;
5. další větrné mlýny se před uzavřením identifikace porovnávají také s databází Povětrník;
6. `URB-U-0036` zůstává aktivní, dokud nové prameny nepotvrdí nebo nevyvrátí polohu a historii Kakalova mlýna.

Doporučený stav: `draft_pr_open_with_complete_pilot_file_set`.
