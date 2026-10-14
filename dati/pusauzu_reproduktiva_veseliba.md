# Pusaudžu seksuālā un reproduktīvā veselība Latvijā: laikrindas (2000–2025)

Datu fails: `pusauzu_reproduktiva_veseliba.csv`. Tas ir garajā formātā ar kolonnām `indicator,code,year,sex,age,value,unit,geo,source_url,notes`. Dati apkopoti 2026. gada 14. oktobrī.

**Kodējums:**
- **Koda prefikss** norāda sadaļu: `A_` = HBSC, `B_` = ESPAD, `C` = dzimstība, `D` = aborti, `E_` = STI/HIV, `F_` = HPV vakcinācija.
- **sex:** `F` = sievietes/meitenes, `M` = vīrieši/zēni, `T` = kopā.
- **geo:** `LV` = Latvija, `EU27` = ES-27, `HBSC_avg` = HBSC valstu vidējais, `EUEEA30_21` / `EU_EEA31` = ES/EEZ (ECDC).

**Principi:**
- Neviena vērtība nav izdomāta vai interpolēta.
- Aprēķinātās vērtības ir skaidri marķētas ar "DERIVED" vai "APRĒĶINĀTS".
- Nedrošās vērtības ir atzīmētas piezīmēs ar "UNCERTAIN", "NEDROŠS" vai "verify".

## A. HBSC – Latvijas skolēnu veselības paradumu pētījums (15 gadus veci skolēni)

**Pieejamie apsekojuma viļņi:** 2001/02, 2005/06, 2009/10, 2013/14, 2017/18 un 2021/22. CSV gads ir viļņa beigu gads, piemēram, 2002 = 2001/02. Latvijā 2021/22 viļņa lauka darbs notika 2022./2023. mācību gadā.

**Avoti:**
- **2001/02, 2005/06 un 2009/10:** dati nolasīti no PVO HBSC starptautisko ziņojumu (2004, 2008, 2012) diagrammu datu etiķetēm. Etiķetes saskaņotas ar valsti pēc to novietojuma PDF lapā, tāpēc tās ir drukātas vērtības, nevis tabulu dati.
- **2013/14–2021/22:** HBSC Data Browser (vērtības noapaļotas līdz veseliem procentiem).
- **Latvijas kopējās vērtības (T):** SPKC nacionālie ziņojumi par 2017/18 un 2022/23.
- **Agrīnā dzimumdzīves uzsākšana:** Költő et al. 2025, *Int J Public Health*, papildu tabulas.

**Definīcijas:**
- Seksuālās veselības jautājumus uzdod tikai 15 gadus veciem skolēniem.
- Prezervatīva, kontracepcijas tablešu un "ne viena, ne otra" lietošanu rēķina tikai no tiem, kuriem jau bijis dzimumakts.
- "Agrīna uzsākšana" nozīmē dzimumaktu pirms 14 gadu vecuma, t. i., 13 gados vai agrāk. Šo rādītāju rēķina no *visiem* 15-gadīgajiem, un dati nav svērti. HBSC vidējais šim rādītājam ir apvienotā izlase, nevis valstu vidējais.

**Definīciju un datu izmaiņas starp viļņiem:**
- 2001/02 kontracepcijas tabletes atsevišķi netika ziņotas. Ir tikai rādītājs "vismaz viena metode", kurā pārtrauktais dzimumakts nav ieskaitīts.
- Tablešu rādītājs pieejams no 2005/06.
- Rādītājs "ne prezervatīvs, ne tabletes" pieejams tikai 2017/18 un 2021/22.
- Dati par pārtraukto dzimumaktu un "nekādu metodi" Latvijai nav publicēti nevienā atrastajā avotā.
- 2009/10 un 2013/14 Latvijas nacionālajos ziņojumos nav nodaļas par seksuālo uzvedību.

**Neatbilstības starp avotiem:**
- **2002, prezervatīvs:** starptautiskajā ziņojumā meitenēm ir 77,3 % un zēniem 81,0 %. Nacionālajos ziņojumos šīs vērtības ir otrādi, tātad dzimumi samainīti vietām. Vērtības atzīmētas kā nedrošas.
- **2014, prezervatīvs:** Data Browser dod meitenēm 69 % un zēniem 71 %, bet nacionālais ziņojums 78,5 % un 77,8 %. Atšķirības iemesls nav zināms, vērtības atzīmētas kā nedrošas.
- **Rādītājs "bijis dzimumakts":** starptautiskie un nacionālie avoti visos viļņos sakrīt.

**2025/26. vilnis:** lauka darbs notika 2026. gadā. Līdz 2026. gada 14. oktobrim rezultāti nebija publicēti: nav starptautiskā ziņojuma, nav jaunu datu Data Browser, nav SPKC publikācijas. Rezultāti gaidāmi ap 2027.–2028. gadu.

## B. ESPAD

Standarta ESPAD anketā seksuālās veselības moduļa nav. Vienīgais saistītais jautājums ir neobligātais 2019. gada jautājums par dzimumaktu bez prezervatīva pēdējo 12 mēnešu laikā, un Latvija to izmantoja.
- Avots ir viens zinātnisks raksts (PMC12841082).
- Raksta tabulā zēnu un meiteņu kolonnu secība bija jāsecina, tāpēc vērtības jāpārbauda.
- Tas ir viens datu punkts, nevis laikrinda.

## C. Pusaudžu dzimstība

**Primārais avots ir Eurostat:**
- `demo_frate`: dzimstības koeficients 15–19 gadus vecām sievietēm uz 1000 sievietēm. Eurostat sākotnēji to dod uz vienu sievieti, tāpēc vērtība pareizināta ar 1000. Latvijai 2000–2024, ES-27 2001–2024.
- `demo_fagec`: dzīvi dzimušo skaits pēc mātes vecuma 10–14 un 15–19 gadi, 2000–2024.

**Sekundārais avots ir Pasaules Banka (`SP.ADO.TFRT`):** tie ir ANO *World Population Prospects* modelēti novērtējumi. Tie atšķiras no Eurostat, piemēram, Latvijai 2000. gadā Pasaules Bankas vērtība ir 20,1, bet Eurostat 24,1. Diagrammai ieteicams lietot Eurostat; Pasaules Bankas sērija iekļauta tikai salīdzināšanai.

## D. Aborti pusaudžu vecumā

**Avoti:**
- **Eurostat `demo_fabort`:** abortu skaits pēc vecuma (<15 un 15–19) 2000–2020. Pēc 2020. gada vecuma sadalījuma nav.
- **CSP `VSM090`** (dati no SPKC): inducēto (legālo un medicīnisko) abortu skaits pēc vecuma ≤14, 15–17 un 18–19 gadi, 2010–2025. No 2019. gada pieejams arī visu abortu skaits, kurā ieskaitīti spontānie, neattīstījušās grūtniecības u. c.
- **SPKC `MCH060`:** aborti uz 1000 dzīvi dzimušajiem pēc vecuma, 2010–2025. Tā ir attiecība, nevis rādītājs uz iedzīvotājiem.

**Eurostat 2019. gada kļūda:** Eurostat 2019. gada vērtības pēc vecuma ir kļūdainas, jo tās nobīdītas par vienu vecuma grupu: 15–19 gadu grupā uzrādīti 39 aborti, 20–24 gadu grupā 135. Pareizās vērtības pēc CSP datiem ir <15 = 0 un 15–19 = 174. Eurostat rindas ir saglabātas ar atzīmi "NEDROŠS" un korekcijas piezīmi.

**Aprēķinātie rādītāji uz 1000 sievietēm:** SPKC jaunākiem gadiem tādus nepublicē. CSV rindās ar atzīmi DERIVED rādītājs aprēķināts šādi: aborti / (vidējais sieviešu skaits 1. janvārī gadā t un t+1) × 1000. Iedzīvotāju dati ņemti no CSP IRD041 un IRD081. Metode precīzi atkārto SPKC 2012. gada publicētos skaitļus (15–17 g.: 4,6; 18–19 g.: 14,4). Tie nav oficiāli rādītāji.

**ES salīdzinājums:** nav iekļauts, jo Eurostat ES kopsumma abortiem nav pilnīga un nav salīdzināma.

## E. STI un HIV jauniešiem

**Avoti:**
- **ECDC Surveillance Atlas:** pašreizējā datu kopa (`CUR`) un arhivētā datu kopa `2019.STI`. Sifiliss, gonoreja un hlamīdijas 15–24 gadu vecumā 2000–2024, ieskaitot 15–19 un 20–24 gadu grupas un sadalījumu pēc dzimuma.
- **Skaitļi, kas aprēķināti no procentiem:** ECDC publicē dzimuma un vecuma sadalījumu procentos. Skaitļi aprēķināti kā procents × kopskaits, un visi rezultāti ir veseli skaitļi.
- **SPKC ziņojumi:** daļa vērtību nolasīta no diagrammām, tāpēc to ticamība ir vidēja. Atzīmēts piezīmēs.

**HIV:** jaunu diagnožu skaits 15–19 un 20–24 gadu vecumā pieejams tikai 2014–2024. Pirms 2014. gada ECDC atlantā Latvijas gadījumu dati ir nepilnīgi. SPKC lieto citas vecuma grupas (15–17 un 18–29 gadi). HIV dati pēc dzimuma jauniešu vecuma grupās nav pieejami.

**Hlamīdijas:**
- Ap 2009. gadu notiek ziņošanas pārrāvums. Skaits strauji pieaug un sieviešu īpatsvars kāpj no ~40 % līdz ~80 %. Visticamāk, tas atspoguļo testēšanas un ziņošanas izmaiņas, nevis reālas saslimstības pārmaiņas.
- SPKC un ECDC skaitļi būtiski atšķiras.

**ES/EEZ salīdzinājums:**
- Divas ECDC valstu kopas, kas nav pilnībā salīdzināmas: ar Lielbritāniju līdz 2013. gadam un bez tās no 2014. gada.
- Hlamīdijām nav ES/EEZ datu par 2014–2019.
- Ļoti mazo skaitu dēļ (piemēram, sifiliss 2020–2024 ir 5–12 gadījumi gadā) sadalījumi ir nestabili.

## F. HPV vakcinācija

Ir trīs nesalīdzināmas definīcijas:
1. **PVO "programmas aptvere"** (`PRHPV*`): 12 gadus veci. Meitenēm 2010–2025, zēniem 2022–2025.
   - 2022. gadā zēnu saucējs aptver vairākas kohortas, tāpēc vērtība nav salīdzināma ar citiem gadiem.
   - 2021. gadā pirmās un pēdējās devas skaitītāji, šķiet, samainīti vietām.
2. **PVO "līdz 15 gadu vecumam"** (`15HPV*`): kohortas rekonstrukcija meitenēm no 2013. gada.
3. **SPKC "savlaicīgums"** (vakcinēti līdz 12 gadu vecumam), 2019–2025, un **SPKC "imunizācijas līmenis"**, 2019–2022. Imunizācijas līmenī ieskaitīta arī vecāku bērnu vakcinācija.

**2024.–2025. gads:** PVO un SPKC vērtības nesakrīt, tāpēc par primāro avotu ieteicams izmantot SPKC. 2024. gadā SPKC pilna kursa savlaicīguma rādītājs strauji krītas; iespējama metodikas maiņa, bet tā nav apstiprināta.

## G. Jauniešu zināšanu aptaujas

Salīdzināmas laikrindas nav atrastas. Papardes zieds un SKDS ir veikuši atsevišķus pētījumus:
- 2016. gadā – vecāku aptauja;
- 2018. gadā – jauniešu tiešsaistes aptauja;
- 2023. gadā – pedagogu aptauja.

Šiem pētījumiem atšķiras mērķgrupas un jautājumi, tāpēc tie CSV nav iekļauti.

## Galvenie avoti

- **HBSC:**
  - Data Browser: https://data-browser.hbsc.org/
  - PVO ziņojumi: Currie et al. 2004; *Inequalities in Young People's Health* 2008; *Social Determinants of Health and Well-being* 2012
  - SPKC nacionālie ziņojumi: https://spkc.gov.lv/lv/media/4267/download un 2022/23. gada ziņojums
  - Költő et al. 2025: doi 10.3389/ijph.2025.1607711
- **Eurostat:** demo_frate, demo_fagec, demo_fabort – https://ec.europa.eu/eurostat/databrowser/
- **Pasaules Banka:** https://data.worldbank.org/indicator/SP.ADO.TFRT
- **CSP:** VSM090, IRD041, IRD081 – https://data.stat.gov.lv/
- **SPKC statistikas datubāze:** MCH060 – https://statistika.spkc.gov.lv/
- **ECDC Surveillance Atlas:** https://atlas.ecdc.europa.eu/public/index.aspx
- **PVO imunizācijas dati:** https://immunizationdata.who.int/
- **SPKC Epidemioloģijas biļeteni:** https://www.spkc.gov.lv/lv/media/{17096, 18339, 18852, 21687, 23429, 25529}/download

Precīzs avota URL katrai vērtībai ir norādīts CSV kolonnā `source_url`.
