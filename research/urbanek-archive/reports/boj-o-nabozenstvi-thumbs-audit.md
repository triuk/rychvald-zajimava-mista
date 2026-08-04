# Audit `Thumbs.db` – Boj o náboženství v Rychvaldě

Datum auditu: 2026-08-04

## Soubor

- zdrojová cesta: `Boj o náboženství v Rychvaldě/Thumbs.db`
- velikost: 10 752 B
- SHA-256: `56948ec4331d112ae5f4605c0eca21501614e9db7eda986c5ce3104f918ce699`
- Git blob SHA: `851ca380ea17a719b05d5cffd5b8ebaad462dbdd`
- Drive ID: `1EG6QKs7nFBSwHroOKpP1qwijBvk5P6GO`

Drive originál a soubor ve větvi jsou binárně shodné: lokálně vypočtený Git blob SHA
odpovídá blobu evidovanému v repozitáři.

## Struktura

Soubor je platný Compound File Binary dokument používaný staršími verzemi Windows
pro cache náhledů. Obsahuje stream `Catalog` a tři obrazové streamy `1`, `2` a `3`.

Katalog obsahuje přesně tři záznamy:

1. `P1010899.JPG`
2. `P1010900.JPG`
3. `P1010901.JPG`

Katalogové časy odpovídají 4. červnu 2012 a navazují na EXIF časy tří plných JPEGů.
Jde o metadata vzniku digitálních reprodukcí a cache, nikoli o data historických událostí.

## Obrazové porovnání

Ze všech tří streamů byl dekódován náhled JPEG o rozměru 72 × 96 pixelů.
Každý náhled byl porovnán se zmenšenými plnými soubory:

- stream `1` odpovídá `P1010899.JPG`;
- stream `2` odpovídá `P1010900.JPG`;
- stream `3` odpovídá `P1010901.JPG`.

Všechny tři plné originály jsou v kolekci přítomny a Git-ověřeny.

## Závěr

- katalogové názvy: 3;
- dekódované náhledy: 3;
- názvy nebo náhledy bez odpovídajícího plného souboru: **0**;
- chybějící plné originály doložené touto cache: **0**;
- další samostatný obrazový obsah: **nezjištěn**.

`Thumbs.db` se eviduje jako technický soubor a není klasifikován ani OCR zpracován jako
běžný obrazový pramen.
