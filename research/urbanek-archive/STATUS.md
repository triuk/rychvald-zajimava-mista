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
| zpracováno | 470 | 20 | **490** |
| zbývá | 117 | 9 | **126** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je deset kolekcí. Kolekce `Rychvald` je rozpracována v rozsahu 30 z 33 položek.

## Rychvald – dávka 06

Zpracovány byly soubory `Zp1109 340.jpg`, `Zp1109 379.jpg`, `Zp1109 382.jpg`, `Zp1109 390.jpg` a `zzz-satiny 255.jpg`:

- `Zp1109 340.jpg` zachycuje jednokolejnou železniční trať, cihlovou budovu těsně vedle koleje a železniční vozidlo v dálce; přesná lokalita a funkce budovy nejsou z obrazu určovány;
- `Zp1109 379.jpg` zachycuje vodní plochu a informační označení s bezpečně čitelnými texty „PŘÍRODNÍ REZERVACE“ a „Přírodní rezervace Skučák“;
- `Zp1109 382.jpg` a `Zp1109 390.jpg` jsou dva rozdílné záběry stejného zařízení u vodní plochy s řadou kulatých nádob či kádí a malými čluny; širší záběr obsahuje také zelené mechanické zařízení. Funkce zařízení není podle vzhledu domýšlena;
- `zzz-satiny 255.jpg` je široký hřbitovní pohled. Podle shodných výrazných tvarových detailů je v ose cesty zachycen tentýž kamenný kříž jako na položkách 019 a 020, nyní v širším kontextu. Přítomné osoby nejsou identifikovány a přesná identita hřbitova či historická datace pomníku zůstávají neověřeny.

Všech pět raw souborů bylo staženo z kanonické Drive složky a jejich velikost i vypočtený Git blob SHA přesně odpovídají souborům v repozitáři. Všechny uvádějí Panasonic DMC-FZ7. První čtyři mají EXIF časy 21. října 2009 od 15:29:22 do 15:47:28, poslední snímek 2. listopadu 2009 14:10:36. Tyto časy jsou metadata moderního fotografického zachycení, nikoli historická data zobrazených objektů.

Mezi pěti položkami dávky 06 není přesná binární duplicita. Položky 028 a 029 jsou samostatné záběry stejného zařízení; položka 030 je samostatný širší záběr téhož pomníku jako položky 019 a 020.

Nejistota `URB-U-0082` byla rozšířena na položky 001–030. Nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvald – zbývá | 1 | 2 | 3 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **117** | **9** | **126** |

## Registr nejistot

- `open`: 47;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 82.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 490 položek;
- zbývá 126 položek;
- kolekce `Rychvald` je zpracována v rozsahu 30 z 33 položek;
- všech pět raw Drive souborů dávky 06 přesně odpovídá Git blobům a velikostem;
- v dávce 06 není přesná binární duplicita mezi pěti vybranými cestami;
- položky 028 a 029 jsou dva rozdílné snímky stejného zařízení u vodní plochy;
- položka 030 zobrazuje v širším kontextu tentýž kamenný kříž jako položky 019 a 020;
- dříve potvrzená položka 007 zůstává přesným duplikátem položky 002;
- registr používá součty 47/32/3/82;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další obsahová dávka kolekce `Rychvald`: `zzz-satiny 258.jpg`.
- Po posledním obsahovém souboru zbývá audit technických souborů `Thumbs.db` a `ZbThumbnail.info`.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
