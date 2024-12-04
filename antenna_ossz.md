# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** Antenna összehasonlítás mérés  
**A mérés száma:** 5. mérés  
**A mérés dátuma:** 2024. 12. 04  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor  

---

## 1. Mérési Feladat
A mérési feladat célja három különböző vételi ponton az antennák nyereségének összehasonlítása. A méréseket **634 MHz** frekvencián végeztük.

---

## 2. Alkalmazott Mérőeszközök és Készülékek

- **Frekvencia:** 634 MHz

| Eszköz/Műszer neve                  | Típus                | Leírás/Link                                    |
|-------------------------------------|----------------------|------------------------------------------------|
| Programozható antennaerősítő-szűrő  | Johansson 6700       |                                                |
| Spektrum Analizátor                 | Metek HDD            |                                                |
| Antenna                             | Iskra P20 LOGPER     | [Leírás](https://bolt.sat.hu/iskra-p-20f-passziv-uhf-logper-antenna-75-dbi-2940?srsltid=AfmBOooxPj6D1HDPUjw5xcao_Izt7di15AA-8xsBtznfbAX431Rg7y63) |
|                                     | SMART HD 550         | [Leírás](https://bolt.sat.hu/opticum-smart-hd-550-szobaantenna-3135?srsltid=AfmBOopzsStuWMBIGKVNKGFObYG5-NeQaW_3Z0zCVwr0YBzbp-i0dHRI)    |
|                                     | IKUSI FLASHD C48     | [Leírás](https://bolt.sat.hu/ikusi-flashd-c48-digitalis-foldfelszini-tv-antenna-3173?srsltid=AfmBOoqicoM5aMRo9iAcvIR_4QmPxyr4AOYSCxklJKDQJqXJ67bfkvK-)  |


---

## 3. Vételi Pontok és Eredmények

| Vételi Pont | Antenna Típus    | Mért Jelszint (dBm)  |
|-------------|------------------|----------------------|
| V3 Labor    | Smart HD 550     | -62.1 dBm            |
|             | Iskra P20     	 | -56.6 dBm            |
|             | Ikusi FlasHD C48 | -53.3 dBm            |
|-------------|------------------|----------------------|
| 3. Emelet   | Smart HD 550     | -34.2 dBm            |
|             | Iskra P20        | -28.6 dBm            |
|             | Ikusi FlasHD C48 | -25.8 dBm            |
|-------------|------------------|----------------------|
| Udvar       | Smart HD 550     | -53.5 dBm            |
|             | Iskra P20        | -48.3 dBm            |
|             | Ikusi FlasHD C48 | -46.8 dBm            |

---

## 4. Mérési Helyszínek Leírása
- **V3 Labor:** V3 Labor beltér,  [Antenna távolsága ](https://raw.githubusercontent.com/ErosBence27/jegyzokonyv/refs/heads/main/image/v3lab.PNG)
- **3. Emelet:** [3. emelet beltér](https://raw.githubusercontent.com/ErosBence27/jegyzokonyv/refs/heads/main/image/3_emelet.PNG),  [Antenna Távolsága ](https://raw.githubusercontent.com/ErosBence27/jegyzokonyv/refs/heads/main/image/3.emelet.PNG) 
- **Udvar:** [Udvar kültér](https://raw.githubusercontent.com/ErosBence27/jegyzokonyv/refs/heads/main/image/udvar_kint.PNG),  [Antenna Távolsága](https://raw.githubusercontent.com/ErosBence27/jegyzokonyv/refs/heads/main/image/udvar.PNG)  

---

## 5. Következtetések
1. **Ikusi FlasHD C48** antenna minden mérési ponton a legjobb jelszintet biztosította.  
   - **V3 Labor**: -53.3 dBm  
   - **3. Emelet**: -25.8 dBm  
   - **Udvar**: -46.8 dBm  
   Ez azt jelzi, hogy ez az antenna a legnagyobb nyereséggel rendelkezik az adott frekvencián és körülmények között.

2. **Iskra P20** antenna szintén jó teljesítményt nyújtott, de minden ponton alulmaradt az Ikusi FlasHD C48-hoz képest. Az eredmények azt mutatják, hogy:
   - A **V3 Laborban** -56.6 dBm,  
   - A **3. Emeleten** -28.6 dBm,  
   - Az **Udvaron** -48.3 dBm-es jelszintet mértünk.

3. **Smart HD 550** antenna a leggyengébb teljesítményt mutatta minden mérési ponton:
   - **V3 Labor**: -62.1 dBm,  
   - **3. Emelet**: -34.2 dBm,  
   - **Udvar**: -53.5 dBm.  
   Ez arra utal, hogy ez az antenna kisebb nyereséggel vagy kevésbé hatékony vétellel rendelkezik az adott környezetben.

## Általános Megjegyzések
- A mérési eredmények alapján az **Ikusi FlasHD C48** antenna ajánlható olyan helyszínekre, ahol kiemelkedően fontos a jó jelszint.  
- Az **Iskra P20** megfelelő alternatíva lehet, ha kisebb mértékű nyereség is elegendő.  
- A **Smart HD 550** beltéri használatra, közelebbi vételi pontokra lehet alkalmasabb.

---

## 6. További Mérési Javaslatok

A pontosabb és átfogóbb eredmények érdekében a következő mérési javaslatokat ajánljuk:

1. **Szélesebb Frekvenciasáv Vizsgálata**  
   Vizsgáljuk meg az antennák teljesítményét több frekvencián, például 470 MHz és 790 MHz között, hogy lássuk, hogyan változik a nyereség az UHF sáv teljes tartományában.

2. **Időjárási Hatások Elemzése**  
   Hasonló mérések elvégzése különböző időjárási körülmények között (esőben, szélben, ködben), hogy értékelhessük, milyen hatással vannak ezek a vételi jelszintre.

3. **Interferencia Hatásának Mérése**  
   Mérés különböző interferenciával terhelt környezetekben (például városi területeken), hogy kiderüljön, mennyire képesek az antennák szűrni a zavaró jeleket.

4. **Erősítő Hatásának Vizsgálata**  
   Hasonlítsuk össze az antennák teljesítményét különböző jelerősítők használatával, hogy kiderüljön, melyik kombináció adja a legjobb eredményt.

5. **Kültéri és Beltéri Teljesítmény Összehasonlítása**  
   Végezzünk további méréseket kifejezetten beltéri és kültéri környezetben, hogy részletesebb képet kapjunk az antennák helyspecifikus teljesítményéről.

Ezek a további mérések segíthetnek a különböző környezeti és technikai tényezők pontosabb megértésében, valamint az antennák optimális alkalmazási feltételeinek meghatározásában.

---

## 7. Záró Összegzés

A mérések alapján egyértelműen megállapítható, hogy az **Ikusi FlasHD C48** antenna nyújtotta a legjobb teljesítményt mindhárom mérési helyszínen. Ez az antenna a legmagasabb nyereséget biztosította, különösen a kültéri és távoli vételi pontokon, így kimondottan ajánlott nagy távolságú vétel esetén.

Az **Iskra P20** antenna szintén stabil és megfelelő jelszinteket eredményezett, azonban teljesítménye minden helyszínen elmaradt az Ikusi FlasHD C48-hoz képest. Ez az antenna jó alternatíva lehet azokban az esetekben, ahol közepes teljesítmény is elegendő.

A **Smart HD 550** antenna a legalacsonyabb jelszinteket biztosította, így elsősorban beltéri, rövid távolságú alkalmazásokra javasolt, ahol a kisebb nyereség nem okoz problémát.

Összességében az antennák közül az Ikusi FlasHD C48 bizonyult a legjobbnak, és javasolt elsődleges választásként alkalmazni a hasonló körülmények között végzett telepítéseknél.

---

**Aláírás:** Erős Bence

**Dátum:** 2024. 12. 04.
