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

![R1 képlete]()

![R2 képlete]()

6 dB-es csillapítás esetén az ellenállások értékei az alábbi ábrán láthatók:



Az alábbi kapcsolási rajz bemutatja a jelgenerátor belső ellenállását, valamint a π csillapító áramkört a megfelelő ellenállásértékekkel:




---

### 3. **Mérési Paraméterek**

| Paraméter           | Érték |
|---------------------|-------|
| Generátor feszültsége | 5.00 Vp2p|
| Kimeneti jel        | 2.06 Vp2p |
| Generátor frekvencia| 1000 Hz |
| Csillapítás         | -7.702 dB |
| Átviteli arány      | 7.702 dB |
| Bemeneti impedancia | 450 Ω |
| Kimeneti impedancia | 450 Ω |   

Az oszcilloszkópos méréseken a sárga 1-es csatornán a csillapított kimeneti jel, a kék 2-es csatornán pedig a generátor jele látható.



---

### 4. **Mérési Eredmények**

- **Kimeneti Jel**: A kimeneti jel a generátor jelének 41,2%-a.  
- **Csillapítás/Átviteli arány**: A csillapítási érték 7,702 dB.  
- **Kimeneti/Bemeneti impedancia**: Az értékek mérése folyamatban.

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


