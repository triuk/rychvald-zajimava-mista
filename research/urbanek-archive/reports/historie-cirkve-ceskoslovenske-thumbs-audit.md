# Audit `Thumbs.db` – kalendář 2015

## Rozsah

- Kolekce: `Historie Církve československé v Rychvaldě ve fotografiích`
- Technický soubor: `10 Kalendář 2015/Thumbs.db`
- Repo cesta: `sources/osobni-archiv-jaromira-urbanka/4 Historie  Církve Československé  v Rychvaldě ve fotografiích/10 Kalendář 2015/Thumbs.db`
- Původ: Z osobního archivu p. Jaromíra Urbánka.
- Práva: neznámá
- Drive ID: `1UR9-TOX20gexQsxgM_o-oFxiV4wVOEiM`
- Velikost: `70656` B
- SHA-256: `056cb436b5556dea975512e8ff00cd80ffb8eaa7ecbf7c3c4795e8f47831d037`
- Git blob SHA: `91d73b30448ce8f8aa02a8ed79dafee5d349f0c2`

## Metoda

Soubor byl porovnán mezi Google Drive a Git repozitářem, identifikován jako OLE/CFB `Thumbs.db` a rozebrán na katalog a mini-streamy. Dekódovatelné náhledy byly normalizovány na stejný rozměr a porovnány se všemi patnácti plnými kalendářovými JPEGy. Korelace v tabulce je pouze kontrolní obrazová metrika; rozhodující bylo také jednoznačné nejlepší přiřazení a vizuální kontrola.

## Struktura a integrita

- Dochovaný soubor je ve Drive i Gitu binárně totožný.
- Katalog obsahuje přesně 16 záznamů: názvy `1.jpg` až `15.jpg` a jednu interní GUID položku `{A42CD7B6-E9B9-4D02-B7A6-288B71AD28BA}`.
- GUID položka je 96 × 96 px složený náhled složky Windows; není samostatným zdrojovým obrazem.
- Katalogové časy u JPEGů jsou `2015-01-24 04:58:06` až `04:58:10`; GUID položka má `2015-01-24 12:43:38.078124`. Jde o metadata cache, nikoli o dataci historických událostí nebo vložených fotografií.
- CFB struktura odkazuje za konec dochovaného souboru: chybí jeden odkazovaný 512B MiniFAT sektor a šest 512B sektorů kořenového mini-streamu. Pro naplnění deklarovaného streamu `15.jpg` schází 2 861 B po dvanáctibajtové hlavičce náhledu; k dispozici je pouze 308B začátek JPEG dat.
- Příčina strukturální neúplnosti není z dochovaného souboru zjistitelná. Audit proto neoznačuje soubor za poškozený při přenosu; konstatuje pouze ověřitelný nesoulad v jeho uložené CFB struktuře.

## Mapování katalogu

| ID katalogu | Stream | Název | Výsledek | Korelace |
|---:|---:|---|---|---:|
| 1 | `2` | `1.jpg` | dekódován; nejlepší shoda `1.jpg` | 0.991490 |
| 2 | `3` | `2.jpg` | dekódován; nejlepší shoda `2.jpg` | 0.979011 |
| 3 | `4` | `3.jpg` | dekódován; nejlepší shoda `3.jpg` | 0.994403 |
| 4 | `5` | `4.jpg` | dekódován; nejlepší shoda `4.jpg` | 0.995051 |
| 5 | `6` | `5.jpg` | dekódován; nejlepší shoda `5.jpg` | 0.995412 |
| 6 | `7` | `6.jpg` | dekódován; nejlepší shoda `6.jpg` | 0.995324 |
| 7 | `8` | `7.jpg` | dekódován; nejlepší shoda `7.jpg` | 0.995768 |
| 8 | `9` | `8.jpg` | dekódován; nejlepší shoda `8.jpg` | 0.994220 |
| 9 | `01` | `9.jpg` | dekódován; nejlepší shoda `9.jpg` | 0.994176 |
| 10 | `1` | `10.jpg` | dekódován; nejlepší shoda `10.jpg` | 0.994650 |
| 11 | `11` | `11.jpg` | dekódován; nejlepší shoda `11.jpg` | 0.993248 |
| 12 | `21` | `12.jpg` | dekódován; nejlepší shoda `12.jpg` | 0.994834 |
| 13 | `31` | `13.jpg` | dekódován; nejlepší shoda `13.jpg` | 0.993814 |
| 14 | `41` | `14.jpg` | dekódován; nejlepší shoda `14.jpg` | 0.994842 |
| 16 | `61` | `15.jpg` | katalogován; cache JPEG neúplný (308B fragment); plný originál přítomen | — |
| 15 | `51` | `{A42CD7B6-E9B9-4D02-B7A6-288B71AD28BA}` | dekódovaný složený náhled složky Windows; není zdrojový JPEG | — |

Poznámka: pořadí ID 15 a 16 je v katalogu obrácené vůči názvům; ID 15 patří GUID položce a ID 16 souboru `15.jpg`.

## Závěr

1. Cache obsahuje názvy všech patnácti dochovaných kalendářových JPEGů a žádný další název zdrojového obrázku.
2. Čtrnáct plných cache náhledů se jednoznačně shoduje s odpovídajícími soubory `1.jpg` až `14.jpg`.
3. Záznam `15.jpg` je v katalogu přítomen, ale jeho cache stream je kvůli strukturální neúplnosti souboru nedokončený. Plný originál `15.jpg` je v kolekci přítomen a byl samostatně ověřen proti Git blob SHA.
4. Cache neposkytuje doklad žádného chybějícího plného originálu. Počet chybějících plných originálů doložených pouze touto cache je **0**.
5. Jednotlivé vložené fotografie uvnitř kalendářových stran nejsou v katalogu vedeny jako samostatné soubory. Cache proto nemění závěry o dosud nepřiřazených vložených fotografiích na stranách 191, 197 a 198.

## Omezení

Kvůli chybějícím koncovým sektorům nelze obnovit celý cache náhled `15.jpg` ani z cache určit příčinu její strukturální neúplnosti. Toto omezení nemá vliv na úplnost sady patnácti plných kalendářových JPEGů, protože jejich názvy jsou v katalogu kompletní a všechny plné soubory jsou přítomny v repozitáři.
