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
| zpracováno | 465 | 20 | **485** |
| zbývá | 122 | 9 | **131** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je deset kolekcí. Kolekce `Rychvald` je rozpracována v rozsahu 25 z 33 položek.

## Rychvald – dávka 05

Zpracovány byly soubory `Rychvald2009 005.jpg`, `Rychvald2009 008.jpg`, `Zp0707 090.jpg`, `Zp1109 005.jpg` a `Zp1109 082.jpg`:

- `Rychvald2009 005.jpg` zachycuje moderní světlou budovu se vstupem pod širokou stříškou, částečně zakrytou vzrostlou zelení; přesná instituce a lokalita nejsou z obrazu určeny;
- `Rychvald2009 008.jpg` zachycuje malou červenou dřevěnou sakrálně působící stavbu s křížem na štítu vedle mohutného stromu; přesná identita, zasvěcení a datace nejsou určeny;
- `Zp0707 090.jpg` zachycuje vícepatrovou světlou budovu s červenou taškovou střechou, vikýři a řadou balkonů; funkce a přesná identita budovy nejsou z obrazu samostatně doloženy;
- `Zp1109 005.jpg` zachycuje sportovní areál s oválnou běžeckou dráhou, travnatou plochou, fotbalovou brankou, osvětlením a oploceným víceúčelovým hřištěm;
- `Zp1109 082.jpg` zachycuje oranžovo-žlutou budovu s rampou a oploceným venkovním prostorem s dětskými herními prvky. Přítomné osoby nejsou identifikovány a funkce budovy není domýšlena.

Všech pět lokálních raw souborů přesně odpovídá Git blobům a velikostem evidovaným v repozitáři; položky byly současně dohledány v kanonické složce na Drive. Všechny uvádějí Panasonic DMC-FZ7. EXIF časy jsou 11. června 2007 15:18:10, 1. září 2009 09:17:26 a 09:18:39, 23. září 2009 15:20:20 a 26. září 2009 15:38:27. Tyto časy jsou metadata moderního fotografického zachycení, nikoli historická data objektů.

Mezi pěti položkami dávky 05 není přesná binární duplicita.

Nejistota `URB-U-0082` byla rozšířena na položky 001–025. Nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvald – zbývá | 6 | 2 | 8 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **122** | **9** | **131** |

## Registr nejistot

- `open`: 47;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 82.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 485 položek;
- zbývá 131 položek;
- kolekce `Rychvald` je zpracována v rozsahu 25 z 33 položek;
- pět lokálních raw souborů dávky 05 přesně odpovídá Git blobům a velikostem a jejich názvy/identity byly ověřeny v kanonické Drive složce;
- v dávce 05 není přesná binární duplicita mezi pěti vybranými cestami;
- dříve potvrzená položka 007 zůstává přesným duplikátem položky 002;
- registr používá součty 47/32/3/82;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `Zp1109 340.jpg`, `Zp1109 379.jpg`, `Zp1109 382.jpg`, `Zp1109 390.jpg` a `zzz-satiny 255.jpg`.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
