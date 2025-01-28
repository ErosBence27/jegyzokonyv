# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence  
**A mérés tárgya:** Komplex Távközlési Hálózat Tervezése, Telepítése és Mérése <br>
**A mérés száma:** 01. mérés  
**A mérés dátuma:** 2025. 01. 28  
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

---


