# Bērnu un pusaudžu veselība un veselības izglītība Latvijā

Šī interaktīvā vizualizācija rāda Latvijas bērnu un pusaudžu veselības rādītājus (psihiskā veselība, ņirgāšanās, uzturs, miegs, fiziskā aktivitāte, liekais svars, atkarības, reproduktīvā veselība), veselības izglītībai skolā atvēlēto laiku un veselības izglītības politikas posmus.

**Skatīt:** atveriet `index.html` pārlūkā vai GitHub Pages adresē.

## Saturs

- `index.html` – vizualizācija. Tā ir viens fails, un vienīgā ārējā atkarība ir Chart.js no cdnjs.
- `dati/pusauzu_reproduktiva_veseliba.csv` – laika rindas (gads, dzimums, vecums, vērtība, mērvienība un avota URL katrai rindai).
- `dati/pusauzu_reproduktiva_veseliba.md` – datu definīcijas, avoti un iztrūkumi.
- `dati/veselibas_izglitibas_hronologija.csv` – 52 veselības izglītības politikas notikumi (1992–2026) ar avotiem un ticamības novērtējumu.
- `dati/veselibas_izglitibas_hronologija.md` – piezīmes par hronoloģiju.
- `dati/berni_pusaudzi_veseliba.csv` – bērnu un pusaudžu veselības rādītāji (HBSC, COSI, ESPAD, GYTS, PISA, Eurostat), tajā pašā formātā.
- `dati/berni_pusaudzi_veseliba.md` – definīcijas, avoti, iztrūkumi.
- `dati/mutes_veseliba.csv`, `dati/mutes_veseliba.md` – skolēnu mutes veselība (SPKC, 2016 un 2023).
- `dati/terminu_saskanosana.md` – lapā lietoto terminu atbilstība SPKC un CSP oficiālajiem terminiem.
- `dati/stundu_skaits_veseliba.md` – veselības tēmām skolā atvēlētais laiks (MK noteikumi Nr. 747, VISC programmas paraugi).

## Rādītāji

| Rādītājs | Avots | Periods |
|---|---|---|
| Dzimumattiecības, agrīns sākums, prezervatīvu un tablešu lietošana (15 g. pusaudži) | SPKC / WHO HBSC | 2002–2022 (ik 4 gadus) |
| Pusaudžu dzemdības (15–19 g.) | Eurostat | 2000–2024 |
| Aborti (15–19 g.) | Eurostat, CSP, SPKC | 2000–2025 |
| Sifiliss, gonoreja, hlamīdijas (15–24 g.) | ECDC, SPKC | 2000–2024 |
| HIV jaunie gadījumi (15–24 g.) | SPKC | 2014–2024 |
| CPV vakcinācija | WHO, SPKC | 2010–2025 |
| Ņirgāšanās, veselības sūdzības, nervozitāte, pašvērtētā veselība, vientulība | HBSC | 2002–2022 |
| Brokastis, augļi, fiziskā aktivitāte, miegs, zobu tīrīšana | HBSC | 2002–2022 |
| Kariess, KPE indekss, sīlanti (12 un 15 g.) | SPKC mutes veselības pētījums | 2016, 2023 |
| Lieka ķermeņa masa un aptaukošanās | HBSC; PVO COSI (mērīts) | 2002–2024 |
| E-cigaretes, smēķēšana, alkohols, azartspēles, sociālie tīkli | HBSC, ESPAD, GYTS | 1995–2024 |

## Ierobežojumi

- Grafiks rāda **sakritības laikā, nevis cēloņsakarību**.
- Abortu koeficients ir aprēķināts, tas nav oficiāls rādītājs.
- Hlamīdiju datos ap 2009. gadu ir ziņošanas pārrāvums.
- HBSC 2025./26. gada dati vēl nav publicēti.
- Laikposms 1995–2005 politikas hronoloģijā balstās uz vienu avotu.

Sagatavots 2026. gada oktobrī.
