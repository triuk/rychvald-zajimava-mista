# Audit `Thumbs.db` – Články z Českého slova

## Zdroj a metoda

- Cesta v repozitáři: `sources/osobni-archiv-jaromira-urbanka/Články z Českého slova/Thumbs.db`
- Velikost: 304 640 B
- SHA-256: `0647ec694c2bbbd6be13517d0e201f498199bd57e825b63140c4f32ae0c43800`
- Git blob SHA: `f087d7ecec991aaa5d3327f4e7a9cf4130e44c3c`
- Stav: `repo_verified`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**

Soubor byl načten jako Microsoft Compound File Binary. Z katalogu bylo získáno 97 záznamů a ze všech odpovídajících streamů se podařilo načíst platný JPEG náhled. Náhledy byly porovnány podle dekódovaných obrazových pixelů, nikoli pouze podle názvů.

## Souhrn

- katalogových názvů: **97**;
- názvů přesně odpovídajících současným 37 obrazovým souborům: **37**;
- dalších historických nebo pracovních názvů: **60**;
- unikátních obrazových náhledů po odstranění obrazových duplicit: **45**;
- unikátních náhledů odpovídajících současným souborům: **37**;
- unikátních obrazů, jejichž současný plný soubor nebyl nalezen: **8**.

Zbývajících 52 nestávajících názvů sdílí přesně stejný dekódovaný náhled s některým ze současných souborů. Jde tedy zejména o starší názvy, meziverze nebo přejmenování, nikoli o další unikátní obrazový obsah.

## Osm unikátních chybějících obrazů

| ID katalogu | Historický název | Rozměr náhledu | JPEG SHA-256 | Bezpečný vizuální popis |
|---:|---|---:|---|---|
| 2 | `P1020274aa.jpg` | 96 × 52 | `a41828dff366b9186531fc1e408b1bd6d8a78bd3c80593f54e67684c0178c441` | Výřez novinové stránky s velkým nadpisem a více sloupci; přesné znění nadpisu není při tomto rozlišení spolehlivě čitelné. |
| 22 | `P1020273aaaa.jpg` | 96 × 71 | `e87783988c13a08e4690e17624dd1739ab581341970cdcf87f4d72a86d3828c3` | Ručně popsaný titulní nebo oddělovací list; bezpečně je čitelné spojení `České slovo` a rok `1938`, další slovo nad ním je nejisté. |
| 24 | `P1020311aaaaa.jpg` | 96 × 60 | `85c6079cd0a8804f4e9e0a9fda406095c1e5a65132ea770046ac68b678aac4ec` | Novinový článek s výrazným nadpisem; přesný přepis není z náhledu spolehlivý. |
| 25 | `P1020315aaa.jpg` | 96 × 66 | `a5c58a5a33af8230dbe772e74026ab09e404963dcb7fcde4a81baa8e35fdaadc` | Novinový článek, jehož nadpis končí bezpečně čitelným spojením `na Těšínsku`; předchozí slova zůstávají nejistá. |
| 26 | `P1020316aaa.jpg` | 96 × 68 | `9130e4bfada5b0393807c73a56c2a793872d475cbd3cc41b497c0d1b22e903d2` | Další novinový článek s nadpisem obsahujícím spojení `polského záboru` a `na Těšínsku`; začátek nadpisu je oříznutý nebo nečitelný. |
| 30 | `P1020321aaa.jpg` | 96 × 41 | `d87c496c0f0475574143a238151ce5a231f07c7155eef95066cd4bd4a97f01a8` | Úzký výřez novinového článku se třemi sloupci; nadpis nelze bezpečně přepsat. |
| 31 | `P1020320aaaa.jpg` | 57 × 96 | `61d6ff261f7dc81d439aca3d670de35cf05ca595518b88ac0406c80d18fcda13` | Svislá novinová stránka nebo koláž s několika fotografiemi či ilustracemi a textovými bloky. |
| 42 | `P1020334aaa.jpg` | 96 × 35 | `7c6778f7ed8f88d1122058c2b2df146080e9c49c38b0bc583d2b4bddc537b14f` | Velmi úzký výřez novinového článku s výrazným nadpisem; přesné znění je nejisté. |

## Důsledky pro další práci

- `Thumbs.db` je součástí Git repozitáře a nesmí být smazán; je jediným známým nosičem osmi dodatečných obrazových náhledů.
- Náhledy nejsou náhradou originálních fotografií a nemají být používány jako plnohodnotné stránky pro OCR.
- Osm náhledů lze použít jako vodítko při hledání originálních snímků v jiných složkách archivu nebo v dalších zálohách.
- Před zahájením dalšího zpracování současných 37 souborů není nutné chybějící obrazy rekonstruovat; je však nutné zachovat jejich názvy, kontrolní součty a vazbu na cache.
- Historické názvy v cache ukazují, že současná číselná řada vznikla přejmenováním nebo výběrem z většího pracovního souboru.

## Omezení

Vizuální popisy jsou `machine_unverified`. Původní náhledy mají velmi malé rozlišení a zvětšení nepřidává chybějící obrazovou informaci. Nejasné nadpisy proto nebyly domýšleny.
