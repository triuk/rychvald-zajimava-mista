# Audit `Thumbs.db` – Fotografie knihy Rychvald včera a dnes

Datum auditu: 2026-08-06

## Soubor

- zdrojová cesta: `Fotografie knihy Rychvald včera a dnes/Thumbs.db`
- repo cesta: `sources/osobni-archiv-jaromira-urbanka/Fotografie knihy Rychvald včera a dnes/Thumbs.db`
- velikost: `203264` B
- SHA-256: `86a9e6592075496d6302389198300e09623f104c3a74a593a93ffca2107d8ff8`
- Git blob SHA: `994155fade2d4f2472cb8b77976262b767ab38f4`
- Drive ID: `1tH47HgF21oE69wvCOytZSMnNgJczU-0q`

Drive originál a soubor ve větvi jsou binárně shodné: velikost se shoduje a lokálně vypočtený Git blob SHA odpovídá blobu evidovanému v repozitáři.

## Metoda

Soubor byl identifikován jako OLE/Compound File Binary dokument používaný staršími verzemi Windows pro cache náhledů. Audit zahrnoval:

1. rozbor hlavičky, FAT, MiniFAT, adresářových položek a kořenového mini-streamu;
2. dekódování streamu `Catalog`;
3. kontrolu vazby katalogových ID na datové streamy;
4. extrakci a dekódování všech JPEG náhledů;
5. porovnání katalogových názvů se sadou plných souborů v Git;
6. přímé obrazové porovnání se stejně pojmenovanými originály `20.jpg`–`53.jpg`, které byly v pracovním prostředí dostupné.

## Struktura a integrita

- CFB major verze: `3`;
- velikost sektoru: `512` B;
- velikost minisektoru: `64` B;
- katalog verze: `7`;
- deklarovaný počet katalogových položek: `54`;
- deklarovaný cílový rozměr náhledu: `96 × 96` px;
- obrazové datové streamy: `54`;
- streamy s platným JPEG od offsetu 12: `54`;
- chybějící nebo nadbytečné datové streamy: `0`;
- binárně duplicitní cache náhledy: `0`.

Všechny náhledy se dekódují. Jejich šířka je vždy 96 px a výška se podle poměru stran originálu pohybuje od 40 do 63 px.

## Katalogové názvy

Katalog obsahuje přesně tuto množinu názvů:

- `0 titulní stránka.jpg`;
- `1.jpg` až `53.jpg`.

Tato množina se přesně shoduje se 54 plnými JPEGy v repozitáři. Cache neobsahuje žádný další název zdrojového obrázku a v repozitáři nechybí žádný katalogovaný plný soubor.

Katalogové pořadí není čistě lexikografické ani číselné; například `53.jpg` je uloženo před položkami `48.jpg`–`52.jpg`. Katalogové ID a navázané streamy jsou však konzistentní, takže pořadí není známkou chybějícího souboru.

## Obrazové porovnání

Pro 34 lokálně dostupných plných JPEGů `20.jpg`–`53.jpg` byly cache náhledy porovnány se zmenšenými originály ve stejné orientaci:

- všech 34 náhledů má jednoznačně nejlepší shodu se stejně pojmenovaným plným souborem;
- nebyla zjištěna otočená ani zrcadlená záměna;
- průměrná absolutní odchylka RGB po normalizaci se pohybovala přibližně od `3,74` do `7,50`, což odpovídá běžnému rozdílu po zmenšení a opětovné JPEG kompresi.

U zbývajících dvaceti položek je vazba jména na stream doložena přímo katalogovou strukturou; jejich plné soubory jsou přítomny v Git a žádný další katalogový název ani stream neexistuje.

## Časová metadata

Katalogové časy obrazových položek sahají přibližně od 22. srpna do 11. října 2013. Kořenový CFB záznam má čas 8. prosince 2014. Tyto hodnoty jsou metadata vytvoření či aktualizace cache a nejsou dokladem data fotografování, vydání knihy ani historické události.

## Závěr

- katalogové názvy: **54**;
- dekódované náhledy: **54**;
- názvy nebo náhledy bez odpovídajícího plného souboru: **0**;
- chybějící plné originály doložené touto cache: **0**;
- další samostatný obrazový obsah: **nezjištěn**.

`Thumbs.db` se eviduje jako technický soubor a není klasifikován ani OCR zpracován jako běžný obrazový pramen. Audit uzavírá inventarizaci kolekce v rozsahu 55 z 55 položek. Neřeší otevřenou otázku autorství, práv ani přesného vztahu fotografií ke knize vedenou pod `URB-U-0076`.
