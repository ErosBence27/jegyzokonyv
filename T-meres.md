# MÉRÉSI JEGYZŐKÖNYV

**Mérést végző neve:** Erős Bence

**Mérés tárgya:** T-típusú ellenállás-hálózat

**Mérés száma:** 01

**Mérés időpontja:** 2024.12.18

**Mérést vezette:** Sándor Péter

**Évfolyam:** 13. E
**Csoport:** GYAK 2
**Helyszín:** V3 labor

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

- **Megjegyzés:**
  A csillapító áramkört breadboardon építettük össze. A jelgenerátor 1000 Hz-es, $2 \ \text{Vp2p}$ váltakozó feszültséget állított elő. A CH0 a bemeneti, míg a CH1 a kimeneti feszültséget mutatta. A mérés megerősítette, hogy a kimeneti jel amplitúdója nagyjából a fele a bemenetének.

[Szimulációs eredmények]()