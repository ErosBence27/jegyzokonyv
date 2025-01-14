# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** T-Mérés <br>
**A mérés száma:** 1. mérés  
**A mérés dátuma:** 2024. 12. 18  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

## 1. Mérés célja

A T-típusú ellenállás-hálózat működési jellemzőinek meghatározása 6 dB-es csillapítási értéknél.

---

## 2. Felhasznált eszközök

- **NI myDAQ**
- **Ellenállások:**

| **Ellenállás** | **Számolás alapján** | **Méréskor használt**                  |
|----------------|-----------------------|----------------------------------------|
| Rg            | 1100 Ω               | 2,2 kΩ + 2,2 kΩ                        |
| R1            | 367 Ω                | 220 Ω + 120 Ω                          |
| R2            | 1.473 kΩ             | 1.5 kΩ                                 |


---

## 3. Elméleti háttér

A T-típusú csillapítókör ("T pad") egy speciális csillapító áramkör, amelyet az elektronikában a jel szintjének csökkentésére használnak. Az elrendezés a "T" betű formáját utánozza.

A csillapítók működési elve, hogy lapos frekvenciamenettel bírnak, azaz a csillapítás mértéke az összes frekvencián azonos az adott tartományon belül. Feladatuk az erősítőkével ellentétes, hiszen nem erősítik, hanem csillapítják a jelet.

A csillapítók kialakítása egyszerű, a szűrőkörökéhez hasonló, de a frekvenciaválasz együttese miatt nincs szükség komplex áramköri elemekre.

### Az ellenállások értékeinek kiszámítása:

- Generátor impedancia: 1100 Ω
- Csillapítá mértéke: 6 dB

### Ellenállások számítási képletei:

![Képletek](https://github.com/user-attachments/assets/6f1eb4c4-6b68-451b-8bc6-b52f0b87d846)

### Helyettesítés után:

![Képletek](https://github.com/user-attachments/assets/08469239-b31b-4f84-a100-24f94ad70c49)

---

## 4. Szimuláció

A T-típusú csillapítókör szimulációja Falstadban megépitve.

![flastad](https://github.com/user-attachments/assets/6e2a14cf-838b-4980-a3c4-6109fa8dd237)


---

## 5. Mérési eredmények

 **Rögzített adatok:**

| Paraméter           | Érték |
|---------------------|-------|
| Generátor jel       | 2.002 Vp2p |
| Kimeneti Jel        | 1.062 Vp2p |
| Generátor Frekvencia| 1000 Hz |
| Csillapítás         | -5.507 dB |
| Átviteli Arány      | 5.507 dB |
| Bemeneti impedancia | 2.17 kΩ |
| Kimeneti impedancia | 687 Ω |   


![scope](https://github.com/user-attachments/assets/7a7e01e3-dead-48c8-988d-87fd22a07c80)

![generator](https://github.com/user-attachments/assets/a774508a-608e-477c-afa3-0c0390111e16)

---

- **Megjegyzés:**
  A csillapító áramkört breadboardon építettük össze. A jelgenerátor 1000Hz-s 2Vp2p váltakozó feszültséget állított elő. A CH0 a bemeneti, míg a CH1 a kimeneti feszültséget mutatta. A mérés megerősítette, hogy a kimeneti jel amplitúdója nagyjából a fele a bemenetének.

---

[Szimulációs eredmény](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWcMBMcUHYMGZIA4UA2ATmIxAUgoqoQFMBaMMAKADcRsEUQAWbHlx4oEhKOGRwQPKrOgIWAJ07dpovnioixVZnCUat6wvjU7OhDAZN4zIHGO3jsl66ac2+A8WF44DDnaB-DLgYPoA7vYuXjyeIVAsUYFOeN5OkEnRYglpPAmZAA6GdryasZx84plRQhVlVAVZDRXx3kUgeXZdCdhVsiwA5iBtcaa8hLzVLEA)



---
**Aláírás:** Erős Bence

**Dátum:** 2024. 12. 18.
