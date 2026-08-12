# Stav připravenosti na systematické řešení nejistot

Datum: 2026-08-12

## Výsledek přípravy

Archivní indexace je pro aktuální Git snapshot dokončena a další běh už nemá pokračovat v běžném inventárním zpracování.

- indexováno: **616 / 616 položek**;
- obsahové soubory: **587 / 587**;
- technické soubory: **29 / 29**;
- dokončené kolekce: **15 / 15**;
- zbývá k indexaci: **0**;
- otevřené nejistoty: **53**;
- vyřešené: **32**;
- `not_actionable`: **3**;
- celkem evidováno: **88**.

Revize všech 53 otevřených položek již proběhla v `uncertainty-prioritization-review-2026-08-11.md`. Nebyla nalezena žádná dvojice otevřených položek, kterou by bylo bezpečné sloučit jako totožnou otázku bez ztráty atributů nebo historie evidence.

Machine-readable pracovní fronta je nyní v:

`research/urbanek-archive/uncertainties/resolution-queue.yml`

## Jak navazovat

Další práce má začínat načtením:

1. `research/urbanek-archive/state.yml`;
2. `research/urbanek-archive/uncertainties/index.yml`;
3. `research/urbanek-archive/uncertainties/resolution-queue.yml`;
4. konkrétního `open-*.yml` souboru pro aktivní ID;
5. všech již existujících verifikačních zpráv a zdrojových indexů uvedených u daného ID.

Není třeba znovu inventarizovat všech 616 souborů ani znovu prioritizovat celý registr, pokud nevznikne nový snapshot archivu nebo se neobjeví důkaz, který pořadí zásadně mění.

## První vlna

První vlna obsahuje 15 přímo rychvaldských položek s vysokým projektovým přínosem.

### Již mají samostatný výzkumný checkpoint, ale zůstávají open

- `URB-U-0036`
- `URB-U-0038`
- `URB-U-0044`
- `URB-U-0049`
- `URB-U-0053`
- `URB-U-0062`
- `URB-U-0063`
- `URB-U-0065`
- `URB-U-0067`
- `URB-U-0075`
- `URB-U-0077`

`research checkpoint` neznamená `resolved`. Znamená pouze, že už existuje samostatná zdrojová kontrola a část atributů byla zpřesněna.

### Aktivní cíl

`URB-U-0078` — ozbrojená skupina u tabule `MĚSTO RYCHVALD`, archivně spojovaná s říjnem 1938.

Při přípravné kontrole byla opravena důležitá chyba vstupní evidence: na zdrojovém obrázku jsou **čtyři** viditelní muži, nikoli pět. Tato oprava je přímé vizuální zjištění. Datum, jednotka, totožnost osob a provenience zůstávají otevřené.

Samostatný přípravný checkpoint:

`research/urbanek-archive/verifications/urb-u-0078-preparation-recheck-2026-08-12.md`

### Následující fronta první vlny

1. `URB-U-0079` — fond, signatura, účel a úplnost tajného seznamu SNB Fryštát z 10. 7. 1945;
2. `URB-U-0081` — přesné vydání a stránky fotografovaného `Českého slova` z roku 1938;
3. `URB-U-0085` — bibliografické zařazení novinových výstřižků 1903–1925.

Pořadí není absolutní: pokud pramen nalezený pro jeden cíl přímo řeší jiný, má se využít, ale závěry zůstávají pod oddělenými stabilními ID.

## Paralelní obnova chybějících plných originálů

Technická větev zůstává oddělena od historického výzkumu:

- `URB-U-0086` — 9 odlišných cache-only obrazových obsahů;
- `URB-U-0088` — 16 odlišných cache-only obrazových obsahů.

Exact-name hledání v připojeném Drive bylo bez výsledku. Další směr je obrazová shoda pod jiným názvem nebo jiné úložiště/záloha. Náhled v cache není náhradou plného originálu.

## Průřezové položky

`URB-U-0073`, `URB-U-0076`, `URB-U-0082`, `URB-U-0083`, `URB-U-0084` a `URB-U-0087` se nemají uzavírat jedním širokým tvrzením. Při výzkumu je nutné řešit konkrétní atributy a v případě potřeby vytvářet užší navazující položky.

## Pravidla pro uzavírání

- Viditelný text, metadata souboru, archivní filename, sekundární popisek a historická interpretace jsou různé vrstvy důkazu.
- Filename nebo název složky je archivní atribuce, ne automaticky ověřený historický fakt.
- Osoby se neurčují pouze podle obličeje; jednotka, národnost ani hodnost se neurčují pouze podle uniformy nebo výzbroje.
- Bezpečně vyřešený dílčí atribut lze během práce evidovat pod `partially_resolved_attributes`, zatímco položka zůstává `open`.
- Před přesunem položky do `resolved` nesmí zmizet žádný materiální nevyřešený atribut. Pokud původní otázka obsahuje další podstatnou nejistotu, musí být vyřešena nebo převedena do propojeného open ID.
- Negativní hledání není samo o sobě historickým důkazem neexistence.
- Přímá obrazová shoda může řešit identitu podkladového obrazu, ale sama neřeší autora, přesné datum ani původní nosič.

## Stav pro handoff

Repozitář je po tomto checkpointu **resolution-ready**. Další aktivní krok je systematický výzkum `URB-U-0078`; indexace se považuje za uzavřenou pro současný snapshot.
