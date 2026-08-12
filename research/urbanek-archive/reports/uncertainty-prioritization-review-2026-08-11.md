# Revize a prioritizace otevřených nejistot

Datum revize: 2026-08-11

## Rozsah

Revize navazuje na dokončení úplného inventárního a indexačního průchodu aktuálním Git snapshotem archivu Jaromíra Urbánka (616/616 položek). Bylo ručně projito všech 53 položek se stavem `open` v registru nejistot.

Cílem nebylo mechanicky měnit původní `priority:` ani slučovat tematicky podobné otázky, ale vytvořit výzkumné pořadí podle:

1. přímého významu pro dějiny a místopis Rychvaldu;
2. dopadu na identifikaci míst, staveb, osob a významných událostí;
3. schopnosti jedné odpovědi odemknout více dalších položek;
4. dostupnosti textových, mapových, matričních, tiskových nebo technických pramenů;
5. rizika, že by široká nebo sekundární otázka pohltila samostatné dílčí nejistoty.

## Kontrola duplicit

Nebyla nalezena žádná dvojice otevřených položek, kterou by bylo bezpečné sloučit jako totožnou otázku bez ztráty nevyřešených atributů nebo historie evidence.

Řada položek se překrývá — zejména v kolekci `Historie Církve československé v Rychvaldě ve fotografiích` — ale překryv je vztah mezi otázkami, nikoli důkaz jejich totožnosti. Existující stabilní ID proto zůstávají zachována.

## Výzkumná vlna 1 — přímý Rychvald a vysoký přínos

Následujících 15 položek má přednost v systematickém řešení:

- `URB-U-0036` — Kakalův mlýn: přesná poloha, vlastnictví, existence a technologie;
- `URB-U-0038` — větrný mlýnek za domem čp. 339: vlastník, poloha a historie;
- `URB-U-0044` — průčelí Husova sboru, nápis a znak v období polského záboru;
- `URB-U-0049` — chronologie rekonstrukce interiéru Husova sboru;
- `URB-U-0053` — autorství a datace figurálních maleb, archivně připisovaných Obšilovi;
- `URB-U-0062` — volba, jmenování a inaugurace Gabriela Chrobáčka a související obrazová série;
- `URB-U-0063` — 50. výročí CČS v Rychvaldě roku 1970 a identifikace hostů;
- `URB-U-0065` — obnovená tradice husovské hranice a její chronologie;
- `URB-U-0067` — Karel a Libuše Vodičkovi, pamětní deska, návštěvy a pohřební série;
- `URB-U-0075` — přesný rukopisný svazek a úplnost oddílu `Náboženský převrat v Rychvaldě`;
- `URB-U-0077` — identifikace historického nádraží;
- `URB-U-0078` — ozbrojená skupina u tabule `MĚSTO RYCHVALD`, archivně spojovaná s říjnem 1938;
- `URB-U-0079` — archivní kontext tajného seznamu SNB Fryštát z 10. 7. 1945;
- `URB-U-0081` — přesné zařazení fotografovaných vydání a stran `Českého slova` z roku 1938;
- `URB-U-0085` — bibliografické zařazení novinových výstřižků z let 1903–1925.

Pořadí uvnitř vlny není neměnné. Pokud jedna položka narazí na pramen, který zároveň přímo řeší jinou položku, má se využít společný pramen a zachovat oddělené závěry pod příslušnými ID.

## Paralelní větev — obnova chybějících plných originálů

Tyto dvě položky jsou technicky dobře vymezené a lze je řešit paralelně cíleným hledáním názvů a binárních/obrazových shod v ostatních úložištích:

- `URB-U-0086` — 9 odlišných chybějících obrazových obsahů v kolekci novinových článků 1903–1925;
- `URB-U-0088` — 16 odlišných chybějících obrazových obsahů v kolekci `popopo`.

Cache-only náhledy zůstávají technickým důkazem existence obrazového obsahu, nikoli náhradou plného originálu.

## Průřezové a dekompoziční položky

Následující široké položky nemají být řešeny jedním globálním tvrzením. Mají fungovat jako zastřešující registr a při výzkumu se mají uzavírat jen konkrétní atributy nebo vytvářet úžeji vymezené navazující položky:

- `URB-U-0073` — kalendář 2015, autorství, zdroje, sekundární historická tvrzení a práva;
- `URB-U-0076` — letecké fotografie a jejich vztah ke knize `Rychvald včera a dnes`;
- `URB-U-0082` — široká kolekce `Rychvald`;
- `URB-U-0083` — kořenová část `fotodokument`;
- `URB-U-0084` — fotografie nepoužité pro knihu ani kalendář;
- `URB-U-0087` — smíšená kolekce `popopo`.

## Závislé a následné položky

Zbývajících 30 otevřených položek se ponechává aktivních a řeší se po první vlně nebo dříve, pokud je přímo odemkne nově nalezený pramen:

`URB-U-0008`, `URB-U-0037`, `URB-U-0039`, `URB-U-0040`, `URB-U-0041`, `URB-U-0042`, `URB-U-0043`, `URB-U-0045`, `URB-U-0046`, `URB-U-0047`, `URB-U-0048`, `URB-U-0050`, `URB-U-0051`, `URB-U-0052`, `URB-U-0054`, `URB-U-0055`, `URB-U-0056`, `URB-U-0057`, `URB-U-0058`, `URB-U-0059`, `URB-U-0060`, `URB-U-0061`, `URB-U-0064`, `URB-U-0066`, `URB-U-0068`, `URB-U-0069`, `URB-U-0070`, `URB-U-0071`, `URB-U-0072`, `URB-U-0080`.

Toto zařazení neznamená nižší historickou hodnotu. Vyjadřuje pouze pořadí efektivního výzkumu pro projekt Rychvald.

## Evidence-link review

Struktura registru, soubory `open-*.yml`, kolekční evidence a `sources/index.d` byly při revizi kontrolovány na úrovni repozitářových cest a názvosloví. Nebyla zjištěna položka, kterou by bylo nutné uzavřít jen kvůli zjevně neexistujícímu kořenovému zdroji. Jednotlivé evidence cesty se mají znovu dereferencovat při řešení konkrétního ID; revize záměrně nepovažuje samotnou existenci cesty za potvrzení historického tvrzení.

## První aktivní položka

Systematické řešení začíná `URB-U-0036` — Kakalův mlýn.

Identita obrazu jako Kakalův mlýn je již uzavřena pod `URB-U-0007`. Otevřené zůstávají přesná poloha, číslo domu, vlastník, období existence a technické vybavení. Negativní vyhledání není důvodem k uzavření těchto atributů.
