# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence és Szabó Tamás

**A mérés tárgya:** Inter Vlan Routing 

**A mérés száma:** 1. mérés  
**A mérés dátuma:** 2025. 01. 09  
**A mérést vezette:**  Csontos Dénes 

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** Fizikai Labor  

# Inter VLAN routing jegyzőkönyv


A projekt során inter-VLAN routingot valósítottunk meg a "Router on a Stick" módszerrel, amely lehetővé teszi a különböző VLAN-ok közötti kommunikációt egyetlen router interfészen keresztül.

A **VLAN** (Virtual Local Area Network) egy logikai alhálózat, amely lehetővé teszi, hogy a hálózati eszközök csoportosítva legyenek, függetlenül a fizikai elhelyezkedésüktől, így javítva a hálózat biztonságát és teljesítémét.

Ezen kívül beállítottunk egy **DHCP-szervert** is, amely automatikusan kiosztja az IP-címeket a hálózati eszközöknek. A konfigurációt a Packet Tracer szoftverben végeztük, amely segített a hálózati beállítások egyszerű és vizuális megvalósításában.

A projekt célja a VLAN-ok közötti forgalom irányítása és az IP-címek automatikus kezelése volt, így biztosítva a zökkenőmentes hálózati működést.

---

## Topologia

![topologia](https://github.com/user-attachments/assets/1c3f711c-80c1-4bec-bd94-c1a46fd2b336)

---

## Használt Eszközök:

| **Eszköz**           | **Típus**             | **Sorozatszám** |
|-----------------------|-----------------------|-----------------|
| Laptop 2x            | HP ProBook 450 G7    | 5CD0161WBB      |
| Switch 2x            | Cisco Catalyst 1000  | -               |
| Router 2x            | Cisco 4221           | -               |
| Wireless Router      | Linksys WRT54gl      | -               |

---

## Addressing táblázat

| **Device** | **Interface**  | **IP Address**   | **Subnet Mask**  | **Default Gateway** |
|------------|----------------|------------------|------------------|---------------------|
| R1         | G0/0/1.10      | 192.168.10.1     | 255.255.255.0    | N/A                 |
|            | G0/0/1.20      | 192.168.20.1     | 255.255.255.0    |                     |
|            | G0/0/1.30      | 192.168.30.1     | 255.255.255.0    |                     |
|            | G0/0/1.40      | 192.168.40.1     | 255.255.255.0    |                     |
|            | G0/0/1.1000    | N/A              | N/A              |                     |
| S1         | VLAN 10        | 192.168.10.11    | 255.255.255.0    | 192.168.10.1        |
| S2         | VLAN 10        | 192.168.10.12    | 255.255.255.0    | 192.168.10.1        |
| WR_1       | AP ONLY        | AP ONLY          | AP ONLY          | AP ONLY             |
| PC-A       | NIC            | 192.168.20.3     | 255.255.255.0    | 192.168.20.1        |
| PC-B       | NIC            | 192.168.30.3     | 255.255.255.0    | 192.168.30.1        |

A hálózatot felszeleteltük több VLAN-ra. Ez segíti a hálózat átláthatóságát és irányítását.

---

## VLAN Táblázat

| **VLAN** | **Name**       | **Interface Assigned**                   |
|----------|----------------|-----------------------------------------|
| 10       | Management     | S1: VLAN 10, S2: VLAN 10                |
| 20       | Sales          | S1: GE0/6                               |
| 30       | Operations     | S2: GE0/18                              |
| 40       | Guest          | S2: GE0/24                              |
| 999      | Parking_Lot    | S1: GE0/2-4, GE0/7-24, GE0/1-2          |
|          |                | S2: GE0/2-17, GE0/19-24, G0/1-2        |
| 1000     | Native         | N/A                                     |

---

Elneveztük a WiFi-t úgy, mint egy igazi cégnél.

### Wireless Router AP WiFi:

- **SSID**: Guest_Free  
- **WPA2-PSK**  
- **Biztonság**: AES  
- **Passphrase**: Free12345

---

![összerakot](https://github.com/user-attachments/assets/0c50995b-bc2c-49e9-90c2-7d105c850142)

---

## A router-on-a-stick módszerhez létrehozott alinterfészek:

### R1 alinterfészek:

![brief](https://github.com/user-attachments/assets/7d7f6975-4c50-4e97-8a85-214db57fe3f2)



---

## A switcheken létrehozott különböző VLAN-ok:

### S1 VLAN-ok:

![S1_vlan](https://github.com/user-attachments/assets/087ed9b9-8085-4ff6-a80b-5749736250d8)


### S2 VLAN-ok:

![s2_vlan](https://github.com/user-attachments/assets/32717b83-9215-44b4-8693-59de7b965924)



---

## A Dinamikus IP cím kiosztásért felelős DHCP beállítások:

### DHCP Beállítások:

![dhcp](https://github.com/user-attachments/assets/1cc0bcd8-f1b1-444c-922e-5a79e6fd31ed)

![dhcp binding](https://github.com/user-attachments/assets/a7e8bb45-029e-4682-a65a-8100afdd62eb)


---

## A VLAN-ok közötti forgalom irányítás tesztelése különböző kliensekkel, pingeléssel:

- **Ping VLAN 20 → 30**
  
 ![Ping_PCA-PCB](https://github.com/user-attachments/assets/41b15034-1f88-4854-8d06-90e75987fd91)

- **Ping VLAN 20 → 40**
  
  ![Ping_PCA-LaptopA](https://github.com/user-attachments/assets/26ae9c4f-59cd-47f3-9162-812085b6b76c)

- **Ping VLAN 30 → 40**
  
  ![Ping_PCB-LaptopA](https://github.com/user-attachments/assets/61431883-4132-4a43-9972-1aed9976e942)

---

## Wifi Konfig:

![wifi_1](https://github.com/user-attachments/assets/1b1277b3-b0f2-4b5a-868c-3484a7c79b8c)

![wifi_2](https://github.com/user-attachments/assets/80f46a56-93d4-4b29-a9df-1239bbf1eb72)

![wifi_3](https://github.com/user-attachments/assets/43be472a-e6f6-413e-8629-4e2185765fdc)

---

## Konfigok:

[R1 Konfig](https://github.com/user-attachments/files/18359510/R1.txt)

[S1 Konfig](https://github.com/user-attachments/files/18359515/S1.txt)

[S2 Konfig](https://github.com/user-attachments/files/18359516/S2.txt)


---
 
**Aláírás:** Erős Bence Szabó Tamás

**Dátum:** 2025. 01. 09.
