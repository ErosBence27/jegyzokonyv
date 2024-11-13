# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** Bitsebesség vs jelminőség mérés
**A mérés száma:** 3. mérés  
**A mérés dátuma:** 2024. 10. 14  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

# Mérési Jegyzőkönyv

### 1. Mérési feladat
Ismerkedés a **Johansson 8202 DVB-T modulátor** képességeivel, valamint a bitsebesség és jelminőség vizsgálata. A célunk a műszer alapos megismerése volt.

### 2. Alkalmazott mérőeszközök és készülékek

| Eszköz                     | Típus                       | Funkció                                           |
|----------------------------|-----------------------------|---------------------------------------------------|
| Johansson 8202             | DVB-T modulátor            | Bitsebesség és jelminőség vizsgálata              |
| RF kábel                   | Koaxiális kábel            | Modulátorok és spektrumanalizátor összekötése     |
| Metek HDD                  | Spektrum/jelszint analizátor| Frekvencia, moduláció, sávszélesség, jelszint, MER és bitsebesség mérése |


### 2. Előkészületek
A mérés során a két Johansson 8202 DVB-T modulátort összekötöttük, majd az egyik modulátor **RF-out** pontját csatlakoztattuk a spektrumanalizátorhoz. Az eszközök megfelelő beállítását követően megkezdtük a mérést.


### 3. Mért Adatok - TV2 Erős és TV1 Pongo
A következő paramétereket olvastuk le a spektrumanalizátorról és a modulátor kijelzőjéről:

| Paraméter       | TV2 Erős 10Mb/s       | TV2 Erős 21.5Mb/s | TV1 Pongo       |
|-----------------|----------------|-----------------------|-----------------|
| MER             | 36.8 dB        | 36.2 dB              | 34.2 dB         |
| Packet Errors   | 0              | 0                    | 0               |
| Noise Margin    | 19.5           | 20.2                 | 18.3            |
| Power           | -34.4 dBm      | -34.8 dBm            | -29.3 dBm       |
| Bitsebesség     | 7.5 - 9.2 Mb/s | 11.2 - 18.6 Mb/s     | 10 - 12.8 Mb/s  |



### 4. Következtetés
A mérések során megismertük a **Johansson 8202 DVB-T modulátor** alapvető képességeit, és pontos adatokat kaptunk a bitsebességről és jelminőségről. A mérési eredmények alapján a modulátor megfelelő teljesítményt nyújtott, és a jelszint, bitsebesség, valamint a MER értékek a várakozásoknak megfelelően alakultak.Azonnal láthatóvá válik, hogy a TV1 Pongo magasabb bitsebességgel és erősebb teljesítménnyel dolgozik, míg a TV2 Erős jobb MER értékkel bír.

## 5. Mért Képek:
<details>
<summary>Kattins a részletekért</summary>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/674_spek.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/674_meter.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/674_bit.bmp"/>

<br>
<img src="https://erosbence27.github.io/jegyzokonyv/image/682_spek_10mb.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/682_meter_10mb.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/682_bit_10mb.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/682_meter_21.5mb.bmp"/>

<br>

<img src="https://erosbence27.github.io/jegyzokonyv/image/682_bit_21.5mb.bmp"/>

<br>


</details>
