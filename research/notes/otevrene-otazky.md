# Otevřené otázky

Sem zapisuj nevyřešené otázky, rozpory mezi prameny a informace vyžadující další ověření.

## Úplnost a původ textových přepisů kronik

- `kronika-ka631`: úvod přepisu uvádí 400 stran, ale soubor končí značkou strany 294 a událostí z roku 1930. Název souboru přitom uvádí období 1922–1935. Je nutné porovnat přepis s obrazovým originálem a zjistit, zda stránky nebo pozdější zápisy chybějí, případně zda zbývající stránky původní knihy nebyly popsány.
- `kronika-ka632-27`: název souboru obsahuje roky 1965–1970, zatímco vnitřní titul a jednotlivé oddíly uvádějí období 1964–1969. Za určující je zatím považován vnitřní obsah; původ názvu souboru je třeba objasnit.
- `kronika-ka632-28`: název souboru zdůrazňuje rok 1971, hlavní kronikářský zápis však zachycuje rok 1970. Za nadpisem „Rok 1971“ následují dvě listiny z prosince 1972, nikoli pozorovatelný kronikářský zápis za rok 1971.
- U všech tří textových přepisů není znám postup jejich vzniku ani míra kontroly proti originálu. Nemají spolehlivě zachované digitální hranice stran, proto před použitím v článku vyžadují ověření lokátoru proti obrazové nebo archivní předloze.

## Obrazové materiály, mapy a obsahové přehledy

- Inventář rozlišuje doložené fotografie na vizuálně zkontrolovaných prvních stranách a kandidátní výskyty map či obsahových přehledů zjištěné celotextovým vyhledáním. Hodnota `candidate` v `sources/index.yml` neprokazuje existenci konkrétní mapy nebo rejstříku; je nutné ověřit příslušnou stranu.
- Textové přepisy kronik odkazují na fotografie nebo dokumentární přílohy, ty však nejsou v textových souborech vloženy. Je třeba dohledat obrazové originály a jejich přesné vazby na zápisy.
- V `images/` zatím nejsou samostatné historické fotografie ani mapy. Fotografie obsažené ve zpravodajích nelze vyčlenit k publikaci bez zjištění autora, původu, držitele práv a licenčního stavu.

## Nestandardní dokumenty mezi zpravodaji

- `rm-2019-027` je uložen v adresáři zpravodajů, obsahem však jde o samostatné usnesení Rady města Rychvald ze dne 28. června 2019. V inventáři je proto veden jako jiný typ dokumentu, aniž by byl původní soubor přemístěn.
- `rychvald-2024-sumar` je samostatný roční souhrn města, nikoli běžné číslo Rychvaldského zpravodaje.
- `rz-2026-01` je lednové číslo 2026, které v jednom PDF obsahuje také přílohu „Sumář 2025“. Je třeba rozhodnout, zda při výzkumu citovat celý soubor pod jedním `source_id`, nebo příloze zavést samostatný logický lokátor v rámci stejného souboru.

## Práva

- U žádného z 209 dokumentů nebyla při inventarizaci ověřena licence umožňující další zveřejnění. U zpravodajů a městských dokumentů je uveden vydavatel Město Rychvald, což samo o sobě neurčuje autora jednotlivých textů a fotografií ani rozsah publikačních oprávnění.

## Rozpory zjištěné při katalogizaci míst

- **Rychvaldský zámek:** `rz-2011-04`, s. 3 uvádí rok výstavby 1573; `rz-2011-11`, s. 8 druhou polovinu 70. let 16. století; `rz-2025-05`, s. 5 léta 1575–1577; a `kronika-ka631`, ř. 4564–4575 klade důkladnou přestavbu nynějšího zámku do roku 1595. Je třeba zjistit, zda prameny zaměňují získání panství, výstavbu a pozdější přestavbu, nebo si v dataci odporují.
- **Košicko-bohumínská dráha:** `kronika-1989-2000`, s. 7 uvádí výstavbu přes Rychvald roku 1867; `kronika-ka631`, ř. 265–304 uvádí rok 1870. Rozpor je nutné ověřit v železničním nebo mapovém prameni.
- **Škola U Laštůvků:** `kronika-ka631`, ř. 3569–3590 uvádí stavbu roku 1904, zatímco `rz-2012-11`, s. 10 uvádí otevření roku 1906. Může jít o rozdíl mezi výstavbou a zahájením výuky.
- **Rybník Skučák:** prameny zachycují podoby Skučák, Škuťák a Škuták. Je třeba určit, které jsou úřední, nářeční nebo chybně přepsané.
- **Cihelník:** vztah názvů Cihelňák, Cihelník, Velký Cihelník a Malý Cihelník zatím není mapově ověřen.

## Lokalizace a současný stav

- U každého záznamu v `research/places.yml` je uvedena jen přesnost, kterou dovolují nahrané prameny. Přesná současná poloha, adresa a stav musí být před článkem ověřeny samostatným aktuálním zdrojem.
- Je třeba dohledat přesnou polohu bývalé zastávky Vyhýbka, kaple u Bodingera, Drobíkova, Vítkova a Pospěchova mlýna, Dvorku velkostatku a historických lesíků Fojtok, Liščok a Pastuchův lesík.
- U starých čísel popisných nelze bez katastrálního nebo mapového srovnání předpokládat, že dnešní číslování označuje tutéž budovu.
- U zaniklých škol je třeba oddělit instituci od budovy: názvy školy se mohly stěhovat a jedna budova mohla sloužit více školám.

## Fotografie a kresby konkrétních míst

- Zpravodaje obsahují obrazový materiál k zámku, kostelu sv. Anny, Skučáku, školám, mlýnům, Sokolovně a památníkům. Před převzetím do `images/` je nutné u každého snímku nebo kresby zjistit autora, datum, původ, držitele práv a licenci.
- Kresby mlýnů na `rz-2011-09`, s. 14 jsou reprodukcemi děl Přemysla Pastuchy, nikoli automaticky volně použitelnými historickými fotografiemi.
- U tvrzení převzatých pouze z textových přepisů kronik je stav nejvýše `partially_verified`, dokud nebude výňatek a lokátor porovnán s obrazovým originálem.
