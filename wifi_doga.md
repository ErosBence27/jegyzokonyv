# Miskolci Szakképzési Centrum  
**Kandó Kálmán Informatikai Technikum**  
**Miskolc Palóczy u. 3.**

# MÉRÉSI JEGYZŐKÖNYV

**A mérést végző neve:** Erős Bence 

**A mérés tárgya:** Wifi Doga 

**A mérés száma:** 2. mérés  
**A mérés dátuma:** 2025. 02. 06  
**A mérést vezette:**  Csontos Dénes 

**Évfolyam:** 13. E  
**Csoport:** GYAK 2  
**Helyszín:** Fizikai Labor

---

## Wifi Doga Jegyzőkönyv

- Ez a jegyzőkönyv a Linksys router konfigurálását és a hozzá csatlakozó hálózati eszközök tesztelését rögzíti. A feladat során az IP-címek kezelése, a routing tábla ellenőrzése, ping tesztelés és egyéb hálózati parancsok végrehajtása történt.

---

## Használt Eszközök

| Eszköz                | Funkció                                                                 |
|-----------------------|-------------------------------------------------------------------------|
| Catalyst 2950 switch   | Biztosította a hálózati eszközök közötti kommunikációt.                |
| Linksys router         | A hálózati forgalom irányítását és központi vezérlését végezte.         |
| ThinkPad laptop        | A tesztelési folyamatokhoz használt eszköz, amelyen ping tesztek és egyéb hálózati parancsok futottak. |
| Mobiltelefon           | A Linksys routerhez való csatlakozást tette lehetővé, így pingelni tudtam a laptop és más eszközök között. |

---

## 01. A számítógép IP beállításainak lekérdezése

<details>
  <summary>Kép megtekintése</summary>
![ipconfig](https://github.com/user-attachments/assets/113ca128-9106-4d64-8856-ea6c014122bf)

  

</details>

## 02. Az aktuális IP-cím eldobása

<details>

  <summary>Kép megtekintése</summary>
![release](https://github.com/user-attachments/assets/9b791ee8-bd29-4ac8-93a8-97c014e31911)

  

</details>

## 03. Új IP-cím kérése

<details>

  <summary>Kép megtekintése</summary>
![renew](https://github.com/user-attachments/assets/32c16295-0fe8-4381-aa6c-71625acb84d4)

  

</details>

## 04. A routing tábla 

<details>

  <summary>Kép megtekintése</summary>
![netstat](https://github.com/user-attachments/assets/44836301-d866-4d40-93a5-fae4b308d74b)


</details>

## 05. A microsoft.com szerver elérhetőségének tesztelése

<details>

  <summary>Kép megtekintése</summary>
![ping_microsoft](https://github.com/user-attachments/assets/d813b3d6-e78b-4026-9881-3dbb6a86eb58)

  

</details>

## 06. Az www.ipon.hu szerver felé vezető útvonal lekövetése

<details>

  <summary>Kép megtekintése</summary>

  ![tracer_ipon](https://github.com/user-attachments/assets/3f6893e2-629f-465c-8a63-d4e0c9a1bf27)


</details>

## 07. Használt portok listázása

<details>

  <summary>Kép megtekintése</summary>
![netstat -a](https://github.com/user-attachments/assets/8a533980-69da-42f9-b610-84f3566872f0)

  

</details>

## 08. Hálózati kapcsolatok 

<details>

  <summary>Kép megtekintése</summary>
![netstat -an](https://github.com/user-attachments/assets/26e589b0-2c38-49f8-9721-fe0cedf5fe5a)

  
</details>

## 09. DNS-beállítások aktualizálása

<details>

  <summary>Kép megtekintése</summary>
![dns](https://github.com/user-attachments/assets/2aa26bbb-c02a-432e-bb9b-de81d2ef7060)

  

</details>

## 10. Csatolt hálózati meghajtók 

<details>

  <summary>Kép megtekintése</summary>

  ![net use](https://github.com/user-attachments/assets/b041e600-f1b8-48bd-b7d9-344466935605)


</details>

## 11. A www.ipon.hu tartománynév és IP-cím 

<details>

  <summary>Kép megtekintése</summary>
![nslookup_ipon](https://github.com/user-attachments/assets/491ffa30-659a-4f2e-a162-e3a452f9eba3)

  

</details>

## 12. Telefon Wifi-kapcs.

<details>
  <summary>Kép megtekintése</summary>

  
</details>

## 13. Router konfig

<details>
  <summary>Kép megtekintése</summary>
![router_config_1](https://github.com/user-attachments/assets/61640790-543a-42e4-8189-8859c7e74d91)

  
</details>

<details>
  <summary>Kép megtekintése</summary>

  ![router_config_2](https://github.com/user-attachments/assets/a80c1e72-e317-465a-b5fe-cda82154c91b)

</details>

<details>

  <summary>Kép megtekintése</summary>
![router_config_3](https://github.com/user-attachments/assets/29d51a61-419e-4830-bfee-7bc591f53790)

  
</details>

<details>
<summary>Kép megtekintése</summary>
  ![block_wan_ping](https://github.com/user-attachments/assets/7c472f26-0d37-45cb-bb76-db88ec5080c7)

</details>


## 14. Ping_PC ---> Telefon

<details>

<summary>Kép megtekintése</summary>
![ping_telefonra](https://github.com/user-attachments/assets/1283e75a-f727-4130-88a2-78cc0887dd8c)


</details>

## 15. SpeedTest

<details>

<summary>Kép megtekintése</summary>
![speedtest](https://github.com/user-attachments/assets/2099c4a7-46df-4f43-bb72-e5fe286fa20c)


</details>


## 16. Wifi Analyzer

<details>

<summary>Kép megtekintése</summary>


</details>

---

## Záró Összegzés

- A tesztelés során a **Linksys router**, a **Catalyst 2950 switch** és a többi hálózati eszköz problémamentesen működtek együtt. Az IP-konfigurációk kezelése, a routing tábla megjelenítése, valamint a különböző hálózati parancsok futtatása zavartalanul zajlott. A mobiltelefonos csatlakozás lehetővé tette a laptop és a többi eszköz közötti kommunikációt.


**Aláírás:** Erős Bence 

**Dátum:** 2025. 02. 06.
