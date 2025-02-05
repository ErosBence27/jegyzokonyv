# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** DVB-T jel fejállomásba küldése és IPTV rendszeren való kiadása <br>
**A mérés száma:** 02. mérés  
**A mérés dátuma:** 2025. 02. 03  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

## Bevezetés

- A földfelszíni digitális televíziózás **(DVB-T)** elterjedése lehetővé teszi a nagy felbontású és megbízható televíziós adások vételét különböző régiókban. A vizsgafeladat célja egy ilyen rendszer kiépítése, amely magában foglalja a megfelelő adótorony kiválasztását, a vételi jel méréseit és annak IPTV rendszeren keresztüli továbbítását. A Miskolc, Avasi adótorony jeleit fogva a DVB-T jel egy **LEMCO SCL-824CT** fejállomásba kerül bevezetésre, amely ezt követően IPTV streamként szolgáltatja a tartalmat. Az **IPTV rendszer** megfelelő működéséhez a multicast IP tartomány beállítása és a **Set-top-box konfigurálása** is szükséges.

---

## Mérési Cél

- A vizsgázó feladata egy földfelszíni digitális TV vételi rendszer kiépítése, a megfelelő adótorony **(Miskolc, Avasi adótorony)** kiválasztása, a jel mérésének és elosztásának elvégzése, valamint az **IPTV rendszer konfigurálása**.

- A fogható multiplexek jelerősségének ellenőrzése, és a DVB-T jel **LEMCO SCL-824CT** fejállomásba történő bevezetése. A fejállomásból a digitális tartalom IPTV streamként kerül kiadásra.

- A Multicast IP tartomány megválasztása és az **IPTV Set-top-box** konfigurálása a megfelelő vételhez.

---

## Alkalmazott eszközök:

| Műszer neve                                      | Típus       | Gyártási szám       |
| -------------------------------------------------| ------------| --------------------|
| LEMCO SCL-824CT                                  | LEMCO       |                     |
| MAG IPTV                                         | Set-top box |                     |
| METEK HDD                                        | METEK       |                     |
| P-2845F                                          | ISKRA       |                     |
| Archer C7                                        |TP-Link      |                     |

|Használt Szoftverek|
|-------------------|
|Iperf              |
|VLC                |
|Wireshark          |
|FFmpeg             |

---

## Vételi Paraméterek

| Paraméter         | Érték              |
|-------------------|-------------------|
| Antenna irányszög (Dny) | 234°         |
| Osztó típusa     | RF16              |
| Jelszint         | 51 dB             |
| MER (Modulációs hiba arány) | 25 dB  |
| Moduláció        | DVB-T / QPSK / 8K / 1/32 |
| Páratartalom     | 68%               |
| Légnyomás        | 1027 mBar         |
| Hőmérséklet      | 5°C               |
| Szélsebesség     | 3,2 m/s           |

---

## Fejállomás bemeneteire beérkező multiplexek

  - **Input 1**: Multiplex A
  - **Input 2**: Multiplex B
  - **Input 3**: Multiplex E 
  - **Input 4**: Miskolc Városi TV 

---

## Router Konfig

- Router Default IP 192.168.1.1
- Alapértelmezet Átjáró 192.168.1.1
- DHCP Konfig 192.168.1.100 - 192.168.1.249
- IGMP Snopping Procotol [<span style="color: #00FF00; font-weight: bold;">ON</span>]
- Lan1 --> Lan3 IPTV Bridge

---

## Mag IPTV Konfig

- Ethernet Auto DHCP Link Status [<span style="color: #00FF00; font-weight: bold;">UpLink</span>]
- USB-ről átmásoltuk a kimentet csatorna listát


## Mérési Eredmények

- Multicast csomagok []
- IPTV stream elemzése []
- Hálózati teljesítmény []
- Csomagvesztés []

---

## Lemco SCL-824CT Programok

| #  | Input  | Program címe          | OriginalService ID | LCN  | Encrypted | TS Output | OutputService ID | IP cím      | IP port | Protokoll |
|----|--------|----------------------|-------------------|------|-----------|-----------|----------------|------------|--------|-----------|
| 1  | Input 1 | M1 HD               | 100               | 0    | FTA       | 1         | 100            | 224.0.0.2  | 10001  | UDP       |
| 2  | Input 1 | M4 Sport HD         | 101               | 0    | FTA       | 1         | 101            | 224.0.0.2  | 10002  | UDP       |
| 3  | Input 1 | Duna HD             | 102               | 0    | FTA       | 1         | 102            | 224.0.0.2  | 10003  | UDP       |
| 4  | Input 1 | DunaW/M4Sport+      | 103               | 0    | FTA       | 2         | 103            | 224.0.0.2  | 10004  | UDP       |
| 5  | Input 1 | Kossuth Radio       | 130               | 0    | FTA       | 4         | 130            | 224.0.0.2  | 10005  | UDP       |
| 6  | Input 1 | Petőfi Radio        | 131               | 0    | FTA       | 4         | 131            | 224.0.0.2  | 10006  | UDP       |
| 7  | Input 1 | Bartók Radio        | 132               | 0    | FTA       | 4         | 132            | 224.0.0.2  | 10007  | UDP       |
| 8  | Input 1 | Dankó Radio         | 133               | 0    | FTA       | 4         | 133            | 224.0.0.2  | 10008  | UDP       |
| 9  | Input 2 | M2 HD               | 200               | 0    | FTA       | 1         | 200            | 224.0.0.2  | 10009  | UDP       |
| 10 | Input 2 | M5 HD               | 201               | 0    | FTA       | 2         | 201            | 224.0.0.2  | 10010  | UDP       |
| 11 | Input 2 | TV2                 | 202               | 0    | FTA       | 1         | 202            | 224.0.0.2  | 10011  | UDP       |
| 12 | Input 2 | RTL                 | 203               | 0    | FTA       | 1         | 203            | 224.0.0.2  | 10012  | UDP       |
| 13 | Input 2 | MAX4                | 206               | 0    | FTA       | 2         | 206            | 224.0.0.2  | 10013  | UDP       |
| 14 | Input 2 | Spektrum Home +     | 207               | 0    | FTA       | 2         | 207            | 224.0.0.2  | 10014  | UDP       |
| 15 | Input 2 | MinDig TV Plusz Info | 208              | 0    | FTA       | 2         | 208            | 224.0.0.2  | 10015  | UDP       |
| 16 | Input 3 | HEVC teszt          | 524               | 0    | FTA       | 2         | 524            | 224.0.0.2  | 10016  | UDP       |
| 17 | Input 4 | Miskolc TV          | 1000              | 0    | FTA       | 2         | 1000           | 224.0.0.2  | 10017  | UDP       |


---





