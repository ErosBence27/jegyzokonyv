# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** Tranzisztor működésének vizsgálata
**A mérés száma:** 8. mérés  
**A mérés dátuma:** 2025. 01. 08  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

## 1. Mérés Célja 
Tanzisztor működésének vizasgálata.

---

## 2. Alkalmazott Mérőeszközök és Készülékek és Alkatrészek

| Műszer neve                         | Gyártási szám         |
| ----------------------------------- | -------------------   |
|  NImyDAQ                            | 3045906               |
| Metex                               | 736015                |

---

|Alkatrészek|Értékek|
|-----------|-------|
|Rbe        |1.47k $\Omega$  |
|Rc         |220 $\Omega$    |
|$\beta$    |89     |

---

## 3. Mérés folyamata 

- Az NI myDAQ műszerrel tanulmányoztam a tranzisztor működését. A mérési áramkörben a tranzisztor bázisára vezérlőjelet adtam egy sorosan kapcsolt ellenálláson keresztül. A vizsgálat során megmértem az emitter- és kollektoráramokat, valamint a kollektor-ellenálláson eső feszültségből következtettem a tranzisztor állapotára és a vezérlőáram hatására.

---

## 4. Kapcsolasi rajz

![kapcsolasrajz](https://github.com/user-attachments/assets/00b86d92-13a3-4277-b019-df7a2c8ef0b5)

---

## 5. Mért adatok vs. Szimuláció

| **Mért adatok** |         |         | **Szimuláció** |         |         |
|------------------|---------|---------|----------------|---------|---------|
| Vbe [V]         | Urc [V] | Ic [mA] | Vbe [V]        | Urc [V] | Ic [mA] |
| 0,4             | 0,00    | 0,00    | 0,4            | 0,00    | 0,52    |
| 0,5             | 0,00    | 0,02    | 0,5            | 0,01    | 0,02    |
| 0,6             | 0,13    | 0,57    | 0,6            | 0,16    | 0,74    |
| 0,7             | 0,96    | 4,37    | 0,7            | 0,89    | 4,05    |
| 0,8             | 2,30    | 10,45   | 0,8            | 1,94    | 8,80    |
| 0,9             | 2,63    | 11,95   | 0,9            | 2,98    | 13,56   |
| 1               | 2,66    | 12,09   | 1              | 3,05    | 13,85   |
| 1,5             | 2,71    | 12,32   | 1,5            | 3,09    | 14,04   |
| 2               | 2,72    | 12,36   | 2              | 3,10    | 14,10   |

---

## 6. Diagrammok

![mértadatok diagramm](https://github.com/user-attachments/assets/ef901e09-2eb6-4ae4-8ccb-e58e06724324)


![szimulácios diagramm](https://github.com/user-attachments/assets/57cc4008-8504-4f00-9c31-95d7451f9419)


---

## 7. Tapasztalat

- A mérés során észrevettem, hogy 1 V felett az értékek gyakorlatilag állandósulnak, és nem mutatnak jelentős változást.

---

## 8. Összeépített

<img src="https://erosbence27.github.io/jegyzokonyv/image/20250108_130253.jpg"/>

---

## 9.Falstad Link

[Link](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWcMBMcUHYMGZIA4UA2ATmIxAUgoqoQFMBaMMAKABcQUUAWEXXlHjx9IvKhBgI8haRkLZShBAkIoo0QpsrF8JQhm4YEvPMRAATOgDMAhgFcANmxZhVnIeEJVBwn5wvW9k4MDnTm4FCRMJCsAO7uwthoCXwyUCwA5inYaX7crlEsAE6cPCK8rlT8kWCUkCzxfjnClanC9QBunlVprdVUVNzeUeoILABKKdy+HgUDIEPU85INUzPCeAPFKZsprd5oq3mJadPpjbNebd3pAA7XZ8032CNg8O8sQA)

---

**Aláírás:** Erős Bence

**Dátum:** 2025. 01. 08.

