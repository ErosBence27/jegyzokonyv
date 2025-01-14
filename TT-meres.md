# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** Π Csillapító Áramkör Mérés <br>
**A mérés száma:** 2. mérés  
**A mérés dátuma:** 2024. 12. 18  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

### 1. **Bevezetés**

A jelen jegyzőkönyv tárgyát egy π csillapító áramkör megvalósítása és a csillapítási paraméterek vizsgálata képezi. Az áramkört breadboardon építettük fel, ami gyors és rugalmas megoldást biztosít a mérésekhez.

---

### 2. **Elméleti Háttér**

A π csillapító áramkör az ellenállások elrendezéséről kapta nevét, amelyek a görög π betű formáját utánozzák. Az áramkör tervezéséhez a következő képleteket használtuk az ellenállások értékeinek kiszámításához:


## R1 képlete

![svgviewer-output](https://github.com/user-attachments/assets/69e1d223-8301-47d5-991e-cf5a02ca3129)



## R2 képlete

![svgviewer-output(1)](https://github.com/user-attachments/assets/066c4496-6457-491b-8b07-8cb2e8a842ca)


6 dB-es csillapítás esetén az ellenállások értékei az alábbi ábrán láthatók:

![ql_41d4e91c270a0827beb0bb25f1c6a62a_l3](https://github.com/user-attachments/assets/885313a7-7437-4c7a-ae67-1187bd0af9c2)


Az alábbi kapcsolási rajz bemutatja a jelgenerátor belső ellenállását, valamint a π csillapító áramkört a megfelelő ellenállásértékekkel:

![falstad](https://github.com/user-attachments/assets/6a13f673-6dae-4699-b7e5-f4dd4bd87ebf)



---

### 3. **Mérési Paraméterek**

- **NI myDAQ**
- **Ellenállások:**

| Paraméter           | Érték |
|---------------------|-------|
| Generátor feszültsége | 2.00 Vp2p|
| Kimeneti jel        | 0,494 Vp2p |
| Generátor frekvencia| 1000 Hz |
| Csillapítás         | -6,35 dB |
| Átviteli arány      | 2,076 dB |
| Bemeneti impedancia | 450 Ω |
| Kimeneti impedancia | 450 Ω |   

Az oszcilloszkópos méréseken a zöld 1-es csatornán a csillapított kimeneti jel, a kék 2-es csatornán pedig a generátor jele látható.

![scope](https://github.com/user-attachments/assets/c7ba884a-8443-4741-84d1-18e663a28d21)

![generator](https://github.com/user-attachments/assets/47bb4378-eae5-4169-a4f1-36f3bb9e3b4b)



---

### 4. **Mérési Eredmények**

- **Kimeneti Jel**: A kimeneti jel a generátor jelének 48,15%-a.  
- **Csillapítás/Átviteli arány**: A csillapítási érték 2,076 dB.  
- **Kimeneti/Bemeneti impedancia**: 450 Ω.

---

### 5. **Elemzés**
A π csillapító (pi pad) ellenállásáramkör elemzése révén megállapítható, hogy az áramkör hatékonyan csökkenti a jel amplitúdóját, miközben annak hullámformája lényegében változatlan marad. Az áramkör fő komponensei közé tartozik három precíz ellenállás, valamint egy terhelő ellenállás, amelyek közösen biztosítják az optimális csillapítást. A kiszámolt és a mért értékek közötti minimális eltérés a komponensek gyártási tűréshatárának következményeként értelmezhető.

### 6. **Következtetések**
Az áramkör sikeresen megvalósításra került, és a mérési eredmények alátámasztják, hogy a csillapítási teljesítmény megfelel a tervezett specifikációknak. Az áramkör optimális teljesítést nyújtanak a célzótt frekvenciatartományban, miközben a jelminőség nem romlik. A mérések során gyûjtött tapasztalatok hangsúlyozzák a komponensek tűréshatárainak és a környezeti feltételeknek az áramkör teljesítményére gyakorolt hatását.

### 7. **Javaslatok**

- **Komponens Tolerancia**: A jövőbeli tervezések során érdemes figyelembe venni a precízebb toleranciájú komponensek alkalmazását, hogy minimalizáljuk a mérési eltéréseket.
- **Hőmérséklet Hatások**: Az áramkör viselkedését különböző hőmérsékleti körülmények között is tesztelni kell, hogy pontosan meghatározható legyen a stabilitás.
- **További Frekvenciatesztek**: Szélesebb frekvenciatartományban végzett vizsgálatok további ránézést biztosíthatnak az áramkör átviteli karakterisztikáiról.
- **Automatizált Mérés**: Az ismérhetőség érdekében javasolt a mérési eljárások automatizálása.

---

**Aláírás:** Erős Bence

**Dátum:** 2024. 12. 18.


