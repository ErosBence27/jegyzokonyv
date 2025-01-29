# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** Komplex Távközlési Hálózat Tervezése, Telepítése és Mérése <br>
**A mérés száma:** 01. mérés  
**A mérés dátuma:** 2025. 01. 29  
**A mérést vezette:** Sándor Péter  

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** V3 Labor 

---

## Bevezetés

A vizsgafeladat során egy komplex távközlési hálózat tervezése, telepítése és mérése a célom. Ehhez különböző eszközöket – mint például a Mikrotik LHG18 LTE antenna, a Mikrotik nRay 60GHz mikrohullámú antenna szett és a SOHO router – kell használnom. Feladatom a gyári beállítások visszaállítása, a hálózati topológia megtervezése, az eszközök konfigurálása és a hálózat működésének tesztelése. 

A vizsgafeladat lehetőséget ad arra, hogy gyakorlati tapasztalatot szerezzek a távközlési hálózatok telepítésében és mérésében. Célom, hogy képes legyek a hálózati eszközök megfelelő konfigurálására és a hálózat teljesítményének értékelésére.

## Mérési cél

A mérés célja, hogy létrehozzak egy olyan távközlési hálózatot, amely az LTE és 60GHz-es mikrohullámú technológiák integrálásával stabil és nagy sávszélességű kapcsolatot biztosít. 

Feladatom az eszközök megfelelő konfigurálása, a hálózati forgalom optimalizálása, valamint a hálózat teljesítményének mérése és dokumentálása. Kiemelten figyelek az eszközök közötti kommunikáció stabilitására, a jelminőségi paraméterek – például RSRP, RSRQ, SINR, RSSI – monitorozására, valamint a hálózat késleltetésének és sávszélességének mérésére.

---


## Alkalmazott eszközök:

| Műszer neve                                      | Típus     | Gyártási szám       |
| -------------------------------------------------| ----------| --------------------|
| Mikrotik LHG18 LTE antenna                       | Mikrotik  |                     |
| Mikrotik nRay 60GHz mikrohullámú antenna szett   | Mikrotik  |                     |
| ASUS SOHO                                        | ASUS      |                     |


---

## Blokkvázlat:

![topologia](https://github.com/user-attachments/assets/a948cd32-2470-48fa-b8b2-47d84276ebc6)

---

## Hálózati eszközök és IP-címek

| Eszköz                              | Alapértelmezett IP-cím |
|-------------------------------------|------------------------|
| Mikrotik LHG18 LTE antenna          | 192.168.188.1          |
| Mikrotik nRay 60GHz antenna (Master)| 192.168.88.2           |
| Mikrotik nRay 60GHz antenna (Slave) | 192.168.88.3           |
| SOHO router (AP módban)             | 192.168.88.4           |
| Switch (opcionális)                 | 192.168.88.254         |
| Kliens laptop (DHCP)                | 192.168.88.100-250     |

|Használt Szoftverek|
|-------------------|
|Winbox             |
|Iperf              |


---

## Feladat megoldás

Első lépésként visszaállítottam a hálózati eszközök gyári beállításait.  

Ezután konfiguráltam az LTE antennát, amely a **192.168.88.1** IP-címet kapta, valamint DHCP-szerverként is működik, a címeket **192.168.88.100–192.168.88.250** tartományban osztja ki. A dátum is frissítésre került. A laptopot összekötöttem az antennával, beállítottam a megfelelő IP-címet a laptopra, hogy elérjem az eszközt. Ezen a ponton néhány tesztet is elvégeztem, melyek eredményeit az alábbi képek szemléltetik:

![teszt1-3](https://github.com/user-attachments/assets/aba3442a-a28c-479d-b5b0-e8b1bfb71450)

- Kapcsolat Állapota
  ![teszt1](https://github.com/user-attachments/assets/b574ba60-2c77-4ff0-b23e-a27880f5f5c1)




- Ezután következett a **Mikrotik nRay 60GHz** antennák konfigurálása. Az egyik eszközt **Slave**, a másikat **Master** üzemmódba állítottam be. IP-címeket kaptak: **192.168.88.2** és **192.168.88.3**. A dátumot, időt és jelszót szintén frissítettem.

- A következő lépésben az **ASUS routert** AP módba állítottam be, a szükséges IP-címekkel és felhasználói beállításokkal. Ezt követően a rendszer már elérhetővé vált, és megkezdhettem a tesztelést.  

---

## **Hálózati kapcsolatok ellenőrzése**  

A hálózat működését **ping parancsokkal** teszt

<details>
  <summary>Ping teszt a Google szerverre</summary>
![meres2](https://github.com/user-attachments/assets/743152f3-51f2-4e73-bd2f-a6777dac9128)



</details>

Következő a **Mikrotik nRay 60GHz** antennapár közötti kapcsolatot is teszteltem az **iperf** segítségével:
![meres4](https://github.com/user-attachments/assets/3c87c7bc-d395-4594-b1c4-fc0d18ef6e13)
![teszt utols2](https://github.com/user-attachments/assets/828c176f-c610-45b1-b9ff-95e6356c2d5e)


A laptopón **Speedtestet** végeztem:
![speed](https://github.com/user-attachments/assets/f39b4028-60e0-4992-a683-425a1c5e378c)


**Aláírás:** Erős Bence

**Dátum:** 2025. 01. 29.

