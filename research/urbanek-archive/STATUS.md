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
| zpracováno | 455 | 20 | **475** |
| zbývá | 132 | 9 | **141** |
| celý aktuální snapshot | **587** | **29** | **616** |

Dokončeno je deset kolekcí. Kolekce `Rychvald` je rozpracována v rozsahu 15 z 33 položek.

## Rychvald – dávka 03

Zpracovány byly soubory `P1010069.JPG`, `P1010070.JPG`, `P1010071.JPG`, `P1010072.JPG` a `P1010114.JPG`:

- `P1010069.JPG` je moderní reprodukce historické ilustrované vícepohledové pohlednice či karty s výrazným titulem „Pozdrowienie z Rychwaldu“; menší popisky nejsou přepisovány tam, kde není čtení zcela jisté;
- `P1010070.JPG` je reprodukce starší černobílé fotografie či pohlednice velké sakrální stavby s věží a čitelným nápisem „PRAVDA VÍTĚZÍ“; přesná stavba, lokalita a datum nejsou určeny pouze podle architektury;
- `P1010071.JPG` zachycuje dokumentární stránku s ručně kresleným místopisným plánem, číslem „- 14 -“ a nadpisem „Místopis kolem a po r. 1900.“;
- `P1010072.JPG` zachycuje obdobnou stránku s číslem „- 14 -“ a nadpisem „Místopis před r. 1900.“;
- `P1010114.JPG` zachycuje stránku rukopisného historického textu s číslem „- 25 -“; úplný kurzivní přepis a historická interpretace jsou odloženy, aby nebyly doplňovány nejisté znaky, jména či letopočty.

Všech pět souborů přesně odpovídá Drive i Git blobům. Všechny uvádějí Panasonic DMC-TZ3. `P1010069.JPG` a `P1010070.JPG` mají metadata 28. února 2010 12:38:10 až 12:38:56, `P1010071.JPG` a `P1010072.JPG` 27. dubna 2010 11:11:45 až 11:12:51 a `P1010114.JPG` 1. září 2010 15:17:19. Tyto časy jsou evidovány jako metadata moderního zachycení, nikoli jako data historických předloh.

Viditelné nadpisy, nápisy a čísla stran jsou evidovány doslovně pouze tam, kde je čtení bezpečné. Bez dalšího neprokazují autora, vydavatele, původní dataci, historickou přesnost ani přesnou identitu zobrazených objektů. Mezi pěti položkami dávky 03 není přesná binární duplicita.

Nejistota `URB-U-0082` byla rozšířena na položky 001–015. Nová nejistota nevznikla.

## Zbývající skupiny a položky

| Skupina | Obsahové | Technické | Celkem |
|---|---:|---:|---:|
| Rychvald – zbývá | 16 | 2 | 18 |
| fotodokument mimo `den po dešti` | 41 | 2 | 43 |
| fotografie, které nebyl použité pro knihu ani kalendář | 28 | 1 | 29 |
| novinové články 1903–1925 | 16 | 2 | 18 |
| popopo | 31 | 2 | 33 |
| **Celkem** | **132** | **9** | **141** |

## Registr nejistot

- `open`: 47;
- `deferred`: 0;
- `resolved`: 32;
- `not_actionable`: 3;
- celkem: 82.

Systematické řešení nejistot je odloženo do závěrečné fáze. Položky zůstávají `open`; workflow odložení je nepřevádí do stavu `deferred`.

## Kontrola konzistence

- součet skupin v kořenovém inventáři je 616 položek;
- zpracovaný rozsah je 475 položek;
- zbývá 141 položek;
- kolekce `Rychvald` je zpracována v rozsahu 15 z 33 položek;
- všech pět Drive souborů dávky 03 přesně odpovídá Git blobům;
- v dávce 03 není přesná binární duplicita mezi pěti vybranými cestami;
- dříve potvrzená položka 007 zůstává přesným duplikátem položky 002;
- registr používá součty 47/32/3/82;
- PR zůstává otevřený draft a není žádostí o sloučení;
- absence hlášených CI status checks není úspěšně proběhlý test.

## Aktuální krok

- Aktivní fáze: `full_archive_indexing`.
- Další dávka: `P1010115.JPG`, `P1010116.JPG`, `P1010117.JPG`, `Rychvald2009 003.jpg` a `Rychvald2009 004.jpg`.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení bez výslovného rozhodnutí.
