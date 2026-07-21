# AGENTS.md

## Účel projektu

Tento repozitář obsahuje výzkumná data a články o historicky nebo místně zajímavých místech v Rychvaldu.

Nejdůležitějším pravidlem projektu je dohledatelnost všech faktických tvrzení.

## Jazyk

- Veškeré články a výzkumné poznámky piš česky.
- Používej věcný a srozumitelný styl.
- Nepoužívej reklamní jazyk, dramatizaci ani nepodložené superlativy.

## Práce se zdroji

- Každé faktické tvrzení v článku musí mít citaci.
- Citace musí být bezprostředně za tvrzením, které podporuje.
- U kroniky nebo zpravodaje uváděj `source_id` a přesnou stránku.
- Chybějící informace nikdy nedoplňuj odhadem.
- Nečitelný nebo nejednoznačný text označ jako nejistý.
- Rozpory mezi prameny nezakrývej.
- Internetové zdroje používej až po vytěžení nahraných pramenů.
- Preferuj oficiální, archivní, knihovní, památkové a odborné zdroje.
- Wikipedie, sociální sítě a neozdrojované weby mohou být pouze vodítkem.
- Nejasnosti a rozpory se po vytěžení nahraných pramenů pokus ověřit v relevantních internetových zdrojích. Výsledek
  popiš jako potvrzení, částečné vyřešení nebo trvající nejistotu; původní varianty nemaž.
- Každý použitý internetový zdroj zapiš do `sources/index.yml` včetně URL a data přístupu.
- V oddílu Zdroje článku uváděj vedle `source_id` a lokátoru také přímý klikací odkaz na konkrétní PDF, TXT nebo webovou
  stránku. Čtenář nemá být nucen dohledávat dokument v adresářové struktuře.

## Úrovně jistoty

Používej tyto stavy:

- `verified`
- `partially_verified`
- `conflicting`
- `uncertain`
- `unverified`

Do publikovaného článku mohou být jako jistý fakt použita pouze tvrzení se stavem `verified`.

## Registr nejistot

- Autoritativní fronta nevyřešených otázek je `research/urbanek-archive/uncertainties.yml`.
- Každá nová podstatná nejistota dostane stabilní ID ve tvaru `URB-U-XXXX`.
- U nejistoty eviduj zdrojovou položku, typ, stav, prioritu, přesnou otázku, doklady a konkrétní následující krok.
- Podrobná poznámka může zůstat v OCR nebo klasifikačním souboru, ale musí být dohledatelná z centrálního registru.
- Při vyřešení původní záznam nemaž. Změň stav na `resolved` a doplň výsledek, nový doklad, datum a způsob ověření.
- Stavy registru jsou `open`, `in_progress`, `blocked`, `deferred`, `resolved` a `not_actionable`.
- Tvrzení navázané na otevřenou nebo odloženou nejistotu nesmí být prezentováno jako `verified`.
- Při předání práce do nového chatu musí být registr načten spolu se `STATUS.md` a `state.yml`.

## Práce s dokumenty

- Originální dokumenty v `sources/` neupravuj.
- Neměň jejich názvy nebo cesty bez závažného důvodu.
- Každý nový zdroj zaeviduj v `sources/index.yml`.
- U zdroje zaznamenej název, období, typ dokumentu, cestu k souboru, počet stran, čitelnost a známý stav práv.

## Inventáře importovaných souborů

- U každé položky fyzicky přítomné v repozitáři eviduj úplnou cestu od kořene repozitáře jako `repo_path` a její
  `git_blob_sha`. Samotný blob SHA nenahrazuje cestu, protože neobsahuje název ani umístění souboru.
- Původní archivní umístění může být vedeno samostatně jako `source_path` nebo `original_path`; nesmí být zaměněno za
  `repo_path`.
- Přímý odkaz na GitHub není autoritativní údaj a není nutné jej ukládat do každého řádku. V případě potřeby jej odvoď z
  repozitáře, refu nebo commitu a `repo_path`.
- U položek přítomných v repozitáři neukládej `drive_url`. Případné `drive_file_id` je pouze pomocné auditní metadata a
  nesmí nahrazovat `repo_path` ani `git_blob_sha`.
- `drive_url` ponechávej pouze u souborů záměrně vyloučených z importu nebo evidovaných jako chybějící v repozitáři,
  například se stavem `excluded` nebo `drive_listed_repo_missing`. U takové položky ponech `repo_path` a `git_blob_sha`
  prázdné.
- Každý inventář musí výslovně obsahovat `repo_status`, aby bylo zřejmé, zda položka existuje v repozitáři, byla vyloučena,
  nebo zůstává pouze v původním archivu.

## OCR a text zachycený v obraze

- OCR prováděj nejen u skenů článků, dokumentů a popisků, ale také u textu, který je součástí fotografované scény a může
  identifikovat nebo upřesnit zobrazený obsah.
- Za text ve scéně považuj zejména nápisy na budovách, vývěsní štíty, cedule, uliční tabule, pamětní desky, plakáty,
  transparenty, označení provozoven, vozidel a předmětů.
- Dokumentový text a text ve scéně eviduj odděleně, například jako `document_text` a `scene_text`; neslučuj je do jednoho
  přepisu bez označení původu.
- U textu ve scéně zaznamenej jeho přibližné umístění v obraze a k čemu se vztahuje, pokud je to z fotografie zřejmé.
- Strojový přepis vždy označ jako `machine_unverified`, dokud nebyl vizuálně zkontrolován proti originálu.
- Nečitelné znaky, neúplná slova a sporné interpretace výslovně označ; chybějící text nedoplňuj odhadem.
- Nápis ve fotografii může být vodítkem k identifikaci místa, osoby, organizace nebo události, ale sám o sobě se nesmí
  automaticky změnit na ověřené historické tvrzení.

## Práce s články

- Nový článek založ podle `articles/sablona.md`.
- Rozpracované články ukládej do `articles/rozpracovane/`.
- Do `articles/publikovane/` přesouvej pouze články po kontrole citací.
- Každý publikovaný článek přidej do hlavního `README.md`.
- Historii místa řaď chronologicky.
- Nejasnosti a rozpory uváděj v samostatné sekci.
- Současný stav místa musí mít vlastní zdroj.
- Geolokace musí mít uvedenou přesnost a metodu určení.

## Fotografie

U každého obrazového materiálu eviduj:

- popis,
- autora, pokud je znám,
- datum nebo přibližné období,
- původ,
- vlastníka,
- licenci nebo stav práv,
- případnou nejistotu identifikace.

Fotografie, mapy a jejich výřezy lze v projektu převzít i bez ověřené licence, pokud je to pro článek užitečné a uživatel
jejich převzetí schválil. U takového materiálu bezprostředně uveď původ, přesný lokátor, autora a držitele práv, pokud jsou
známi, a přesné označení **„neznámá práva“**. Materiál s neznámými právy neprezentuj jako volně publikovatelný ani volně
použitelný mimo projekt.

Převzatý obrazový soubor eviduj také v `images/README.md`. Originální dokument, ze kterého byl obraz vyčleněn, neupravuj.

## Git workflow

Projekt spravuje jeden autor.

- Běžné malé změny mohou být commitovány přímo do `main`.
- Každý commit má obsahovat jednu logickou změnu.
- Používej konkrétní zprávy commitů.
- Před commitem zkontroluj změněné soubory.
- Větve používej pro větší reorganizace nebo experimentální změny.
- Nikdy nemaž větší množství souborů bez výslovného pokynu uživatele.

Příklady commitů:

- `Add index of uploaded chronicles`
- `Extract places from chronicle volume 1`
- `Add research data for old school`
- `Draft article about old school`
- `Verify citations in old school article`

## Kontrola před dokončením článku

Ověř:

- každé faktické tvrzení má citaci,
- citace skutečně podporuje uvedené tvrzení,
- všechny citované zdroje existují,
- stránky nebo jiné lokátory jsou uvedeny,
- každá položka v oddílu Zdroje obsahuje přímý funkční odkaz na dokument nebo webovou stránku,
- rozpory mezi zdroji jsou zachovány,
- poloha není označena jako přesnější, než dovolují důkazy,
- fotografie a mapy mají uvedený původ, přesný lokátor, autora, držitele práv a licenci nebo označení „neznámá práva“,
- všechny podstatné otevřené nejistoty jsou v `research/urbanek-archive/uncertainties.yml`,
- text neobsahuje fakta vytvořená pouze odhadem AI.

Nejistota je platný výsledek výzkumu a nesmí být skryta.