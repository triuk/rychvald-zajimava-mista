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

Audity `Thumbs.db` prokázaly **12 chybějících plných originálů**. Příslušné samostatné soubory v repozitáři nejsou; zachovány jsou pouze jejich náhledy v cache:

| Kolekce | Počet chybějících plných originálů | Poznámka |
|---|---:|---|
| Rychvaldské větrné mlýny | 1 | `P1010269.JPG` |
| Články z Českého slova | 8 | historické názvy a náhledy jsou v samostatném reportu |
| Ochotníci rychvald | 2 | `img387.jpg` a stránka `ochotnicke divadlo 2xxx.jpg` |
| fotodokument/den po dešti | 1 | `P1020841.JPG` |
| Nálet na Ostravu 1944 | 0 | čtyři další názvy jsou pouze alternativními verzemi dochovaných snímků |
| **Celkem** | **12** | náhledy nejsou náhradou plných originálů |

Absence samostatného plného souboru je evidenční výsledek, nikoli otevřená otázka. Samostatně mohou zůstat otevřené pouze otázky identifikace, datace, lokalizace nebo interpretace zachovaného náhledu.

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

Autoritativní index je `research/urbanek-archive/uncertainties/index.yml`; úplné záznamy jsou v odkazovaných shard souborech. Původní `research/urbanek-archive/uncertainties.yml` je pouze historický snapshot.

- `open`: 18;
- `deferred`: 0;
- `resolved`: 16;
- `not_actionable`: 1;
- celkem: 35.

Technické položky `URB-U-0001`, `URB-U-0024`, `URB-U-0033` a `URB-U-0035` jsou uzavřeny. Položky `URB-U-0002`, `URB-U-0012`, `URB-U-0025` a `URB-U-0034` jsou rovněž uzavřeny: příslušné plné originály chybějí.

`URB-U-0004` je uzavřena: uživatel potvrdil, že všechny tři fotografie zachycují stejný objekt. Adresní místo Potoční 564 bylo ověřeno ve veřejných datech; přímé přiřazení konkrétní kůlny k adrese je `partially_verified`, protože nebyla nalezena nezávislá veřejná fotografie objektu.

`URB-U-0005` je uzavřena: uživatel potvrdil označení větrný mlýn u Hebdy a funkční spojení větrného kola s mlecím soustrojím. Kandidátní poloha Polní 1275, Rychvald je `partially_verified` podle dlouhodobé veřejné vazby Lumíra Hebdy k této adrese; přímý veřejný doklad samotného mlýna na adrese nalezen nebyl.

## Připravenost větve

Pilotní větev má kompletní evidovanou souborovou sadu. Zbývají tyto věcné výhrady:

1. dvanáct plných originálů chybí; v `Thumbs.db` jsou zachovány pouze jejich náhledy;
2. otevřené historické, identifikační a fyzické lakuny jsou vedeny v aktuálním registru;
3. názvy složek a souborů nejsou samy o sobě považovány za nezávislý historický důkaz;
4. před použitím konkrétního tvrzení v článku je nutné citovat příslušný zdrojový soubor a případně další ověřovací pramen.

Doporučený stav: `draft_pr_open_with_complete_pilot_file_set`.
