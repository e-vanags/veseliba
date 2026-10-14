# Bērnu un pusaudžu veselība Latvijā: laikrindas un salīdzinājums ar starptautisko vidējo (2002–2024)

Datu fails: `berni_pusaudzi_veseliba.csv` (≈3000 rindu, 101 rādītāja kods), garajā formātā ar kolonnām `indicator,code,year,sex,age,value,unit,geo,source_url,notes` – tāpat kā `pusauzu_reproduktiva_veseliba.csv`. Apkopots 2026. gada 14. oktobrī.

**Kodējums:**
- **Koda prefikss:** `HBSC_` = Skolēnu veselības paradumu pētījums (11, 13, 15 g.); `COSI_`/`SPKC_` = bērnu antropometrija (7–9 g., mērīts); `ESPAD_` = 16 g. skolēni; `GYTS_` = 13–15 g.; `PISA_` = 15 g.; `SUICIDE_` = Eurostat nāves cēloņi; `HL_` = veselībpratība; `ORAL_` = zobu veselības pētījums.
- **sex:** `F` meitenes, `M` zēni, `T` kopā. **age:** viens vecums (11, 13, 15) vai intervāls (11-15, 13-15, 15-19, 7-9).
- **geo:** `LV`; `HBSC_avg` (HBSC valstu nesvērtais vidējais); `COSI_avg`, `COSI_min`/`COSI_max` (valstu diapazons); `ESPAD_avg` (32 valstu trenda vidējais), `ESPAD_avg_all` (visu konkrētā viļņa valstu vidējais); `OECD_avg`; `EU27_2020`, `EU28`.

**Principi:** nekas nav izdomāts vai interpolēts. Aprēķinātās vērtības (piem., 2002. g. liekā svara stabiņu summa) piezīmēs marķētas. Definīciju maiņas un nedrošības ir piezīmju kolonnā; dažādas definīcijas glabātas ar **atšķirīgiem kodiem**, lai diagrammā tās nesajauktu.

## A. HBSC – Latvijas skolēnu veselības paradumu pētījums (11, 13, 15 g.)

**Viļņi:** 2001/02, 2005/06, 2009/10, 2013/14, 2017/18, 2021/22. CSV `year` = viļņa beigu gads (2022 = 2021/22). Latvijā 2021/22 viļņa lauka darbs faktiski notika 2022./2023. mācību gadā (pēc COVID-19 pārtraukuma), tāpēc Latvijas "2022" ir apm. gadu vēlāks nekā vairākumam valstu.

**Avoti:**
- **2013/14–2021/22:** HBSC Data Browser (https://data-browser.hbsc.org/), oficiālā datu datne `wp-content/uploads/csvs/data.csv`; katram rādītājam `source_url` norāda attiecīgā rādītāja lapu. Vērtības noapaļotas līdz veseliem procentiem. Latvijai pieejams tikai meitenes (F) un zēni (M); HBSC vidējam ir arī kopējais (T).
- **2001/02, 2005/06, 2009/10:** PVO HBSC starptautiskie ziņojumi (Currie et al. 2004, 2008, 2012). Vērtības nolasītas no valstu stabiņu diagrammu datu etiķetēm, piesaistot etiķeti valstij pēc tās novietojuma PDF lapā (teksta koordinātas), un izlases kārtā pārbaudītas vizuāli. PDF lappuses numurs norādīts piezīmēs.
- **HBSC vidējais** (`HBSC_avg`) ir nesvērts dalībvalstu/reģionu vidējais konkrētajā vilnī; valstu sastāvs mainās (no ~35 valstīm/reģioniem 2002. g. līdz 40+ vēlākajos viļņos), tāpēc tas nav stingri salīdzināms laikā.

**Definīciju izmaiņas un pārrāvumi (svarīgi diagrammai):**
- **Liekais svars:** 2002–2010 ziņojumos izmantoti IOTF (Cole) robežpunkti (`HBSC_OWOB_IOTF`); no 2014 – PVO 2007 augšanas references (`HBSC_OWOB`). PVO robežas dod ievērojami augstāku izplatību, tāpēc **2010→2014 lēciens ir definīcijas, nevis reāla izmaiņa**. Abas sērijas jārāda atsevišķi. 2002. gadā ziņoti tikai 13 un 15 g.; vērtība = "pre-obese" + "obese" stabiņu summa (APRĒĶINĀTS). ĶMI ir pašu ziņots (augums/svars), kas parasti nenovērtē izplatību.
- **Fiziskā aktivitāte:** 2002 – ≥60 min ≥5 dienas nedēļā (`HBSC_MVPA_5D`); no 2006 – katru dienu (7/7) (`HBSC_MVPA_DAILY`). Nav salīdzināmi.
- **Dzīves apmierinātība:** 2002–2010 – % ar "augstu" apmierinātību (Cantril ≥6, `HBSC_LIFESAT_HIGH`); 2014–2022 Data Browser dod vidējo punktu skaitu 0–10 (`HBSC_LIFESAT_MEAN`). Divas atsevišķas sērijas.
- **Smēķēšana un alkohols:** līdz 2010 – lietošana vismaz reizi nedēļā (`HBSC_CIG_WEEKLY`, `HBSC_ALC_WEEKLY`); 2014–2022 – lietošana pēdējās 30 dienās (`HBSC_CIG30`, `HBSC_ALC30`). Nepārtraukta sērija ir **"piedzēries ≥2 reizes mūžā"** (`HBSC_DRUNK2_LIFE`, 2002–2022).
- **Nepārtrauktas sērijas 2002–2022** (vienāda definīcija): brokastis darbadienās, augļi katru dienu, saldinātie dzērieni katru dienu, vairākas veselības sūdzības (≥2 simptomi biežāk nekā reizi nedēļā), iebiedēšana skolā (≥2–3 reizes mēnesī), skolas darba slodzes spiediens. Dārzeņi un saldumi: 2002 + 2014–2022 (2006/2010 ziņojumos nav).
- **Tikai 2018/2022:** problemātiska sociālo mediju lietošana (SMDS ≥6 no 9), kiberiebiedēšana, intensīvs tiešsaistes kontakts. **Tikai 2022:** WHO-5 labbūtības indekss (vidējais 0–100), vientulība (lielākoties/vienmēr), e-cigaretes.
- **Zobu tīrīšana >1 reizi dienā:** 2002–2010 no starptautiskajiem ziņojumiem; Data Browser šo rādītāju nesatur (2014–2022 – sk. sadaļu F).
- **Miegs:** HBSC kodols nemēra miega ilgumu; Data Browser ir tikai "grūtības aizmigt biežāk nekā reizi nedēļā" (`HBSC_SLEEPDIFF`). Par miega ilgumu sk. sadaļu F.

## B. COSI – mērīts liekais svars 7–9 gadus veciem bērniem

**Avoti:** PVO COSI ziņojumi (1.–2. kārtas ieviešanas ziņojums; Wijnhoven et al. 2014 *BMC Public Health*; 3. kārtas ziņojums; 4., 5., 6. kārtas ziņojumu pielikuma tabulas) un SPKC nacionālie ziņojumi "Bērnu antropometrisko parametru un skolu vides pētījums" (2008, 2010, 2012/13, 2015/16, 2018/19 – web.archive.org kopijas; 2022/23 – ppdb.mk.gov.lv). `year` = mācību gada beigu gads (2008, 2010, 2013, 2016, 2019, 2023).

**Definīcijas – nejaukt:**
- `COSI_OW`/`COSI_OB`: PVO 2007 reference, ĶMI-vecumam > +1 SD (liekais svars, ieskaitot aptaukošanos) / > +2 SD (aptaukošanās) – starptautiskā COSI definīcija.
- `SPKC_OW`/`SPKC_OB`: tā pati PVO reference, bet procentiļu robežas (>85. / >97. procentile) – SPKC nacionālā metode; dod citus skaitļus (piem., 2018/19 aptaukošanās 7 g.: 10,1 % pēc procentilēm pret 8,8 % pēc SD).
- `COSI_OW_IOTF`/`COSI_OB_IOTF`: IOTF robežas (2., 4.–6. kārta).
- COSI vidējais publicēts tikai no 4. kārtas (2015–17); 1.–3. kārtai tikai valstu diapazons (6–9 g.). 6. kārta nav tieši salīdzināma ar 5. (cits valstu sastāvs). COSI vidējā `year` ir kārtas beigu gads (2017, 2020, 2024), Latvijai – faktiskā mācību gada beigas (2016, 2019, 2023); diagrammā salīdzināt pa kārtām.

**Nedrošības:** 2012/13 PVO vērtības nolasītas no diagrammas (veseli skaitļi). PVO 1.–4. kārtā Latvijai publicēti tikai zēni/meitenes, ne kopējais. Vēlākajos SPKC trendu attēlos 2008. g. vērtības pa dzimumiem attiecas uz visiem pirmklasniekiem (7 un 8 g.) – CSV izmantoti 2008. g. ziņojuma 7-gadīgo dati. Divas aizdomīgas PVO tabulu šūnas (9 g. kopējais = viena dzimuma vērtība) izlaistas. SPKC 2022/23 ziņojumā 9 g. meitenēm pretrunīgi 21,9 % un 24,8 % – izmantots tabulas 21,9 %. Mērījumu laiks mainījies (2010 un 2023 daļa bērnu jau 8 g.; analīze ierobežota ar 7,0–7,9 g.).

**Galvenais:** 7 g. zēniem liekais svars (PVO SD) ~24–25 % 2008–2019, 22,7 % 2022/23; 9 g. zēniem 30,5 % (2016) un 29,9 % (2023), aptaukošanās 14,8 % (2023). COSI vidējais 6. kārtā: 25 % liekais svars, 11 % aptaukošanās.

## C. ESPAD (16 g.) un GYTS (13–15 g.)

**Avoti:** ESPAD 2024 ziņojums un EUDA Excel avota tabulas (trendi 1995–2024 pa dzimumiem; espad.org atrasts caur web.archive.org); ESPAD 2019 ziņojums; SPKC ESPAD 2024 faktu lapa (spkc.gov.lv/lv/media/24107). GYTS Latvija 2002, 2007, 2011, 2014, 2019 – PVO NCD Microdata faktu lapas; 2024 – SPKC faktu lapa (spkc.gov.lv/lv/media/23423).

**Definīcijas un piezīmes:**
- Latvija piedalījās ESPAD 1995, bet trendu datos tā nav – 1995. g. rindu nav. Latvijas 2015. g. dati avotā atzīmēti kā "ierobežoti salīdzināmi". 2024. g. jaukts tiešsaistes/papīra režīms.
- Kopš 2019 cigarešu jautājums neietver e-cigaretes; pievienota arī sērija "cigaretes un/vai e-cigaretes" (`ESPAD_CIG_OR_ECIG30`).
- `ESPAD_SM_PROB` un `ESPAD_GAMING_PROB` **nav SMDS** – tas ir 3 jautājumu pašnovērtējuma indekss (Holstein 2014), "augsts risks" = 2–3 punkti. Nav salīdzināms ar HBSC `HBSC_PSMU`.
- 32 valstu 2024. g. kopējās vērtības avotā noapaļotas līdz veseliem skaitļiem.
- GYTS 2024 "jebkāds tabaks" ietver arī karsējamo tabaku (plašāka definīcija); atsaucība kritusies līdz 61 %. SPKC faktu lapā zēnu e-cigarešu lietošana pretrunīga (17,0 % tabulā, 17,9 % tekstā) – izmantots tabulas skaitlis. GYTS starptautiskā vidējā nav.

## D. Pašnāvības 15–19 gadu vecumā (Eurostat)

- `SUICIDE_RATE`: `hlth_cd_acdr2`, jēlais mirstības koeficients uz 100 000 (X60–X84, Y87.0), 2011–2023, LV un EU27_2020; arī 10–14 g.
- `SUICIDE_RATE_3Y`: `hlth_cd_ycdr2`, 3 gadu slīdošais vidējais – **ieteicams diagrammai**, jo Latvijā gadā ir tikai 2–15 gadījumi.
- `SUICIDE_N`: `hlth_cd_aro`, gadījumu skaits Latvijā.
- `SUICIDE_RATE_OLD`: `hlth_cd_acdr` (1994–2010, vecā metodoloģija; ES agregāti EU28/EU27_2020 no 2002) – nav stingri salīdzināms ar sēriju no 2011.
- Latvijas koeficients 15–19 g. bija ~2× virs ES (1996: 18,3; 2014: 16,7; 3 g. vidējais 2016: 10,6 pret ES 4,5), bet 2021–2023 noslīdējis zem ES līmeņa (3 g. vidējais 2023: 2,8 pret 4,3). Mazo skaitļu dēļ tas jāinterpretē piesardzīgi.

## E. PISA 2022 (15 g.)

OECD valsts piezīme par Latviju (oecd.org caur web.archive.org): piederība skolai, vientulība skolā, zema dzīves apmierinātība, digitālo ierīču traucējumi matemātikas stundās, iebiedēšana, drošības sajūta. Viens datu punkts (daži arī 2018), ne laikrinda.

## F. Miegs, zobu tīrīšana, spēles, veselībpratība

- **Miegs** (tikai Latvija): HBSC nacionālie ziņojumi 2017/18 (spkc.gov.lv/lv/media/4267, arhīva kopija) un 2022/23 (ppdb.mk.gov.lv). Ilgums aprēķināts no pašu norādītajiem gulētiešanas/celšanās laikiem; "pietiekams" = NSF ieteikums (≥9 h 11 un 13 g., ≥8 h 15 g.). 2013/14 (RSU tēzes) izmantota cita robeža (<8 h) – nav salīdzināms. Starptautiska salīdzinājuma nav (HBSC 2021/22 starptautiskajos sējumos miega nav; PISA 2022 miegu nemēra).
- **Zobu tīrīšana >1 reizi dienā** (`HBSC_TOOTH2`): Latvija un HBSC vidējais 2002–2018 no starptautiskajiem ziņojumiem (2002–2010 vērtības neatkarīgi iegūtas divreiz un sakrīt). `HBSC_TOOTH2_LVNAT`: Latvijas nacionālā sērija 2002–2022 (nacionālā svēršana, var atšķirties par 0,1–0,5 pp.). 2022. g. HBSC vidējā nav. `ORAL_TOOTH2_RSU` – cits instruments (RSU zobu veselības pētījums), nav HBSC.
- **Datorspēles:** Latvija 2022. g. neiekļāva HBSC izvēles moduli par spēlēm, tāpēc problemātiskas spēlēšanas vērtības Latvijai nav (`HBSC_GAMING_*` vidējie ir tikai 12 valstīm). Nacionālā sērija "spēlē ≥3 h dienā" 2006–2022 – jautājuma formulējums paplašināts (2022 ietver viedtālruņus), tāpēc 2022. g. lēciens daļēji ir definīcijas efekts. 2022. g. nacionālajā ziņojumā kļūda (15 g. zēni 2018 nedēļas nogalē 30,6 % vietā 60,6 %) – izmantots 2018. g. ziņojuma skaitlis. Problemātiskai spēlēšanai izmantot ESPAD 2024.
- **Problemātiska sociālo mediju lietošana:** HBSC Data Browser (`HBSC_PSMU`, pa vecumiem) un nacionālā ziņojuma kopējais (`HBSC_SMU_PROB`: 2022 LV 7,7 % pret HBSC vidējo 11 %).
- **Veselībpratība:** bērnu/pusaudžu datu Latvijai **nav** (Latvijas HBSC 2022/23 ziņojumā šī moduļa nav, Latvija nepiedalījās HLS19). Iekļautas divas tikai pieaugušo rindas (`HL_ADULT_LIMITED`; 2019/20 n=102 – ļoti maza izlase; 2025 – sekundārs avots).

## Galvenās nepilnības

- HBSC 2025/26 viļņa rezultāti vēl nav publicēti (gaidāmi ~2027).
- Latvijai HBSC Data Browser nedod kopējo (T) vērtību – tikai meitenes/zēni.
- Nav starptautiska vidējā: miegam, zobu tīrīšanai 2022, GYTS, veselībpratībai.
- Liekā svara, fiziskās aktivitātes, dzīves apmierinātības un smēķēšanas/alkohola HBSC sērijās ir definīciju pārrāvumi (sk. sadaļu A).

## Spilgtākie atradumi (kur Latvija ir sliktāk par vidējo vai tendence pasliktinās)

1. **Iebiedēšana skolā – pastāvīgi ~2× virs vidējā kopš 2002.** 13 g. 2022: meitenes 23 %, zēni 20 % pret HBSC vidējo 12 %/12 %; 15 g. 17 %/16 % pret 8 %/9 %. **Kiberiebiedēšana** 13 g. meitenēm 29 % pret 17 %. PISA 2022: iebiedēti 29 % pret OECD 20–21 %.
2. **Pašvērtētā veselība – viena no zemākajām.** "Teicama" veselība 15 g. meitenēm 2022: 8 % pret 23 % vidēji; zēniem 23 % pret 40 %.
3. **Psihiskās veselības straujš pasliktinājums 2018→2022, īpaši meitenēm.** Vairākas veselības sūdzības 15 g. meitenēm 58 % → 72 % (vidēji 66 %); nervozitāte 13 g. meitenēm 29 % → 55 % (vidēji 45 %); nomāktība 15 g. meitenēm 38 % → 52 % (vidēji 44 %). Dzīves apmierinātība 15 g. meitenēm 6,3 (vidēji 6,8).
4. **Vientulība un miegs.** Vientuļas lielāko daļu laika/vienmēr: 15 g. meitenes 36 % pret 28 %, zēni 20 % pret 13 %. Grūtības aizmigt 15 g. meitenēm 45 % pret 37 % (2014: 23 %). Tikai 32 % skolēnu darbdienās guļ ieteikto laiku; 13 g. meitenēm 15 %.
5. **Augļi un dārzeņi – ļoti zems patēriņš.** Augļi katru dienu 15 g. meitenēm 2022: 16 % (2018: 26 %) pret 34 % vidēji; 11 g. ~23–24 % pret 42–47 %. Dārzeņi 15 g. ~24–25 % pret 34–39 %.
6. **Brokastis – straujš kritums.** 13 g. meitenes, kas brokasto katru darbdienu: 72 % (2002) → 56 % (2014) → 39 % (2022), vidēji 43 %.
7. **E-cigaretes, īpaši meitenēm.** HBSC 2022, 15 g.: pēdējās 30 dienās meitenes 31 %, zēni 25 % pret 20 %/18 %; mūžā 48 % pret 32 %. GYTS 13–15 g.: 9,1 % (2011) → 21,9 % (2024); meitenēm 13,5 % → 26,7 % (2019→2024). Cigaretes 15 g. joprojām virs vidējā (20 %/18 % pret 15 %/15 %).
8. **Datorspēles un azartspēles (ESPAD 2024).** Problemātiska spēlēšana 26,9 % pret 21,6 % (zēni 37,4 %); azartspēles pēdējos 12 mēn. 28,9 % pret 23,3 % (meitenēm 16,8 % → 25,9 % kopš 2019); sociālo mediju problēmu pašvērtējums 50,7 % pret 47,4 %.
9. **Zobu tīrīšana – ilgstoši zem vidējā.** Vairāk nekā reizi dienā 15 g. zēni: 41 % (2018) pret 55 % vidēji; nacionāli 2022 zēniem tikai 47,9 %.
10. **Liekais svars pusaudžiem pieaug.** HBSC (PVO def.) 15 g. meitenes 10 % (2014) → 16 % (2022), 13 g. zēni 24 % → 29 % – Latvija no krietni zem vidējā (2002–2010) pietuvojusies vidējam. COSI: 9 g. zēniem 29,9 % liekais svars un 14,8 % aptaukošanās (2022/23).

**Pozitīvas tendences (kontekstam):** saldināto dzērienu patēriņš ~2× zem vidējā; alkohols un piedzeršanās strauji samazinājušies (ESPAD 2024 alkohols 30 d.: 30,3 % pret 43 %); pašnāvību koeficients 15–19 g. 2021–2023 zem ES līmeņa.
