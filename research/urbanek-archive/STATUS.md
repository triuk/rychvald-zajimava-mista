# Stav zpracování archivu Jaromíra Urbánka

## Kontext

- Repozitář: `triuk/rychvald-zajimava-mista`
- Větev: `agent/import-urbanek-pilot`
- Zdroj: `sources/osobni-archiv-jaromira-urbanka/`
- Původ: **Z osobního archivu p. Jaromíra Urbánka.**
- Originály se nepřejmenovávají, nepřesouvají ani neupravují.

Autoritativní předání tvoří `AGENTS.md`, tento soubor, `state.yml`, `uncertainties.yml` a plán příslušné kolekce.

## Etapy

| Kolekce / etapa | Stav |
|---|---|
| Import originálů | dokončen s chybějícími technickými cache |
| Rychvaldské větrné mlýny | klasifikace a první OCR dokončeny |
| Články z Českého slova | první OCR i druhá vizuální kontrola dokončeny |
| Ochotníci rychvald | audit a klasifikace dokončeny; první OCR probíhá |
| fotodokument/den po dešti | čeká |
| Nálet na Ostravu 1944 | čeká |
| Pull request | čeká |

## Ochotníci rychvald

- Inventář: 63 položek — 60 JPEG, 1 DOC a 2 technické cache.
- Ve větvi je 62 položek; chybí pouze `Thumbs.db`.
- Všech 63 položek bylo klasifikováno nebo technicky auditováno.
- Plán: `research/urbanek-archive/collections/ochotnici-rychvald-processing-plan.yml`.

### Dokončené textové výstupy

- Nativní extrakce: `061`.
- První OCR: `001`, `004`, `010`, `011`, `012`, `013`, `014`, `023`, `032–033`, `039`, `042`, `047`.
- Položka `009` je pouze kontrolní detail k `010` a nebude mít duplicitní přepis.

### Otevřené nejistoty kolekce

- `URB-U-0024`: chybějící `Thumbs.db` ve větvi.
- `URB-U-0025`: plné originály dvou obrazů známých jen z cache.
- `URB-U-0026`: rozpor v obsazení Fabiana.
- `URB-U-0027`: rozdílné počty účastníků soutěže (`3915` a přibližně `3960`).

Centrální registr nyní obsahuje 18 otevřených, 3 odložené, 5 vyřešených a 1 neakční položku; celkem 27.

## Následující krok

1. Přepsat `urbanek-ochotnici-027`, výstřižek **„Jaké jsou naše vesnické soubory?“**.
2. Poté zpracovat `028` a `019` jako jeden přímo navazující článek z časopisu Těšínsko.
3. Ruční věnování na `028` vést jako samostatnou textovou vrstvu.
