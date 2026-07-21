# AGENTS.md

## Účel a jazyk

Repozitář obsahuje výzkumná data a články o historicky nebo místně zajímavých místech v Rychvaldu. Nejdůležitější je dohledatelnost všech faktických tvrzení.

- Piš česky, věcně a srozumitelně.
- Nepoužívej reklamní jazyk, dramatizaci ani nepodložené superlativy.

## Práce se zdroji

- Každé faktické tvrzení v článku musí mít citaci bezprostředně za tvrzením.
- U kroniky nebo zpravodaje uváděj `source_id` a přesnou stránku.
- Chybějící informace nedoplňuj odhadem; nečitelný nebo nejednoznačný text označ jako nejistý.
- Rozpory mezi prameny nezakrývej.
- Internetové zdroje používej až po vytěžení nahraných pramenů. Preferuj oficiální, archivní, knihovní, památkové a odborné zdroje; Wikipedie, sociální sítě a neozdrojované weby mohou být pouze vodítkem.
- Nejasnosti a rozpory se pokus ověřit v relevantních internetových zdrojích. Výsledek popiš jako potvrzení, částečné vyřešení nebo trvající nejistotu; původní varianty nemaž.
- Každý použitý internetový zdroj zapiš do `sources/index.yml` včetně URL a data přístupu.
- V oddílu Zdroje článku uváděj vedle `source_id` a lokátoru také přímý klikací odkaz na konkrétní PDF, TXT nebo webovou stránku.

## Úrovně jistoty

Používej stavy `verified`, `partially_verified`, `conflicting`, `uncertain` a `unverified`. Jako jistý fakt lze v publikovaném článku použít pouze tvrzení se stavem `verified`.

## Registr nejistot

- Autoritativní registr je `research/urbanek-archive/uncertainties.yml`.
- Každá podstatná nejistota dostane stabilní ID `URB-U-XXXX`.
- Eviduj zdrojovou položku, typ, stav, prioritu, přesnou otázku, doklady a následující krok.
- Podrobná poznámka může zůstat v OCR nebo klasifikačním souboru, ale musí být dohledatelná z registru.
- Vyřešený záznam nemaž; změň stav na `resolved` a doplň výsledek, doklad, datum a způsob ověření.
- Stavy registru jsou `open`, `in_progress`, `blocked`, `deferred`, `resolved` a `not_actionable`.
- Tvrzení navázané na otevřenou nebo odloženou nejistotu nesmí být prezentováno jako `verified`.
- Při předání práce načti registr spolu se `STATUS.md` a `state.yml`.

## Dokumenty a inventáře

- Originální dokumenty v `sources/` neupravuj a bez závažného důvodu neměň jejich názvy ani cesty.
- Každý nový zdroj zaeviduj v `sources/index.yml`: název, období, typ, cesta, počet stran, čitelnost a známý stav práv.
- Autoritativním pracovním úložištěm je Git repozitář.
- U každé položky eviduj `repo_path`, `repo_status` a identitu obsahu jako `git_blob_sha` přímo v inventáři nebo v navázaném ověřovacím manifestu.
- Původní archivní umístění může být vedeno jako `source_path` nebo `original_path`; nezaměňuj je za `repo_path`.
- Přímý odkaz na Git není autoritativní údaj; lze jej odvodit z repozitáře, refu nebo commitu a `repo_path`.
- Do aktivních inventářů neukládej identifikátory ani odkazy na dřívější pracovní úložiště.
- Položky pilotu fyzicky přítomné ve větvi mají `repo_status: repo_verified`.
- Pokud `Thumbs.db` obsahuje náhled bez odpovídajícího samostatného plného souboru, eviduj plný originál jako **chybějící**. Náhled není samostatný zdrojový obraz ani náhrada originálu.
- Absence plného souboru není otevřená otázka. Otevřená může zůstat pouze identifikace, datace, lokalizace nebo interpretace náhledu.

## OCR a text v obraze

- OCR prováděj u skenů, dokumentů, popisků i textu ve fotografované scéně, který může identifikovat nebo upřesnit obsah.
- Za scénický text považuj zejména nápisy na budovách, vývěsní štíty, cedule, uliční tabule, pamětní desky, plakáty, transparenty a označení provozoven, vozidel či předmětů.
- `document_text` a `scene_text` eviduj odděleně.
- U scénického textu zaznamenej přibližné umístění v obraze a vztah k zobrazenému obsahu.
- Strojový přepis označ jako `machine_unverified`, dokud nebyl vizuálně zkontrolován.
- Nečitelné znaky, neúplná slova a sporné interpretace označ; text nedoplňuj odhadem.
- Nápis ve fotografii je vodítko, nikoli automaticky ověřené historické tvrzení.

## Články

- Nový článek založ podle `articles/sablona.md`.
- Rozpracované články ukládej do `articles/rozpracovane/`; do `articles/publikovane/` přesouvej pouze články po kontrole citací.
- Každý publikovaný článek přidej do hlavního `README.md`.
- Historii místa řaď chronologicky; nejasnosti a rozpory uváděj samostatně.
- Současný stav místa musí mít vlastní zdroj.
- Geolokace musí uvádět přesnost a metodu určení.

## Fotografie

U každého obrazového materiálu eviduj popis, autora, datum nebo období, původ, vlastníka, licenci či stav práv a případnou nejistotu identifikace.

Fotografie, mapy a výřezy lze v projektu převzít i bez ověřené licence, pokud to uživatel schválil. Uveď původ, přesný lokátor, autora a držitele práv, pokud jsou známi, a označení **„neznámá práva“**. Takový materiál neprezentuj jako volně publikovatelný nebo použitelný mimo projekt.

Převzatý obrazový soubor eviduj také v `images/README.md`; původní dokument neupravuj.

## Git workflow

Projekt spravuje jeden autor.

- Běžné malé změny mohou být commitovány přímo do `main`.
- Jeden commit má obsahovat jednu logickou změnu a konkrétní zprávu.
- Před commitem zkontroluj změněné soubory.
- Větve používej pro větší reorganizace nebo experimenty.
- Nikdy nemaž větší množství souborů bez výslovného pokynu uživatele.

## Kontrola před dokončením článku

Ověř, že:

- každé tvrzení má citaci a citace je skutečně podporuje;
- všechny citované zdroje existují a mají stránku nebo jiný lokátor;
- každá položka v oddílu Zdroje obsahuje přímý funkční odkaz;
- rozpory jsou zachovány;
- poloha není přesnější, než dovolují důkazy;
- fotografie a mapy mají původ, lokátor, autora, držitele práv a licenci nebo „neznámá práva“;
- všechny podstatné otevřené nejistoty jsou v registru;
- text neobsahuje fakta vytvořená pouze odhadem AI.

Nejistota je platný výsledek výzkumu a nesmí být skryta.
