# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Oprávnění k použití pro projekt bylo potvrzeno.
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.

## Draft pull request

- PR: [#1 – Import and classify Jaromír Urbánek archive (pilot + CČS batch)](https://github.com/triuk/rychvald-zajimava-mista/pull/1)
- Stav: otevřený draft; sloučení nebylo vyžádáno.

## Dokončený pilot

Pilot obsahuje 144 obsahových a 15 technických souborů, celkem 159 položek. Všechny jsou ve větvi; 11 plných originálů je známo pouze z náhledů v cache.

## Kolekce CČS

Rozsah: 200 JPEGů + 1 `Thumbs.db` = 201 položek.

Dokončeno je sedmnáct pětičlenných dávek, tedy `urbanek-ccs-001` až `085`:

- zpracováno, Git-ověřeno, vizuálně klasifikováno a indexováno: **85 položek**;
- zbývá: **116 položek**.

### Zjištění dávky 17

Dávka `urbanek-ccs-081` až `085` pokračuje v sérii slavnostní volby a jmenování archivně připisované Gabrielu Chrobáčkovi.

- `081` je skupinový portrét několika dospělých a dítěte. Archivní název uvádí syna Jaromíra, snachu Milenu, dceru Miluši, manželku a useknuté `paní S…`; osoby ani vztahy nejsou obrazem potvrzeny.
- `082–085` zachycují navazující gratulace, předávání květin a formální skupiny s duchovním nesoucím řetěz nebo insignii.
- Obrazová návaznost podporuje společnou slavnostní sérii, nikoli jména, rodinné vztahy, konkrétní úřad ani přesné pořadí jednotlivých úkonů.
- Useknuté jméno `paní S…` nebylo rekonstruováno.

Pracovní soubory:

- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-inventory-17.csv`;
- `research/urbanek-archive/collections/historie-cirkve-ceskoslovenske-batch-17.yml`;
- `sources/index.d/urbanek-ccs-17.yml`;
- rozšířený `research/urbanek-archive/uncertainties/open-12.yml`.

## Registr nejistot

- `open`: 34;
- `resolved`: 31;
- `not_actionable`: 3;
- celkem: 68.

Dávka 17 nepřidala nové ID; rozšířila `URB-U-0062` o rodinný portrét, gratulace, květiny, rodinné vztahy a useknuté jméno.

## Kontrola konzistence

- pilot a kolekce CČS jsou odděleny;
- aktuální stav je 85 zpracovaných a 116 zbývajících položek;
- registr používá součty 34/31/3/68;
- GitHub dosud nevrátil hlášené CI status checks.

## Aktuální krok

- Následující položky: `urbanek-ccs-086` až `090`.
- Očekávané archivní soubory: `10.jpg`, `11.jpg`, `12.jpg`, `13.jpg` a `14  Gratulace manželce.jpg`.
- `Thumbs.db` v podsložce `10 Kalendář 2015` musí být před uzavřením kolekce auditován.
- PR zůstává draft a nesmí být označen jako připravený ke sloučení.
