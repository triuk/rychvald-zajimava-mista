# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový kořen: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt bylo potvrzeno.
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Autoritativním pracovním úložištěm je Git repozitář.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties/index.yml` včetně odkazovaných shard souborů, `reports/pilot-reconciliation.md` a kolekční přehledy v `collections/`.

## Draft pull request

- PR: [#1 – Import and classify Jaromír Urbánek archive (pilot + CČS batch)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

## Dokončený pilot

| Kolekce | Obsahové soubory | Technické soubory | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | klasifikace a první OCR dokončeny |
| Články z Českého slova | 37 | 2 | 39 | OCR a druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | 61 | 2 | 63 | textový průchod a druhá vizuální kontrola dokončeny |
| fotodokument/den po dešti | 8 | 2 | 10 | audit a vizuální klasifikace dokončeny |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | audit a vizuální klasifikace dokončeny |
| **Celkem** | **144** | **15** | **159** | **159 z 159 položek přítomno** |

Audity pilotních cache prokázaly **11 chybějících plných originálů**. Náhled v `Thumbs.db` není náhradou plného originálu.

## Nová dávka – historie Církve československé

Kolekce: `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`

- 10 tematických podsložek;
- 200 JPEGů;
- 1 technický soubor `Thumbs.db`;
- celkem 201 položek;
- stav: `processing_in_progress`;
- pilotní součty se touto dávkou nemění.

Dokončeno je dvacet tři dávek po pěti snímcích, tedy `urbanek-ccs-001` až `115`.

Dosavadní stav nové kolekce:

- zpracováno: **115 z 201 položek**;
- proti Git blob SHA ověřeno: **115 položek**;
- vizuálně klasifikováno: **115 položek**;
- zdrojově indexováno: **115 položek**;
- zbývá: **86 položek**.

### Zjištění dávky 23

Dávka 23 pokračuje v podsložce `5 Kaple CČS na Ostravici`.

- `urbanek-ccs-111` obsahuje čitelný vložený popisek „Uvítání br.biskupa správcem Husitské kaple“. Obraz zachycuje tři muže, kytici a ústředního duchovního s řetězem nebo insignií; identity a funkce nejsou samostatně ověřeny.
- `urbanek-ccs-112` obsahuje čitelný popisek „Záběr z bohoslužeb“ a zachycuje početný dav před otevřeným vstupem kaple, v němž je viditelný oltář nebo liturgický stůl se svícny.
- `urbanek-ccs-113` zachycuje starou subtilní dřevěnou věžovou konstrukci. V horní části je viditelný zavěšený zvon nebo zřetelně zvonovitý předmět; pod zvonicí stojí dav.
- `urbanek-ccs-114` a `115` zachycují tutéž novou dřevěnou zvonici se čtyřmi masivními sloupy, širokou stříškou, zavěšeným zvonem a vysokou kovovou tyčí s kruhovým symbolem.
- Archivní název `114` tvrdí, že stará zvonice byla roku 2016 demontována a nahrazena novou. EXIF obou moderních snímků uvádí pořízení 2. října 2016 v časech 14:04:23 a 14:05:02. To podporuje existenci nové konstrukce k tomuto dni, nikoli přesné datum demontáže, stavby nebo předání.
- Dávka nepřidala nové ID a rozšířila `URB-U-0069` a `URB-U-0070`.

Pracovní soubory dávky 23:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-23.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-23.yml`;
- `sources/index.d/urbanek-ccs-23.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-17.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 36;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 70.

Dávka 23 nepřidala nové ID. `URB-U-0069` nyní zahrnuje obrazovou posloupnost staré a nové zvonice, viditelné zvony, tvrzení o výměně roku 2016, EXIF dataci nové konstrukce a otázku případného přenesení původního zvonu. `URB-U-0070` byla rozšířena o správce Husitské kaple a záběr z bohoslužeb.

EXIF datum může podporovat, že objekt existoval v okamžiku pořízení fotografie; samo neprokazuje datum stavby, demontáže nebo vysvěcení.

## Kontrola konzistence draftu

- pilot a nová dávka jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají stejný rozsah nové dávky: 200 + 1 = 201;
- aktuální průběžný stav je 115 zpracovaných a 86 zbývajících položek;
- registr používá součty 36/31/3/70;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová dávka: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-116` až `urbanek-ccs-120`.
- Očekávané archivní názvy v podsložce `5 Kaple CČS na Ostravici`: `8c.jpg`, `IMG_20161002_140624.jpg`, `IMG_20161002_140644.jpg`, `IMG_20161002_140659.jpg` a `9  biskup dr Horský v r. 1945 - 1946.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení, dokud nová dávka nebude dokončena nebo z rozsahu PR výslovně oddělena.
