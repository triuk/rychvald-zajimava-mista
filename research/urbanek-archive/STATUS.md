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
| zpracováno | 471 | 20 | **491** |
| zbývá | 116 | 9 | **125** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je deset kolekcí. Kolekce `Rychvald` má zpracováno všech **31 obsahových souborů**; zbývají dva technické soubory.

## Rychvald – dávka 07

Zpracován byl poslední obsahový soubor `zzz-satiny 258.jpg`.

Snímek zachycuje několik řad hrobů a náhrobků s květinovou výzdobou a vzrostlými stromy. Nápisy na náhrobcích nejsou používány k identifikaci osob. Přesná identita hřbitova ani historický kontext nejsou z obrazu samotného určeny.

Raw soubor z kanonické Drive složky má 688 289 B a jeho vypočtený Git blob SHA `eda2f4c11852f5e88f753a4174ffa4952fb14005` přesně odpovídá souboru v repozitáři. SHA-256 je `384521f1a47c5bf14e47445feb8950594d8735c58e8b48d43d0252f11abe50e2`.

EXIF uvádí Panasonic DMC-FZ7 a čas `2009-11-02 14:17:12`; jde o metadata moderního fotografického zachycení, nikoli historickou dataci hřbitova nebo náhrobků. Časově a tematicky snímek navazuje na položku 030 pořízenou téhož dne v 14:10:36.

Nejistota `URB-U-0082` byla rozšířena na položky 001–031. Nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvald – zbývá | 0 | 2 | 2 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **116** | **9** | **125** |

## Registr nejistot

- `open`: 47;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 82.

Systematické řešení nejistot je odloženo do závěrečné fáze.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 491 položek;
- zbývá 125 položek;
- kolekce `Rychvald` má zpracováno 31 z 33 položek, tedy všechny obsahové soubory;
- raw Drive soubor dávky 07 přesně odpovídá Git blobu a velikosti;
- dříve potvrzená položka 007 zůstává přesným duplikátem položky 002;
- registr používá součty 47/32/3/82;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Auditovat technické soubory `Thumbs.db` a `ZbThumbnail.info` v kolekci `Rychvald`.
- Po jejich auditu bude kolekce `Rychvald` dokončena a lze přejít na další nezpracovanou skupinu.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
