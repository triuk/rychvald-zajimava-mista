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
| zpracováno | 407 | 18 | **425** |
| zbývá | 180 | 11 | **191** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je devět kolekcí. Skupina šesti volných souborů přímo v kořeni archivu je dokončena.

## Volné soubory v kořeni – dokončení dávkou 02

V dávce 01 byly zpracovány položky `19.jpg`, `20Hlavička 27.10.1938.jpg`, `21zpráva 28.10.1938.jpg`, `9 X 1938 przed zajęciem Rychvaldu.png` a `IMG_0117 seznam bojůvkařů.jpg`.

Dávka 02 dokončila skupinu souborem:

- `img237 německý četník.jpg` – sepiově až azurově tónovaná reprodukce ateliérového portrétu jednoho uniformovaného muže v čepici se štítkem, zapnuté blůze, opasku a vysokých botách; u pravého boku je tmavé pouzdro nebo brašna. Archivní název není nezávislým důkazem národnosti, služebního sboru, hodnosti, totožnosti, data, místa ani vazby k Rychvaldu.

Soubor má 31 086 B, rozměry 328 × 545 px, neobsahuje EXIF metadata a přesně odpovídá blobu evidovanému ve větvi. Nově je vedena nejistota `URB-U-0080`.

Pracovní soubory skupiny:

- `research/urbanek-archive/collections/root-loose-files-overview.yml`;
- `research/urbanek-archive/collections/root-loose-files-batch-01.yml` a `root-loose-files-batch-02.yml`;
- `research/urbanek-archive/collections/root-loose-files-inventory-01.csv` a `root-loose-files-inventory-02.csv`;
- `sources/index.d/urbanek-root-loose-files-01.yml` a `urbanek-root-loose-files-02.yml`;
- `research/urbanek-archive/uncertainties/open-23.yml`.

## Dosud nezpracované skupiny

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Noviny 1938 České slovo | 33 | 2 | 35 |
| Rychvald | 31 | 2 | 33 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **180** | **11** | **191** |

## Registr nejistot

- `open`: 45;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 80.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 425 položek;
- zbývá 191 položek;
- kořenová skupina je zpracována v rozsahu 6 z 6 položek;
- registr používá součty 45/32/3/80;
- PR zůstává otevřený draft a není žádostí o sloučení;
- GitHub dosud nevrátil hlášené CI status checks; nejde tedy o úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Následující skupina: `Noviny 1938 České slovo` (35 položek).
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
