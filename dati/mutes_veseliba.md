# Skolēnu mutes veselība Latvijā – kariess, sīlanti, paradumi (1993–2023)

Datu fails: `mutes_veseliba.csv` (90 rindas). Kolonnas ir tādas pašas kā citos šīs mapes failos: `indicator,code,year,sex,age,value,unit,geo,source_url,notes`. Visiem kodiem ir prefikss `ORAL_`. Apkopots 2026. gada 14. oktobrī.

## Avoti

1. **SPKC, „Mutes veselības pētījums skolēniem Latvijā, 2015./2016. mācību gads”** (Rīga, 2016), https://www.spkc.gov.lv/lv/media/4336/download
   - Pētījumu veica SIA „RSU Stomatoloģijas institūts” (Senakola, Maldupa, Uribe, Ņizamovs).
   - Mērķa grupa: 12-gadīgie (6. klase). Izmeklēti 2138 bērni 92 skolās, atbildes rādītājs 74,5 %. Lauka darbs no 18.01. līdz 31.03.2016.
   - Lapu numuri CSV piezīmēs atbilst ziņojumā drukātajiem numuriem (drukātais numurs = PDF lapa − 3).
2. **SPKC, „Mutes veselības pētījums skolēniem Latvijā, 2022./2023. mācību gads”** (Rīga, 2023), https://www.spkc.gov.lv/lv/media/19467/download
   - Autori: Maldupa, Uribe, Rivare-Pālena, Stāmere, Brinkmane, Senakola.
   - Mērķa grupa: 12- un 15-gadīgie. Izmeklēti 1557 12-gadīgie un 1571 15-gadīgais. Atbildes rādītājs 65 % 6. klasēs un 56 % 9. klasēs. 23 % skolu atteica dalību.
   - Drukātais lapas numurs = PDF lapa − 1.
3. Abi ziņojumi ir publicēti SPKC lapā „Veselību ietekmējošo paradumu pētījumi” (https://www.spkc.gov.lv/lv/veselibu-ietekmejoso-paradumu-petijumi). Citu valsts mēroga SPKC mutes veselības pētījumu tur nav.
4. **Maldupa I. et al.**, *Int Dent J* 2021;71:214–223, https://doi.org/10.1111/idj.12627. Tie paši 2016. gada dati angliski un salīdzinājums ar Eiropas vidējo.
5. **Bjarnason S. et al.**, „Oral health in Latvian 15-year-olds”, *Eur J Oral Sci* 1995, https://doi.org/10.1111/j.1600-0722.1995.tb00026.x. Pētījums veikts 1993. gadā, n=506.
6. **Bjarnason S.**, *Acta Odontol Scand* 1998, https://doi.org/10.1080/000163598422947. Baltijas 12-gadīgo kariesa rādītāji, bet datu gads nav norādīts.
7. **Preprints** (nav recenzēts): Maldupa, Uribe et al., „High Burden of Dental Caries in First-Grade Children in Latvia”, Zenodo, 2026, https://doi.org/10.5281/zenodo.19441202. Aptver tikai Rīgu un Pierīgu (n=822, vidējais vecums 7,1 g.).

**Nav atrasts:**
- PVO „Oral health country profile” Latvijai ar konkrētiem skaitļiem.
- PVO CAPP datubāzes ieraksts. Lapu neizdevās atvērt.
- Vecāka valsts mēroga 6-gadīgo dmft vērtība. 2011. gada pētījums 6 un 12 gadus veciem bērniem nav reprezentatīvs.
- 2004. gada pētījuma (Bērziņa) skaitliskās vērtības. SPKC 2016 to min tikai kā „par 40% samazinājusies” kariesa intensitāti (6. lpp.).

## Oficiālie termini (SPKC ziņojumos)

**Svarīgi:** SPKC lieto **KPE** (nevis „KPS”). KPE ir angļu DMFT/DMFS ekvivalents.
- **„Kariozo, plombēto un ekstrahēto zobu (z) vai virsmu (v) summa”** (2016, saīsinājumi, 3. lpp.).
- Indeksi: **KPEz** (zobiem) un **KPEv** (virsmām).
- Komponentes: **Kz** (kariozie), **Pz** (plombētie), **Ez** (ekstrahētie, „izrautie”).

Līmeņi pēc ICDAS:
- **K1PEz** – „emaljas kariesa bez kavitātes līmenī”; 2023. gadā „emaljas bojājumu bez kavitātes līmenī”. Atbilst D1MFT.
- **K3PEz** – 2016. gadā „kariesa ar kavitāti līmenī”, 2023. gadā **„emaljas-dentīna robežas bojājuma līmenī”**. Atbilst D3MFT. Galvenais SPKC rādītājs.
- **K5PEz** – „kariesa ar skaidri redzamu dentīna kavitāti līmenī”; 2023. gadā „dentīna bojājuma līmenī”. Atbilst D5MFT, t. i., klasiskajam PVO DMFT.

Citi termini:
- **Kariesa izplatība** – % bērnu, kuriem KPE > 0.
- **Kariesa smaguma pakāpe / kariesa intensitāte** – vidējais KPEz.
- **„Kariesa brīvi”** – bērni bez kariesa.
- **SiC** – „Kariesa nozīmīguma indekss”: vidējais KPEz tai trešdaļai bērnu, kuriem kariesa ir visvairāk.
- **Silanti** (2016) / **sīlanti** (2023) – fisūru hermetizācija.
- **Periodonts**: 2016. gadā novērtēts ar CPI, 2023. gadā ar **BPE** indeksu.

## Definīcijas un nedrošības

- **Diagrammai izmantojiet K3PEz** (`ORAL_*_D3`). Ar Eiropas datiem salīdziniet K5PEz (`ORAL_*_D5`), jo vecākie pētījumi un PVO kariesu reģistrē dentīna kavitātes līmenī. Dažādie līmeņi ir saglabāti zem atšķirīgiem kodiem.
- **2016 → 2023 nav tieši salīdzināmi.** SPKC 2023 to norāda pats (60. un 66. lpp.):
  - atbildes rādītājs bija zemāks;
  - 23 % skolu atteica dalību;
  - lauka darbs ilga 7,5 mēnešus.
  Tāpēc, visticamāk, piedalījās „ieinteresētāku ģimeņu bērni”, un kritums var būt daļēji mākslīgs.
- **Iekšējas pretrunas 2023. gada ziņojumā:**
  - 29. lpp. teksts 12-gadīgajiem min K1 izplatību 78,1 %, bet 18. tabula un kopsavilkums – 86,1 %.
  - 19. un 20. tabulas 15-gadīgajiem dod 89,3/72,7/63,5 %, bet 18. tabula – 93,3/83,5/76,3 %.
  - CSV izmantota 18. tabula, jo tā sakrīt ar kopsavilkumu un rekomendācijām.
- **Neārstēts kariess:** % bērnu ar neārstētu kariesu nav publicēts nevienā SPKC ziņojumā.
  - CSV ir tikai vidējais neārstēto kariozo zobu skaits (`ORAL_DT_*`). Tas ir **APRĒĶINĀTS** kā komponenšu summa, un summas pareizība pārbaudīta pret KPE.
  - 1993. gadā D komponente veidoja 33 % no DMFS.
- **Zobu tīrīšana 2023:**
  - SPKC ziņojums 12-gadīgajiem dod 45,0 % (`ORAL_BRUSH2`).
  - RSU kongresa abstrakts dod 37,9 % (`ORAL_TOOTH2_RSU` failā `berni_pusaudzi_veseliba.csv`). Atšķirības iemesls nav zināms.
  - Šie rādītāji nav HBSC un nav salīdzināmi ar HBSC „>1 reizi dienā”.
- **Vizītes:**
  - 2016. gadā jautāja atsevišķi par zobārstu pēdējos 12 mēnešos un higiēnistu vismaz reizi gadā.
  - 2023. gadā jautāja par zobārstu **vai** higiēnistu vismaz reizi gadā.
  - Tie ir dažādi jautājumi, tāpēc kodi ir atšķirīgi.
- **Eiropas vidējais** (D5MFT>0 = 52 %, D5MFT = 1,1) ņemts no Maldupa 2021 abstrakta. Atsauces gads un valstu kopa tur nav norādīti.
- **Bjarnason 1998 Baltijas skaitļi** (LV 5,8; LT 4,9; EE 4,6) apzīmēti kā „mean caries prevalence”, un datu gads nav norādīts. CSV tiem ir atzīme NEDROŠS.
- **7-gadīgo dati** ir preprints, kas aptver tikai Rīgu un Pierīgu. Tie nav valsts mēroga.

## Galvenās atziņas

1. **Kariess skar lielāko daļu pusaudžu.** 2023. gadā kariesa pieredze (K3 līmenī) bija 66,3 % 12-gadīgo un 83,5 % 15-gadīgo. Pilnībā „kariesa brīvi” bija tikai 13,9 % un 6,9 %. SPKC secina:
   - 2023: „Kariesa izplatība Latvijā ir augsta un nenovēro būtisku situācijas uzlabošanos” (63. lpp.).
   - 2016: Latvijas līmenis ir „viens no augstākajiem Eiropā” (4. lpp.).
2. **Vidējais KPEz (K3) 12-gadīgajiem samazinājās no 3,35 (2016) līdz 2,3 (2023).** 15-gadīgajiem 2023. gadā tas bija 4,4.
   - Atšķirības dēļ zemākas atsaucības 2023. gadā šo kritumu jāinterpretē piesardzīgi.
   - Ilgākā laikā uzlabojums ir skaidrs: 1993. gadā 15-gadīgo DMFT bija 8,1.
   - Klasiskajā (K5) līmenī Latvijas 2,5 (2016) ir vairāk nekā divreiz augstāks par Eiropas vidējo 1,1.
3. **Kariess strauji progresē pusaudža gados.** No 12 līdz 15 gadu vecumam K3PEz gandrīz divkāršojas (2,3 → 4,4). SPKC norāda, ka neinvazīvā ārstēšana Latvijā „nav efektīva” (62. lpp.).
4. **Sīlantu ir maz: tikai 6–7 % bērnu (gan 2016, gan 2023).** Turpretī sīlanti būtu indicēti 64 % 12-gadīgo un 74 % 15-gadīgo. SPKC 2016 to nosauc par „neizprotami” zemu (52. lpp.), un sīlantus joprojām neapmaksā no valsts budžeta.
5. **Paradumi gandrīz nemainās:**
   - divas reizes dienā zobus tīra 45–51 %;
   - tikai 40–46 % zina, ka viņu zobu pastā ir ≥1000 ppm fluorīda;
   - 70–73 % ēd saldumus katru dienu, un 64 % katru dienu dzer saldinātus dzērienus.
   - SPKC ieteikumi: zobu pasta ar 1400–1500 ppm fluorīda, sīlanti 6–7 un 11–12 gadu vecumā, fluorīdu laka 2–4 reizes gadā, saldināto dzērienu izslēgšana no izglītības iestādēm un pievienotā cukura marķēšana (64.–65. lpp.).
