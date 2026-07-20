# Audit cache náhledů – Rychvaldské větrné mlýny

## Rozsah a metoda

Bylo zkontrolováno všech pět souborů `Thumbs.db`, které jsou v původní kolekci na Google Drivu, ale při technickém auditu nebyly nalezeny ve větvi `agent/import-urbanek-pilot`.

Soubory byly čteny jako Microsoft Compound File Binary. Z každého souboru byl načten stream `Catalog`, názvy byly porovnány s aktuálním seznamem fotografií ve stejné složce a byly vypočteny kontrolní součty SHA-256. Originály na Drivu nebyly změněny.

## Výsledky

| Původní cesta | Velikost | SHA-256 | Obrazové názvy v katalogu | Názvy navíc |
|---|---:|---|---:|---|
| `Rychvaldské větrné mlýny/Thumbs.db` | 53 760 B | `528e10c340a5a5ab07ee0f690f50c180df4b3c18401b471f3d400c0ce07fa150` | 11 | `P1010269.JPG` |
| `Rychvaldské větrné mlýny/větrný mlýn u hebdy/Thumbs.db` | 21 504 B | `66d06abeac65e6543f5180e377bb71f4c86a849b66e86d5c4de7b89833283dd1` | 3 | žádné |
| `Rychvaldské větrné mlýny/Mlýn u Kakalů/Thumbs.db` | 17 408 B | `f9eb42cd7d2427e47d3039a2095bab21c39a121438a289bcd47db1f75f253689` | 3 | žádné |
| `Rychvaldské větrné mlýny/mlýnské kameny a ruční mlýny/Thumbs.db` | 44 544 B | `f568c57191b317d94146071afd8240adabc1472cddfb765fdb9e0005d30de1ea` | 10 | žádné |
| `Rychvaldské větrné mlýny/Mlýn u domku č. pop. 339/Thumbs.db` | 20 480 B | `4a9b98f4c5a04bd16e00f7da0de0977968f46ed4a66d38c94e87a07ecc462571` | 4 | žádné |

Systémový záznam s GUID nebyl započítán jako obrazový název.

## Nález `P1010269.JPG`

Kořenový `Thumbs.db` obsahuje katalogový záznam `P1010269.JPG`, přestože stejnojmenný originál v aktuální kolekci nebyl nalezen. Z odpovídajícího streamu ID 4 se podařilo vyčlenit JPEG náhled:

- rozměry: 72 × 96 px;
- velikost: 4 896 B;
- SHA-256: `0253a94e8dfddbb1b8eb11ac592841ce49ebc168cd3a316099eee0a504ccf721`;
- technický stav: platný JPEG;
- popis `machine_unverified`: malý tmavý objekt nebo budova se šikmou střechou, částečně zakrytá stromy;
- čitelný text ve scéně: nezjištěn při tomto rozlišení.

Náhled není náhradou původního souboru. Musí být označen jako odvozený nález z cache a jeho identifikace zůstává `unverified`, dokud nebude porovnán s jinými fotografiemi nebo prameny.

## Závěr

- Soubory `Thumbs.db` mají archivní hodnotu a nemají být mazány z původního archivu.
- Čtyři z pěti cache nepřidávají další názvy fotografií.
- Kořenová cache uchovává poslední známou stopu po chybějícím souboru `P1010269.JPG` a také jeho malý náhled.
- Pět původních `Thumbs.db` nadále chybí v GitHub větvi a má být později doplněno pod přesnými původními cestami.
