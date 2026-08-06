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
| zpracováno | 445 | 20 | **465** |
| zbývá | 142 | 9 | **151** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je deset kolekcí. Kolekce `Rychvald` je rozpracována v rozsahu 5 z 33 položek.

## Rychvald – dávka 01

Zpracovány byly soubory `Budova úřadu 003.jpg`, `Budova úřadu 005.jpg`, `Cudlín 033.jpg`, `Cudlín 035.jpg` a `Cudlín 037.jpg`:

- první dva snímky zachycují dvě strany třípodlažní budovy s přímo čitelným nápisem „MĚSTSKÝ ÚŘAD“;
- tři soubory `Cudlín` jsou časově těsně navazující pohledy na upravenou dlážděnou veřejnou plochu s prosklenou budovou, obchody, květinami, kamenným vodním či výtvarným prvkem a obytnými domy v pozadí;
- mezi pěti soubory není přesná binární duplicita;
- pozdější cesta `Kopie - Budova úřadu 005.jpg` má v Git stejný blob SHA jako `Budova úřadu 005.jpg` a bude vedena jako samostatná inventární položka, nikoli jako další nezávislý obrazový důkaz.

Všech pět souborů přesně odpovídá Drive i Git blobům. První dvojice má rozměry 2394 × 1796 px a EXIF z 2. září 2008; druhá trojice má 2048 × 1360 px a EXIF z 28. srpna 2009. Všechny uvádějí Panasonic DMC-FZ7.

Zařazení do adresáře `Rychvald` a jméno `Cudlín` jsou archivní metadata. Přesná lokalita veřejné plochy, význam jména `Cudlín`, autorství, původní účel sady a práva nejsou z obrazů samostatně prokázány; jsou vedeny pod `URB-U-0082`.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvald – zbývá | 26 | 2 | 28 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **142** | **9** | **151** |

## Registr nejistot

- `open`: 47;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 82.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 465 položek;
- zbývá 151 položek;
- kolekce `Rychvald` je zpracována v rozsahu 5 z 33 položek;
- všech pět Drive souborů přesně odpovídá Git blobům;
- mezi pěti soubory dávky není přesná binární duplicita;
- známá přesná duplicita `Budova úřadu 005.jpg` / `Kopie - Budova úřadu 005.jpg` je evidována;
- registr používá součty 47/32/3/82;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `Cudlín 041.jpg`, `Kopie - Budova úřadu 005.jpg`, `P1010066.JPG`, `P1010067.JPG` a `P1010068.JPG`.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
