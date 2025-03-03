# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV 

**A mérést végző neve:** Erős Bence 
**A mérés tárgya:**  Műholdas vételi rendszer kiépítése     
**A mérés száma:** 01. mérés    
**A mérés dátuma:** 2025. 03. 03.    
**A mérést vezette:** Sándor Péter    

**Évfolyam:** 13. E  
**Csoport:** GYAK 1   
**Helyszín:** V3 Labor  

---

## Feladat célja 

Egy szabadon fogható (FTA) csatorna véletének beállítása, műholdas vételi rendszer kiépítése és vizsgálata, majd optimális vételi jel csatlakoztatása egy set op boxba, amin keresztül képet jelenítünk meg.  

## Felhasznált eszközök   

| Eszköz típusa         | Megnevezés                                      |
|-----------------------|------------------------------------------------|
| **Parabolaantenna**   | D80 Mesh hálós acél parabola antenna (tripodra szerelve) |
| **Műholdvevő fej (LNB)** | Ekselans SATCR LNB                           |
| **Set-top box**       | Amiko HD 8265+                                 |
| **Jelmérő eszköz**    | METEK HDD jelmérő                              |
| **Kábelek és csatlakozók** | Koaxiális kábelek és csatlakozók           |
| **Jelosztó**         | 2-es műholdas jelosztó                         |
| **Szerelési eszközök** | Csavarhúzó, villáskulcs, iránytű, dőlésszögmérő |


---

## Mérés célja

- Először összeszereltem az antennát, majd rögzítettem rá az általam választott **Ekselans SATCR LNB** fejegységet.  
Az internetről, a lyngsat.com műholdvevő adatbázis segítségével kikerestem az elérhető **FTA csatornákat**, és kiválasztottam egyet, amelyet az **Eutelsat 9B** műhold sugároz.  
Az antenna dőlésszögét, polarizációját és elforgatását egy iránytű segítségével állítottam be, majd a METEK HDD-t használva igyekeztem a lehető legjobb jelet megtalálni. A végső beállítások szerint az azimut (iránytartás) szöge 198°, az eleváció (emelkedési szög) 36°, az LNB elforgatási szöge pedig 10° lett.  
Ezután összekötöttem az LNB fejegységet a set-top boxszal, majd a boxot egy monitorhoz csatlakoztattam.  
Végül beállítottam a megfelelő régiót és országot, majd elindítottam az automatikus csatornakeresést.

---

## METEK HDD kép és jelszintmérés 

### Az alábbi kép a spektrumanalizátoron lévő műholdas jelszint kijelzőjét mutatja. 

<img src="https://github.com/user-attachments/assets/35f823b8-6930-40b0-b3a9-0e259ef5a671" width="600px">

  - A vizsgált frekvencia 1358.0 MHz.
  - A műhold: Eutelsat 9A (9B-vel megegyező csatornakiosztásai vannak).
  - MER (Modulation Error Ratio) érték : 11.9 dB 
  - Jelszint: 83.2 dBuV 

### Csatornainformációk.

<img src="https://github.com/user-attachments/assets/f09b20e9-6991-4a65-89e1-371d06a6181d" width="300px">

<img src="https://github.com/user-attachments/assets/c9866975-e921-4f90-85b2-ee9293c21204" width="300px">

| Csatorna adatai         | Részletek                                   |
|------------------------|--------------------------------------------|
| **Csatorna neve**      | M1 HD                                     |
| **Szolgáltatás azonosító (Service ID)** | 101                        |
| **Hálózat azonosító (Network ID)**     | 158                        |
| **Eredeti hálózat azonosító (ONID)**   | 106                        |
| **Képfelbontás**       | 1920 × 1080 (Full HD)                     |
| **Videó PID és bitráta** | 1101 / 3.989220 Mb/s (H.264 tömörítés) |
| **Hang PID és bitráta**  | 1201 / 0.415802 Mb/s (AC3 hangformátum) |


---

## Set-Top box

### Tv csatornák keresése

<img src="https://github.com/user-attachments/assets/7dff4e4b-3a8b-46d3-992a-facbcc0215e6" width="300px">


<img src="https://github.com/user-attachments/assets/031b5371-bec4-4781-b633-25378858c61c" width="300px">

**Quality:87** 

---

**Aláírás:** Erős Bence 

**Dátum:** 2025. 03. 03.

