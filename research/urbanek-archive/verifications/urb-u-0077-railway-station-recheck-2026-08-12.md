# URB-U-0077 – historická reprodukce „Nádraží“

Datum kontroly: 2026-08-12

## Otázka

Jaká stanice a lokalita je na reprodukci označené `Nádraží`, z jaké doby pochází a kdo je autorem či vydavatelem předlohy?

## 1. Přímá evidence archivního souboru

Kořenový soubor `19.jpg` (`urbanek-root-loose-001`) je digitální reprodukce historického černobílého obrazu s viditelným tištěným popiskem `Nádraží`.

Obraz zachycuje mimo jiné:

- nízkou podlouhlou stavbu vlevo;
- větší dvoupodlažní budovu ve střední až pravé části;
- cestu či příjezdovou komunikaci;
- nízké oplocení a bílé krajníky/sloupky;
- sloupy vedení;
- dvě osoby na cestě, jedna s malým vozíkem či podobným nákladem;
- vodní příkop nebo malý tok v levém popředí.

V obraze není bezpečně čitelný název stanice ani jiný jednoznačný lokalizační nápis.

Soubor má rozměr 979 × 688 px a embedded obecný EXIF čas `2016:03:17 14:07:04`; jde o metadata digitální reprodukce, nikoli datum historické scény.

## 2. Nově nalezený zdrojový soubor knihy Jaromíra Urbánka

V připojeném Google Drive byla nalezena složka `kniha Rychvald včera a dnes ve fotografii`, která obsahuje zdrojový soubor:

`Rychvald_vcera_a_dnes_ve_fotografii.lyx`

Dokument má na titulní straně:

- `RYCHVALD`
- `včera a dnes ve fotografii`
- autor `Jaromír Urbánek`.

V části `Jak vznikala tato kniha` autor píše, že vycházel mimo jiné z fotografických alb, která do roku 1971 kompletoval Vilém Chrobáček, a že pro knihu používal fotografie z archivu MÚ Rychvald, Státního okresního archivu Karviná, památkové péče, kronik Sokola, škol a ZUŠ i materiály poskytnuté občany. Současně výslovně uvádí, že u mnoha fotografií již není možné určit autora. Text je datován `V Rychvaldu, květen 2012. Jaromír Urbánek`.

README k obnovené sazbě potvrzuje, že LyX používá relativní odkazy na původní očíslované obrazové podklady a že tyto obrázky nejsou pro sazbu duplikovány.

## 3. Železniční kapitola a kandidátní obrazy

Zdroj LyX obsahuje samostatnou část `Železniční nádraží` a odkazuje na pět relevantních historických souborů v podsložce `14. část průmysl a železniční zastávky`:

- `363.jpg` — `„Nádraží“ u železničního přejezdu u rybníku Skučák známé pod názvem „Ozvajch“ (z německého Ausweiche – výhybna). Nejstarší dochovaný obrázek asi z počátku 20. století.`
- `364.jpg` — domek bývalé výhybny po roce 1915, na snímku z konce 60. let;
- `365.jpg` — dvě původní budovy nádraží `Rychvald místo`, obraz z roku 1940–41, s archivně uváděným německým nápisem `Ort Reichwaldau`;
- `366.jpg` — nádraží `Rychvald místo` na obrazu z roku 1970;
- `367.jpg` — nádraží `Rychvald zámek`, obraz z konce 60. let.

Toto rozlišení je důležité: samotné označení `Nádraží` v kořenovém souboru neznamená automaticky `Rychvald-místo` ani `Rychvald-zámek`.

## 4. Přímé obrazové porovnání 19.jpg ↔ 363.jpg

Kořenový `19.jpg` byl přímo porovnán se všemi pěti železničními podklady 363–367 pomocí SIFT feature matching a následného RANSAC homografického ověření.

Výsledek pro `363.jpg`:

- kvalitní Lowe-ratio shody: **3142**;
- geometricky konzistentní RANSAC inliery: **3139–3140** podle prahu opakované kontroly;
- odhadnutá projektivní transformace je prakticky jen posun přibližně **+3 px v ose x a −7 px v ose y**;
- korelace překryvu po zarovnání: **0,9981**;
- průměrná absolutní jasová odchylka po zarovnání přibližně 4 úrovně šedi.

Pro ostatní kandidáty 364–367 vznikly pouze jednotky dobrých shod a žádná srovnatelná geometrická struktura.

`19.jpg` a `363.jpg` proto představují **stejný podkladový historický obraz**, pouze v mírně odlišném ořezu/rekompresi. Nejde o podobné stavby ani o odhad podle motivu; jde o přímou geometrickou shodu obrazu.

Rozměry podporují stejný závěr:

- kořenový `19.jpg`: 979 × 688 px;
- knižní `363.jpg`: 976 × 679 px.

## 5. Identifikace stanice a lokality

Díky přímé shodě s `363.jpg` je kořenový `19.jpg` bezpečně identifikován jako obraz:

**„Nádraží“ / výhybna u železničního přejezdu u rybníku Skučák, místně zvaná `Ozvajch`, z německého `Ausweiche` (výhybna).**

Není to obraz nádraží `Rychvald-místo` ani `Rychvald-zámek`.

Toto zařazení je navíc slučitelné se starší obecní Pamětní knihou, která mezi třemi rychvaldskými železničními body uvádí `Rychvald-zámek`, `Rychvald-místo` a `Rychvald-zastávka`, přičemž poslední označuje také jako `Vyhýbka` a uvádí její zrušení v roce 1916.

Urbánkův pozdější knižní text používá pro tutéž lokalitu místní název `Ozvajch` a vysvětluje jej z německého `Ausweiche`.

## 6. Datace historického obrazu

Zdrojový LyX přímo označuje `363.jpg` jako:

`Nejstarší dochovaný obrázek asi z počátku 20. století.`

To je nejpřesnější nalezená explicitní datace samotného obrazu. Je formulována jako přibližná (`asi`) a musí tak být zachována.

Starší Pamětní kniha uvádí, že `Vyhýbka` byla roku 1916 zrušena. Tento údaj je důležitý pro dějiny objektu, ale sám nedokazuje datum expozice fotografie; budova a zařízení mohly být fotografovány i později. Proto se z něj nevytváří umělý přesný terminus ante quem pro fotografii nad rámec Urbánkova popisku.

EXIF kořenového souboru z roku 2016 a metadata knižního `363.jpg` z roku 2012 jsou data digitálních kopií a nejsou historickou datací.

## 7. Publikační a archivní provenience

Je doloženo, že tentýž obraz byl Jaromírem Urbánkem zařazen do obrazové publikace / sazebního projektu `Rychvald včera a dnes ve fotografii` jako soubor `363.jpg` s výše uvedeným popiskem.

To umožňuje bezpečně uvést:

- **pozdější editor/autor knižního kontextu:** Jaromír Urbánek;
- **knižní/sazební kontext:** `Rychvald včera a dnes ve fotografii`;
- **autorská datace pracovního textu:** Rychvald, květen 2012.

Nelze však z toho určit původního fotografa ani první vydání fotografie.

Urbánek v úvodu knihy uvádí několik zdrojových institucí a soukromé poskytovatele společně, ale `363.jpg` nemá individuální kredit. Není proto bezpečné tvrdit, že právě tento snímek pochází například z MÚ Rychvald, SOkA Karviná, Chrobáčkových alb nebo od konkrétního občana.

Geocachingový listing `RYCHVALD - Nádraží` později používá historickou fotografii a připisuje ji webu Hornického klubu. Listing také popisuje Ozvajch u Skučáku. Bez přímého získání původního obrázku z tehdejšího webu Hornického klubu však nebyla v této kontrole prokázána pixelová totožnost jeho vloženého obrázku s `19.jpg`/`363.jpg`. Tento webový kredit se proto nepovyšuje na původní provenienci archivní fotografie.

## 8. Negativní kontroly

- Historický železniční snímek na straně 29 publikace `Rychvald 1305–2005` není totožný s kořenovým `19.jpg`.
- Stejnojmenný `19.jpg` ve složce `Fotografie knihy Rychvald včera a dnes` je moderní barevný letecký snímek a s kořenovým `19.jpg` nesouvisí.
- Obrazy `365`, `366` a `367`, které jsou v LyXu explicitně označeny jako `Rychvald-místo` nebo `Rychvald-zámek`, se s kořenovým `19.jpg` geometricky neshodují.

Tím se odstraňuje dřívější riziko záměny mezi třemi různými rychvaldskými železničními místy.

## 9. Částečně vyřešené atributy

1. **exact_station_and_locality**
   - hodnota: `Nádraží` / výhybna u železničního přejezdu u rybníku Skučák, místně `Ozvajch` (`Ausweiche`);
   - stav: přímá geometrická shoda `19.jpg` s knižním `363.jpg` + explicitní knižní popisek.

2. **relationship_to_book_asset**
   - hodnota: kořenový `19.jpg` a knižní `14. část průmysl a železniční zastávky/363.jpg` jsou dvě digitální reprezentace stejného historického obrazu;
   - stav: přímo ověřeno obrazovým porovnáním.

3. **historical_image_date**
   - hodnota: `asi z počátku 20. století`;
   - stav: explicitní přibližná datace v Urbánkově knižním popisku, nikoli technická metadata.

4. **later_publication_context**
   - hodnota: Jaromír Urbánek, `Rychvald včera a dnes ve fotografii`, pracovní/sazební text datovaný květen 2012;
   - stav: přímo doloženo zdrojovým LyX dokumentem.

## 10. Zůstává otevřené

- původní fotograf;
- přesný rok nebo datum pořízení historického snímku;
- původní negativ, pohlednice, tisk nebo jiný nosič;
- první publikace nebo první známé užití fotografie;
- individuální archivní fond, sbírka nebo soukromý poskytovatel, z něhož Jaromír Urbánek získal právě tento obraz;
- inventární číslo nebo signatura případného archivního originálu;
- zda geocachingový/hornicko-klubový obraz je přesně tentýž podklad a odkud jej Hornický klub získal.

## Stav

`URB-U-0077` zůstává **open**, ale jeho hlavní lokalizační část je vyřešena. Otevřená je už především původní fotografická provenience a přesnější datace.

## Zdroje

### Archiv projektu
- `research/urbanek-archive/collections/root-loose-files-batch-01.yml`
- `sources/index.d/urbanek-root-loose-files-01.yml`
- `sources/osobni-archiv-jaromira-urbanka/19.jpg`

### Připojený Google Drive
- složka `kniha Rychvald včera a dnes ve fotografii`
- `Rychvald_vcera_a_dnes_ve_fotografii.lyx`
- `README_Rychvald_LyX.txt`
- `14. část průmysl a železniční zastávky/363.jpg`
- srovnávací `364.jpg`, `365.jpg`, `366.jpg`, `367.jpg`

### Historický kontext
- Pamětní kniha obce Rychvaldu 1922–1935, oddíl o Košicko-bohumínské dráze
- specializované železniční databáze pro samostatné kontrolní údaje k Rychvald-místo a Rychvald-zámek
- archivovaný listing geocache `RYCHVALD - Nádraží` jako sekundární webová stopa, nikoli jako doklad původní provenience obrazu

## Bezpečná formulace

Archivní `19.jpg` nezachycuje nádraží Rychvald-místo ani Rychvald-zámek. Přímé obrazové porovnání prokazuje, že jde o stejný historický snímek jako `363.jpg` v Urbánkově knize `Rychvald včera a dnes ve fotografii`. Její popisek jej identifikuje jako „Nádraží“ u železničního přejezdu u rybníku Skučák, místně zvané Ozvajch podle německého Ausweiche – výhybna, a datuje snímek přibližně na počátek 20. století. Původní fotograf ani individuální zdroj fotografie však v knize uvedeni nejsou; Urbánek výslovně poznamenává, že u mnoha použitých historických fotografií již autora nelze určit.