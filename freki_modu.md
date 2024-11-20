# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** Frekvencia vs. moduláció mérés


**A mérés száma:** 4. mérés  
**A mérés dátuma:** 2024. 11. 20  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

# Mérési Jegyzőkönyv

## 1. Mérés Célja
A mérés célja a **Johansson 8202 DVB-T modulátor** működésének megismerése, konfigurációjának tesztelése, valamint a METEK HD spektrum- és jelszintanalizátor használatával a modulátor által generált jel paramétereinek mérése. A mért paraméterek: **jelszint**, **bitsebesség**, **MER (Modulation Error Rate)**.

---

## 2. Használt Eszközök

| Eszköz                     | Típus                       | Funkció                                           |
|----------------------------|-----------------------------|---------------------------------------------------|
| Johansson 8202             | DVB-T modulátor            | Bitsebesség és jelminőség vizsgálata              |
| RF kábel                   | Koaxiális kábel            | Modulátorok és spektrumanalizátor összekötése     |
| Metek HDD                  | Spektrum/jelszint analizátor| Frekvencia, moduláció, sávszélesség, jelszint, MER és bitsebesség mérése |

---

## 3. Beállítások
- **Frekvencia**: 490 MHz  
- **Sávszélesség**: 8 MHz  
- **Modulációs típusok tesztelése**:  
  - QPSK  
  - 16QAM  
  - 64QAM  

---

## 4. Mérési Eredmények
Az alábbi táblázatban összefoglaljuk a mérések eredményeit különböző modulációs beállítások mellett.

| **Moduláció** | **Jelszint [dBm]** | **Bitsebesség [Mbps]** | **MER [dB]** |
|---------------|---------------------|------------------------|--------------|
| QPSK          | -30.3 dBm          | 3.5 - 4.2 Mbps        | 39.9 dB      |
| 16QAM         | -30.1 dBm          | 8.0 - 10.2 Mbps       | 35.8 dB      |
| 64QAM         | -30.5 dBm          | 13.0 - 15.8 Mbps      | 40.0 dB      |

---

## 5. Lépések
1. **Modulátor konfigurációja**:
   - A Johansson 8202 DVB-T modulátoron beállítottuk a kívánt frekvenciát (490 MHz) és a sávszélességet (8 MHz).  
   - A modulációs típusokat egyesével módosítottuk: QPSK, 16QAM, 64QAM.

2. **Jel vizsgálata METEK HD analizátorral**:
   - Az RF kábellel csatlakoztattuk a METEK HD spektrum/jelszint analizátort a modulátor kimenetéhez.  
   - Minden egyes modulációs típus esetén elvégeztük a jelszint, bitsebesség és MER mérést.  

---

## 6. Következtetések
- A mérés során megfigyelhető volt, hogy a moduláció típusának növelésével (QPSK → 64QAM) a bitsebesség jelentősen nőtt, miközben a **MER érték** változásai nem mutattak egyértelmű tendenciát.  
- A mérések a DVB-T elméleti követelményeinek megfelelő eredményeket adtak.

---

## 7. Megjegyzések
- A méréseket stabil környezeti feltételek mellett végeztük, zavarforrásoktól mentes helyiségben.  
- Az adatok alapján a különböző modulációs technikák közötti különbségek jól megfigyelhetőek voltak.

---

## 8. További Mérési Javaslatok

<details>   

<summary>Kattins a részletekért</summary>   

1. Szélsőséges Jelszint Tesztelése   

- **Cél**: Vizsgálni, hogyan viselkedik a rendszer különböző jelszint értékek mellett.   

- **Lépések**:  

  1. Állítsuk be a jelszintet az RF kimeneten szélsőségesen alacsony és magas értékekre (pl. -60 dBm, -20 dBm).  

  2. Mérjük meg a bitsebességet és a MER-t a kiválasztott modulációs típusok mellett.  

- **Elvárt eredmények**: Magasabb jelszintnél stabilabb adatátvitel, alacsonyabb jelszintnél romló MER és csökkenő bitsebesség.   

---  

2. Szűkebb és Szélesebb Sávszélesség Hatásai

- **Cél**: Megvizsgálni a sávszélesség változtatásának hatását a jel minőségére és teljesítményére.

- **Lépések**:

  1. Állítsuk be a sávszélességet különböző értékekre (pl. 6 MHz, 7 MHz, 8 MHz).

  2. Rögzítsük a jelszintet, MER-t és a bitsebességet.

- **Elvárt eredmények**: Szélesebb sávszélességnél nagyobb bitsebesség, de csökkenhet a MER.

---

3. Zavarforrások Hatása

- **Cél**: Meghatározni, hogy a közeli rádiófrekvenciás zavarok hogyan befolyásolják a jelek minőségét.

- **Lépések**:

  1. Helyezzünk egy zavarforrást (pl. másik RF jeladó) a vizsgált frekvencia közelébe.

  2. Mérjük meg a jelszintet, MER-t és a bitsebességet különböző távolságokból.

- **Elvárt eredmények**: Zavarforrás jelenléte csökkentheti a MER-t és növelheti a hibaarányt.

---

4. Moduláció Stabilitásának Vizsgálata Időfüggvényében

- **Cél**: Tesztelni, hogy hosszabb időtartam alatt mennyire stabil a jel különböző modulációs típusok esetén.

- **Lépések**:

  1. Állítsuk be az eszközt egy modulációs típusra (pl. 64QAM).

  2. Mérjünk jelszintet, MER-t és bitsebességet óránként legalább 12 órán keresztül.

- **Elvárt eredmények**: Stabil rendszer esetén a paramétereknek változatlannak kell maradniuk.

---

5. Szomszédos Csatornák Vizsgálata

- **Cél**: Megérteni, hogyan befolyásolja a szomszédos csatornák jelenléte a méréseket.

- **Lépések**:

  1. Aktiváljunk egy szomszédos csatornán (pl. 482 MHz vagy 498 MHz) másik DVB-T jelet.

  2. Mérjük meg a főcsatorna (490 MHz) paramétereit.

- **Elvárt eredmények**: Növekvő interferencia esetén csökkenhet a MER és romolhat a jel minősége.

---

6. Jelkésleltetés Vizsgálata

- **Cél**: Ellenőrizni a rendszer válaszidejét különböző beállítások mellett.

- **Lépések**:

  1. Állítsunk be eltérő modulációkat és sávszélességeket.

  2. Mérjük meg a jelkésleltetést (pl. speciális analizátorral vagy műszerekkel).

- **Elvárt eredmények**: A sávszélesség és moduláció változtatása hatással lehet a késleltetésre.

---

7. Hőmérséklet Hatásának Vizsgálata

- **Cél**: Megérteni, hogyan befolyásolja a környezeti hőmérséklet a rendszer teljesítményét.

- **Lépések**:

  1. Végezze el a méréseket különböző hőmérsékleteken (pl. 0°C, 25°C, 30°C).

  2. Rögzítse a jelszint, MER és bitsebesség értékeket.

- **Elvárt eredmények**: Szélsőséges hőmérsékleteken csökkenhet a rendszer stabilitása.   

</details>

<br>

---

## 9. Diagramm
- Mérési jegyzőkönyv grafikon: *[Melléklet nem elérhető]*  

---

## 10. Záró Összegzés


---

## 11. Mért Képek

<details>
<summary>Kattins a részletekért</summary>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/munkakep1.jpg"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/frekik.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/qpsk_meter.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/qpsk_bit.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/16qam_meter.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/16qam_meter.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/64qam_meter.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/64qam_bit.bmp"/>

<br>

</details>

**Aláírás:** Erős Bence

**Dátum:** 2024. 11. 20.