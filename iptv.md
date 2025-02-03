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

- A Multicast IP tartomány megválasztása és az IPTV Set-top-box konfigurálása a megfelelő vételhez.

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







