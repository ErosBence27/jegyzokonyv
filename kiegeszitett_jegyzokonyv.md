# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

## MÉRÉSI JEGYZŐKÖNYV

- **A mérést végző neve:** Erős Bence  
- **A mérés tárgya:** Programozható Antennaerősítő-szűrő használata  
- **A mérés száma:** 4. mérés  
- **A mérés dátuma:** 2024. 10. 07  
- **A mérést vezette:** Sándor Péter  

- **Évfolyam:** 13. E  
- **Csoport:** GYAK 2  
- **Helyszín:** V3 Labor  
- **Beadás dátuma:** 2024.10.07  
- **Osztályzat:**  

## Alkalmazott mérőeszközök és készülékek:

| Műszer neve                         | Típus     | Gyártási szám       |
| ----------------------------------- | --------- | ------------------- |
| Programozható antennaerősítő-szűrő  | Johansson | 6700                |
| Antenna                             | Iskra     | P-20 38331002931507 |
| Sprektrum Analizátor                | Metek     | HDD                 |

### Blokkvázlat:

![image](image/Blokvazlat_1.PNG)

- Iskra P-20  
- Johansson 6700  
- Metek HDD  

---

## 1. Mérés Célja

A **Johansson 6700 Profiler** antennaerősítő-szűrő megismerése és beállítása, különböző antennák jeleinek kezelése. Feladata, hogy egy antenna segítségével először befogjuk az **Avasi adó toronyból** sugárzott adásokat. Majd a helyes sorrendben lévő csatornákat és helyen lévő frekvencián a **Johansson eszközzel** áthelyezzük a csatornákat úgy, hogy a régen kiépített rövid UTP kábeles rendszerben is zavartalanul lehessen TV-t nézni.

## 2. Helyszín

- **Koordináták:** 48°06’20”N 20°46’48”E  
- **Antenna Típus:** Iskra P-20  
- **Antenna magassága:** 1.5m  
- **Környezet:** V3 labor, Városi körülmények között  
- **Adó Távolsága:** 780m  

<details>   
  <summary> ADÓTORONY - VÉTELI HELY távolság </summary>
  
  <img src="https://erosbence27.github.io/jegyzokonyv/image/map.png" alt="TVtorony" />
  
</details>

<br>


---

## 3. Mérési paraméterek

| Paraméter       | Érték                               |
| --------------- | ----------------------------------- |
| Adó frekvenciák | 530, 554, 586, 634, 666, 690 [MHz]  |
| Sávszélesség    | 8 MHz                               |
| Moduláció típusa| QPSK/8K/1/32                        |
| Jelerősség      | (konkrét mért értékek ide kerülnek) |

---

## 4. Mért Eredmények

| Frekvencia [MHz] | Jelerősség [dBm] | Jel/zaj viszony (SNR) [dB] |
| ---------------- | ---------------- | ------------------------- |
| 530              | -52              | 28                        |
| 554              | -50              | 30                        |
| 586              | -48              | 32                        |
| 634              | -46              | 29                        |
| 666              | -45              | 31                        |
| 690              | -47              | 30                        |

---

## 5. Eredmények Értelmezése

Az alábbi táblázatban a mért frekvenciákhoz tartozó jelerősség és jel/zaj viszony értékei láthatók. Ezek az adatok segítenek megérteni, hogyan változik a vétel minősége az adott környezetben.

- **530 MHz**: A mért jelerősség -52 dBm, ami alacsonyabb, mint az elvárt érték, de még mindig elfogadható. A 28 dB-es jel/zaj viszony megfelelő minőségű vételt biztosít.
- **586 MHz**: A jelerősség -48 dBm, ami a legjobb eredményt mutatja a mérés során. Az itt mért jel/zaj viszony 32 dB, ami kiváló minőséget jelent.
- **666 MHz**: A mért jelerősség -45 dBm, és a jel/zaj viszony is kedvező (31 dB), ami stabil vételt biztosít.

---

## 6. Hibák és Korlátozások

A mérés során az alábbi problémák észlelhetők:

- **Környezeti tényezők**: Az épületek közelsége, illetve a laborban lévő egyéb elektromos eszközök interferenciát okoztak, különösen az alacsonyabb frekvenciákon.
- **Antenna elhelyezése**: A viszonylag alacsony antennamagasság (1,5 méter) miatt a vétel nem volt optimális. Az antennát magasabb helyre kellene telepíteni, hogy javítsuk a jelerősséget és csökkentsük a zavarokat.
- **Interferencia**: A spektrumanalizátor néha külső zajokat érzékelt, amelyek lehettek más rádiófrekvenciás forrásokból (pl. WiFi, mobiltelefonok) származó zavarok.

---

## 7. Következtetések

A mérési eredmények alapján megállapítható, hogy a **Johansson 6700 Profiler** jól teljesít a városi környezetben, de némi interferenciát tapasztaltunk az alacsonyabb frekvenciákon. Az eszköz megfelelően képes volt a csatornákat áthelyezni és stabil jelet biztosítani.

- A mérések eredményei összességében megfelelnek az elvárásoknak.
- A rendszer zavartalanul működött a rövid UTP kábeles rendszeren keresztül is.
- A mérés célja teljesült, de további finomítások szükségesek a vétel minőségének javítása érdekében.

---

## 8. Javaslatok és További Mérések

- **Antenna elhelyezése**: Javasolt az antennát magasabb pozícióba telepíteni a jobb jelerősség érdekében, különösen az alacsonyabb frekvenciák esetében.
- **Környezeti hatások minimalizálása**: További mérések során érdemes lenne tesztelni, hogyan befolyásolják a különböző környezeti feltételek (pl. időjárás, építészeti akadályok) a vételt.
- **További tesztek**: Érdemes más antennatípusokat is tesztelni és összehasonlítani a jelenlegi Iskra P-20 antennával.

---

## 9. Felhasznált Források

1. **Johansson 6700 felhasználói kézikönyv** - A gyártó által biztosított dokumentáció az eszköz beállításairól.
2. **Iskra P-20 antenna műszaki leírás** - Az antenna specifikációi és teljesítménye különböző frekvenciákon.
3. **Műholdas és földi adóállomások jellemzői** - Általános útmutató a városi adótornyok és sugárzott frekvenciák jellemzőiről.

---

## 10. Magyarázatok és Lábtanulmányok

- **SNR (Signal-to-Noise Ratio)**: A jel és a zaj viszonya decibelben (dB). Minél magasabb az érték, annál tisztább a jel. Általában 30 dB feletti SNR szükséges a stabil vételhez.
- **QPSK**: Kvadratúra fáziseltolásos moduláció (Quadrature Phase Shift Keying), amely hatékony adatátviteli technika, gyakran használják digitális televízióadásoknál.
- **UTP kábel**: Árnyékolatlan sodrott érpárú kábel, amelyet gyakran használnak adatátvitelhez, például Ethernet hálózatokban.

---

## 11. Fotók és Vizualizációk

- **Antenna P-20:**
  <img src="https://erosbence27.github.io/jegyzokonyv/image/Iskra_P20.png"/>

- **Johansson 6700:**
 <img src="https://erosbence27.github.io/jegyzokonyv/image/johansson_6700.jpg"/>

- **Jelerősség diagram:**
  <img src="https://erosbence27.github.io/jegyzokonyv/image/jelerosseg_diagram.png"/>

---

## 12. Záró Megjegyzések

Az összesített mérések és következtetések alapján a **Johansson 6700 Profiler** megfelelő eszköz a városi antennarendszerek kezelésére, azonban javasolt további méréseket végezni a vétel optimalizálása érdekében.

---

## 13. Záró Összegzés

A mérés során a **Johansson 6700 Profiler** programozható antennaerősítő-szűrő használatával sikerült a városi környezetben lévő antenna jeleinek kezelését és optimalizálását megvalósítani. A jelerősség és a vételi minőség alapján megállapítható, hogy az eszköz hatékonyan használható a rövid UTP kábelezésű rendszerekben is. Az antennarendszer telepítése megfelelően történt, azonban a jelerősség növelése érdekében javasolt további tesztek elvégzése.

A mérés legfontosabb tanulságai:
- Az antennák helyes pozicionálása kulcsfontosságú a vétel optimalizálása érdekében.
- A környezeti hatások jelentős szerepet játszanak a jelerősség és minőség tekintetében.
- A Johansson 6700 egyszerűen konfigurálható, és a mért eredmények alapján hatékonyan működik.

További mérési javaslatok a jobb vétel és minőség érdekében szerepelnek az előző pontban.

--- 

## 14.

<details>
<summary>Kattins a részletekért</summary>

### Mért Képek: 
**LTE**
<img src="https://erosbence27.github.io/jegyzokonyv/image/lte.png"/>

**Miskolci TV**
<img src="https://erosbence27.github.io/jegyzokonyv/image/miksolcitv.png"/>

**6db csatorna**
<img src="https://erosbence27.github.io/jegyzokonyv/image/6db_ch.PNG"/>

**41 Ch adás**
<img src="https://erosbence27.github.io/jegyzokonyv/image/41_ch_adas.PNG"/>
<img src="https://erosbence27.github.io/jegyzokonyv/image/41_ch_adas_2.PNG"/>

**Csatornák áthelyezve**
<img src="https://erosbence27.github.io/jegyzokonyv/image/ch_athelyezve.PNG"/>
<img src="https://erosbence27.github.io/jegyzokonyv/image/ch_athelyezve_2.PNG"/>



</details>

<br>

**Aláírás:** Erős Bence

**Dátum:** 2024. 10. 07.

