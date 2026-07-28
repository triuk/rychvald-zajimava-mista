# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdrojový kořen: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt bylo potvrzeno.
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.
- Autoritativním pracovním úložištěm je Git repozitář.

## Draft pull request

- PR: [#1 – Import and classify Jaromír Urbánek archive (pilot + CČS batch)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

## Dokončený pilot

| Kolekce | Obsahové soubory | Technické soubory | Celkem | Stav |
|---|---:|---:|---:|---|
| Rychvaldské větrné mlýny | 31 | 8 | 39 | dokončeno |
| Články z Českého slova | 37 | 2 | 39 | dokončeno |
| Ochotníci rychvald | 61 | 2 | 63 | dokončeno |
| fotodokument/den po dešti | 8 | 2 | 10 | dokončeno |
| Nálet na Ostravu 1944 | 7 | 1 | 8 | dokončeno |
| **Celkem** | **144** | **15** | **159** | **159 z 159 položek přítomno** |

Audity pilotních cache prokázaly **11 chybějících plných originálů** dochovaných pouze jako náhledy.

## Kolekce historie Církve československé

Kolekce: `4 Historie  Církve Československé  v Rychvaldě ve fotografiích`

- 10 tematických podsložek;
- 200 JPEGů;
- 1 technický soubor `Thumbs.db`;
- celkem 201 položek;
- stav: `processing_in_progress`.

Dokončeno je třicet osm dávek po pěti snímcích, tedy `urbanek-ccs-001` až `190`.

- zpracováno: **190 z 201 položek**;
- proti Git blob SHA ověřeno: **190 položek**;
- vizuálně klasifikováno: **190 položek**;
- zdrojově indexováno: **190 položek**;
- zbývá: **11 položek**.

### Zjištění dávky 38

Dávka 38 zahájila podsložku `10 Kalendář 2015` a zpracovala titulní stranu, historický souhrn a měsíce leden až březen.

- `urbanek-ccs-186` je titulní strana s rokem 2015, textem „90 let Husova sboru a 95 let Církve československé v Rychvaldu“, současným exteriérem sboru, znakem kalicha s křížem a detailem kamene s číselným údajem.
- `urbanek-ccs-187` je textová strana `1920–2015` s historickým souhrnem založení obce, stavby, výzdoby, období okupací, poválečných úprav, zvonů, farářů a kulturních aktivit. Jde o čitelný sekundární text; jeho historická tvrzení nebyla touto dávkou nezávisle potvrzena.
- `urbanek-ccs-188` je lednová strana. Vizuálně znovu používá fotografie `urbanek-ccs-001`, `003` a `006`.
- `urbanek-ccs-189` je únorová strana. Vizuálně znovu používá fotografie `urbanek-ccs-007`, `008`, `009` a `013`.
- `urbanek-ccs-190` je březnová strana. Vizuálně znovu používá fotografie `urbanek-ccs-037`, `038` a `039`.
- Kalendářové reprodukce jsou další sazební použití už evidovaných snímků, nikoli nové nezávislé obrazové doklady.
- Všech pět souborů má odlišné Git blob SHA, rozměr 2385 × 3354 pixelů a barevný režim CMYK.
- EXIF `Artist` a `XPAuthor` ve všech pěti souborech uvádějí řetězec `Marta`; použitelné embedded datum chybí. Samotný řetězec nepotvrzuje úplnou identitu ani autorství.
- Dávka přidala nové ID `URB-U-0073`.

Pracovní soubory dávky 38:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-38.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-38.yml`;
- `sources/index.d/urbanek-ccs-38.yml`;
- nový záznam `research/urbanek-archive/uncertainties/open-20.yml`;
- aktualizovaný `research/urbanek-archive/uncertainties/index.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 39;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 73.

`URB-U-0073` sleduje autorství, vydavatele, zdrojovou bibliografii, původ a úpravy vložených fotografií, historickou správnost textu a popisků a práva ke kalendáři 2015. Kalendář je sekundární kompilace; viditelné texty potvrzují znění stránky, nikoli automaticky popisované události.

EXIF jméno, kalendářový popisek, moderní historický souhrn ani znovu použitá fotografie samy neurčují autora, vydavatele, původní zdroj nebo historickou správnost tvrzení.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 190 zpracovaných a 11 zbývajících položek;
- registr používá součty 39/31/3/73;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-191` až `urbanek-ccs-195`.
- Očekávané názvy v podsložce `10 Kalendář 2015`: `6.jpg`, `7.jpg`, `8.jpg`, `9.jpg` a `10.jpg`.
- `Thumbs.db` v téže podsložce musí být před uzavřením kolekce samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
