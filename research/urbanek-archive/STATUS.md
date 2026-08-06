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

- PR: [#1 – Index and classify Jaromír Urbánek archive (in progress)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft
- Base: `main`
- Head: `agent/import-urbanek-pilot`
- Sloučení nebylo vyžádáno.

## Stav indexace

| Stav | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| zpracováno | 440 | 20 | **460** |
| zbývá | 147 | 9 | **156** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je deset kolekcí. Kolekce `Noviny 1938 České slovo` je uzavřena v rozsahu 35 z 35 položek.

## Noviny 1938 České slovo – technický audit

Auditovány byly soubory `Thumbs.db` a `ZbThumbnail.info`:

- oba Drive soubory přesně odpovídají Git blobům;
- `Thumbs.db` obsahuje 33 pojmenovaných náhledů odpovídajících 33 plným JPEGům a jeden samostatný náhled ikony složky;
- `ZbThumbnail.info` obsahuje 33 jedinečných názvů JPEGů a 33 vložených náhledů;
- množiny názvů v obou cache se přesně shodují s plnými JPEGy kolekce;
- žádná cache neobsahuje `P1020282.JPG`, cache-only název ani náhled bez plného originálu;
- technické soubory tedy nedokládají chybějící plný originál.

`Thumbs.db` je CFB/OLE soubor verze 3 s katalogem verze 7. Má 34 JPEG streamů: 33 zdrojových náhledů a čtvercový náhled složky. `ZbThumbnail.info` má signaturu `zbex` a 33 JPEG náhledů o rozměrech 160 × 120 nebo 120 × 160 px.

Nejistota `URB-U-0081` zůstává otevřená pro provenienci fyzických předloh, úplnost mimo aktuální snapshot, posloupnost stran a vydání, okolnosti digitalizace a práva. Technická část otázky chybějících souborů v cache byla uzavřena negativním výsledkem.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **147** | **9** | **156** |

## Registr nejistot

- `open`: 46;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 81.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 460 položek;
- zbývá 156 položek;
- kolekce `Noviny 1938 České slovo` je zpracována v rozsahu 35 z 35 položek;
- oba technické soubory přesně odpovídají Git blobům;
- obě cache odkazují právě na 33 přítomných JPEGů a nedokládají další plný originál;
- registr používá součty 46/32/3/81;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další skupina: `Rychvald`.
- První dávka: `Budova úřadu 003.jpg`, `Budova úřadu 005.jpg`, `Cudlín 033.jpg`, `Cudlín 035.jpg` a `Cudlín 037.jpg`.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
