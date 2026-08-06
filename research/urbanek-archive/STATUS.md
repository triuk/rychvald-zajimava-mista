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
| zpracováno | 406 | 18 | **424** |
| zbývá | 181 | 11 | **192** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je osm kolekcí. Skupina volných souborů přímo v kořeni archivu je rozpracovaná v rozsahu **5 z 6 položek**.

## Volné soubory v kořeni – dávka 01

Zpracovány a Git-ověřeny byly:

- `19.jpg` – černobílá historická reprodukce s tištěným označením „Nádraží“; přesná stanice, lokalita, datum, autor a vydavatel nejsou doloženy;
- `20Hlavička 27.10.1938.jpg` – horní část listu *České slovo*, čtvrtek 27. října 1938, ročník X, číslo 297;
- `21zpráva 28.10.1938.jpg` – strana 6 listu *České slovo*, pátek 28. října 1938, číslo 298, s hlavním článkem „Od pondęlka se létá do Prahy“;
- `9 X 1938 przed zajęciem Rychvaldu.png` – pět ozbrojených mužů v uniformách u tabule s čitelným nápisem „MĚSTO RYCHVALD“; archivní název není nezávislým důkazem data, události nebo jednotky;
- `IMG_0117 seznam bojůvkařů.jpg` – fotografie tajného seznamu Okresního velitelství SNB ve Fryštátě z 10. července 1945; osobní údaje v tabulce nejsou v souhrnném indexu přepisovány.

Všechny soubory přesně odpovídají blobům evidovaným ve větvi a v dávce ani v aktuálním archivním stromu nebyla zjištěna přesná binární duplicita. EXIF hodnoty z let 2013–2016 jsou vedeny pouze jako metadata pozdější digitalizace nebo zpracování, nikoli jako historická data zobrazených scén či dokumentů.

Nově jsou vedeny nejistoty `URB-U-0077` až `URB-U-0079`.

Pracovní soubory:

- `research/urbanek-archive/collections/root-loose-files-overview.yml`;
- `research/urbanek-archive/collections/root-loose-files-batch-01.yml`;
- `research/urbanek-archive/collections/root-loose-files-inventory-01.csv`;
- `sources/index.d/urbanek-root-loose-files-01.yml`;
- `research/urbanek-archive/uncertainties/open-23.yml`.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| zbývající volný soubor přímo v kořeni | 1 | 0 | 1 |
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **181** | **11** | **192** |

## Registr nejistot

- `open`: 44;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 79.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 424 položek;
- zbývá 192 položek;
- aktuální kořenová skupina je zpracována v rozsahu 5 z 6 položek;
- registr používá součty 44/32/3/79;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Následující soubor: `img237 německý četník.jpg`.
- Po jeho zpracování bude skupina volných kořenových souborů dokončena.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
