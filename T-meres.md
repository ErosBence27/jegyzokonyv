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

| Típus                | Értékek                            |
|----------------------|------------------------------------|
| **Számított értékek**|                                    |
| $R_g$               | $1100 \\ \Omega$                 |
| $R_1$               | $367 \\ \Omega$                  |
| $R_2$               | $1.473 \\ \text{k}\\Omega$      |
| **Mérés során alkalmazott értékek** |                     |
| $R_g$               | $2.2 \\ \text{k}\\Omega + 2.2 \\ \text{k}\\Omega$ |
| $R_1$               | $220 \\ \Omega + 120 \\ \Omega$ |
| $R_2$               | $1.5 \\ \text{k}\\Omega$         |
---

## 3. Elméleti háttér

A T-típusú csillapítókör ("T pad") egy speciális csillapító áramkör, amelyet az elektronikában a jel szintjének csökkentésére használnak. Az elrendezés a "T" betű formáját utánozza.

A csillapítók működési elve, hogy lapos frekvenciamenettel bírnak, azaz a csillapítás mértéke az összes frekvencián azonos az adott tartományon belül. Feladatuk az erősítőkével ellentétes, hiszen nem erősítik, hanem csillapítják a jelet.

A csillapítók kialakítása egyszerű, a szűrőkörökéhez hasonló, de a frekvenciaválasz együttese miatt nincs szükség komplex áramköri elemekre.

### Az ellenállások értékeinek kiszámítása:

- Generátor impedancia: $R_g = 1100 \ \Omega$
- Csillapítási mérték: $6 \ \text{dB}$

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

### Rögzített adatok:

| Paraméter             | Érték       |
|-----------------------|-------------|
| Generátor feszültség  | $2.002 \ \text{Vp2p}$ |
| Kimeneti feszültség   | $1.062 \ \text{Vp2p}$ |
| Generátor frekvencia  | $1000 \ \text{Hz}$    |
| Csillapítás           | $-5.507 \ \text{dB}$ |
| Átviteli arány       | $5.507 \ \text{dB}$  |
| Bemeneti impedancia   | $2.17 \ \text{k}\Omega$ |
| Kimeneti impedancia   | $687 \ \Omega$       |

![scope](https://github.com/user-attachments/assets/7a7e01e3-dead-48c8-988d-87fd22a07c80)

![generator](https://github.com/user-attachments/assets/a774508a-608e-477c-afa3-0c0390111e16)

---

- **Megjegyzés:**
  A csillapító áramkört breadboardon építettük össze. A jelgenerátor 1000 Hz-es, $2 \ \text{Vp2p}$ váltakozó feszültséget állított elő. A CH0 a bemeneti, míg a CH1 a kimeneti feszültséget mutatta. A mérés megerősítette, hogy a kimeneti jel amplitúdója nagyjából a fele a bemenetének.

---

[Szimulációs eredmény](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWcMBMcUHYMGZIA4UA2ATmIxAUgoqoQFMBaMMAKADcRsEUQAWbHlx4oEhKOGRwQPKrOgIWAJ07dpovnioixVZnCUat6wvjU7OhDAZN4zIHGO3jsl66ac2+A8WF44DDnaB-DLgYPoA7vYuXjyeIVAsUYFOeN5OkEnRYglpPAmZAA6GdryasZx84plRQhVlVAVZDRXx3kUgeXZdCdhVsiwA5iBtcaa8hLzVLEA)



---
**Aláírás:** Erős Bence

**Dátum:** 2024. 12. 18.
