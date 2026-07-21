# Audit cache náhledů – Rychvaldské větrné mlýny

## Rozsah a metoda

Bylo zkontrolováno všech pět souborů `Thumbs.db` v kolekci. Všechny jsou nyní přítomné ve větvi `agent/import-urbanek-pilot` pod přesnými původními cestami.

Soubory byly čteny jako Microsoft Compound File Binary. Z každého souboru byl načten stream `Catalog`, názvy byly porovnány s aktuálním seznamem fotografií ve stejné složce a byly vypočteny kontrolní součty SHA-256. Zdrojové soubory nebyly změněny.

## Výsledky

| Cesta v archivu | Velikost | SHA-256 | Obrazové názvy v katalogu | Názvy navíc |
|---|---:|---|---:|---|
| `Rychvaldské větrné mlýny/Thumbs.db` | 53 760 B | `528e10c340a5a5ab07ee0f690f50c180df4b3c18401b471f3d400c0ce07fa150` | 11 | `P1010269.JPG` |
| `Rychvaldské větrné mlýny/větrný mlýn u hebdy/Thumbs.db` | 21 504 B | `66d06abeac65e6543f5180e377bb71f4c86a849b66e86d5c4de7b89833283dd1` | 3 | žádné |
| `Rychvaldské větrné mlýny/Mlýn u Kakalů/Thumbs.db` | 17 408 B | `f9eb42cd7d2427e47d3039a2095bab21c39a121438a289bcd47db1f75f253689` | 3 | žádné |
| `Rychvaldské větrné mlýny/mlýnské kameny a ruční mlýny/Thumbs.db` | 44 544 B | `f568c57191b317d94146071afd8240adabc1472cddfb765fdb9e0005d30de1ea` | 10 | žádné |
| `Rychvaldské větrné mlýny/Mlýn u domku č. pop. 339/Thumbs.db` | 20 480 B | `4a9b98f4c5a04bd16e00f7da0de0977968f46ed4a66d38c94e87a07ecc462571` | 4 | žádné |

Systémový záznam s GUID nebyl započítán jako obrazový název.

## Nález `P1010269.JPG`

Kořenový `Thumbs.db` obsahuje katalogový záznam `P1010269.JPG`, přestože stejnojmenný plný soubor v aktuální kolekci není. Z odpovídajícího streamu ID 4 byl vyčleněn platný JPEG náhled:

- rozměry: 72 × 96 px;
- velikost: 4 896 B;
- SHA-256: `0253a94e8dfddbb1b8eb11ac592841ce49ebc168cd3a316099eee0a504ccf721`.

Uživatel potvrdil a přesné obrazové porovnání ověřilo, že náhled je zmenšeninou dochovaného souboru `mlýn na podlesí.JPG`. Shodují se větvení stromů, poloha turbíny a stožáru, střecha i budova. Náhled tedy nepředstavuje další chybějící obrazový výjev; chybí pouze samostatný soubor pod původním názvem `P1010269.JPG`.

Objekt byl následně ověřen proti databázi Povětrník jako záznam 229, větrný mlýnek s turbínou na adrese U Školky 344 v Rychvaldu. Podrobnosti jsou v `research/urbanek-archive/verifications/urb-u-0003-0006-podlesi-povetrnik-229.md`.

## Závěr

- Všech pět souborů `Thumbs.db` je součástí Git repozitáře a nemá být mazáno.
- Čtyři z pěti cache nepřidávají další názvy fotografií.
- Kořenová cache uchovává historický název `P1010269.JPG` a duplicitní náhled dochovaného souboru `mlýn na podlesí.JPG`.
- Technická úplnost kolekce je vyřešena a žádný další unikátní obrazový obsah v této cache nechybí.
