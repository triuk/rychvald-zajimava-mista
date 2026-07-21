# Audit `Thumbs.db` – fotodokument/den po dešti

## Zdroj a metoda

- Původní cesta na Google Drivu: `fotodokument/den po dešti/Thumbs.db`
- Velikost: 32 256 B
- SHA-256: `107910de5c9211d7048b338d5df1b7e1ec407bf4c8c75615fafba7f090f9fd9c`
- Stav v GitHubu: `drive_listed_repo_missing`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**

Soubor byl načten jako Microsoft Compound File Binary. Katalog byl spojen s osmi JPEG náhledovými streamy.

## Souhrn

- katalogových záznamů: **8**;
- JPEG náhledů: **8**;
- unikátních náhledů: **8**;
- názvů odpovídajících současným souborům ve složce: **7**;
- dodatečných názvů bez nalezeného plného originálu: **1**;
- současných JPEGů, které ve starší cache nejsou: **1**.

## Katalog cache

| Stream | Historický název | Rozměr náhledu |
|---:|---|---:|
| 1 | `P1020847.JPG` | 72 × 96 |
| 2 | `P1020841.JPG` | 72 × 96 |
| 3 | `P1020840.JPG` | 96 × 72 |
| 4 | `P1020842.JPG` | 72 × 96 |
| 5 | `P1020843.JPG` | 96 × 72 |
| 6 | `P1020844.JPG` | 72 × 96 |
| 7 | `P1020845.JPG` | 72 × 96 |
| 8 | `P1020846.JPG` | 72 × 96 |

## Chybějící plný originál

### `P1020841.JPG`

- V současné složce ani v ověřené cestě GitHubu nebyl nalezen plný soubor.
- Cache uchovává pouze náhled 72 × 96 px.
- Bezpečný vizuální popis: úzká mokrá nebo štěrková cesta lemovaná trávou, stromy a oplocením či zástavbou.
- Náhled není náhradou originálu a nestačí k přesnému určení místa, data nebo rozsahu škod.

## Současný soubor mimo cache

`P1040200.JPG` je v aktuální složce i v GitHubu, ale v této starší cache není. To pravděpodobně znamená, že byl do složky přidán nebo zobrazen až po vytvoření cache; samotná cache časovou posloupnost spolehlivě nedokládá.

## Důsledky

- `Thumbs.db` nesmí být smazán z původního archivu; je jediným známým nosičem náhledu `P1020841.JPG`.
- Při hledání v jiných složkách nebo zálohách použít přesný název `P1020841.JPG` a obrazovou podobnost.
- Chybějící technická cache ve větvi neblokuje klasifikaci osmi současných JPEGů.
- Standardní OCR se pro cache neprovádí.
