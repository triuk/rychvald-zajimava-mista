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

Dokončeno je třicet devět dávek po pěti snímcích, tedy `urbanek-ccs-001` až `195`.

- zpracováno: **195 z 201 položek**;
- proti Git blob SHA ověřeno: **195 položek**;
- vizuálně klasifikováno: **195 položek**;
- zdrojově indexováno: **195 položek**;
- zbývá: **6 položek**.

### Zjištění dávky 39

Dávka 39 pokračovala v podsložce `10 Kalendář 2015` a zpracovala měsíce duben až srpen.

- `urbanek-ccs-191` je dubnová strana se zvony, reliéfním rokem `1920` a veřejnou prohlídkou věže. Znovu používá zvonové podklady položek `014` a `015`; fotografii návštěvníků u zvonu se nepodařilo bezpečně přiřadit k dřívější samostatné položce.
- `urbanek-ccs-192` je květnová strana se sbory a znovu používá položky `040`, `042` a `043`. Popisky sekundárně uvádějí rok 1933, Šlachtu, Vodičku a vánoční koncert se sbormistrem Dajčem roku 1990.
- `urbanek-ccs-193` je červnová strana se skupinami prvního přijímání a znovu používá položky `011`, `012` a `032`. Popisky uvádějí chlapce roku 1930 a další skupinu přibližně roku 1950.
- `urbanek-ccs-194` je červencová strana husovské připomínky a znovu používá položky `050`, `053` a `054`. Text tvrdí založení tradice roku 1926 a každoroční růst účasti.
- `urbanek-ccs-195` je srpnová strana se svatbou, křtem a přijímáním a znovu používá položky `023`, `048` a `036`. Popisky uvádějí roky 1948, 1970 a 1987 a jméno Mgr. Jany Šilerové.
- Kalendářové datace, jména a historické výroky jsou sekundární popisky, nikoli nezávislé potvrzení.
- Všech pět souborů má odlišné Git blob SHA, rozměr 2385 × 3354 pixelů a barevný režim CMYK.
- EXIF `Artist` a `XPAuthor` ve všech pěti souborech uvádějí řetězec `Marta`; použitelné embedded datum chybí.
- Dávka nepřidala nové ID a rozšířila `URB-U-0073` o položky `191` až `195`.

Pracovní soubory dávky 39:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-39.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-39.yml`;
- `sources/index.d/urbanek-ccs-39.yml`;
- aktualizované `research/urbanek-archive/uncertainties/open-20.yml`.

## Registr nejistot

Autoritativní index: `research/urbanek-archive/uncertainties/index.yml`.

- `open`: 39;
- `deferred`: 0;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 73.

`URB-U-0073` nyní zahrnuje položky `186` až `195` a sleduje autorství, vydavatele, zdrojovou bibliografii, původ a úpravy vložených fotografií, historickou správnost textu a popisků a práva ke kalendáři 2015.

EXIF jméno, kalendářový popisek, moderní historický souhrn ani znovu použitá fotografie samy neurčují autora, vydavatele, původní zdroj nebo historickou správnost tvrzení.

## Kontrola konzistence draftu

- pilot a nová kolekce jsou odděleny;
- `STATUS.md`, `state.yml`, kolekční přehled a PR používají rozsah 200 + 1 = 201;
- průběžný stav je 195 zpracovaných a 6 zbývajících položek;
- registr používá součty 39/31/3/73;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Pilot: `completed`.
- Nová kolekce: `ccs_history_batch_processing_in_progress`.
- Následující položky: `urbanek-ccs-196` až `urbanek-ccs-200`.
- Očekávané názvy v podsložce `10 Kalendář 2015`: `11.jpg`, `12.jpg`, `13.jpg`, `14.jpg` a `15.jpg`.
- `Thumbs.db` v téže podsložce musí být po dokončení obrazů samostatně auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
