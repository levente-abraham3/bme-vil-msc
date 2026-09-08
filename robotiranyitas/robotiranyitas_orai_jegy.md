# Robotirányítás rendszertechnikája órai jegyzet

# Adminisztráció

|Oktató|Email|
|---|---|
|Dr. Kiss Domokos|<kiss.domokos@aut.bme.hu>|
|Dr. Tevesz Gábor|<tevesz@aut.bme.hu>|
|Bézi István|<bezi@aut.bme.hu>|
|Oláh István|<olah@aut.bme.hu>|

Előadás közepén lesz 10 perc szünet.

**Tantárgy weboldala**: <https://www.aut.bme.hu/Course/VIAUMA16> (be kell jelentkezni az AUT honlapjára)

**Részletes jegyzet**: 

Ajánlott, hogy a bejöjjenek és ne csak a jegyzetet olvassák otthon.

**Követelmények**:
- 1 nagyzárthelyi
- 1 opc. nagyfeladat (ld. szerdai gyakorlat)
- írásbeli vizsga (30% ZH + 70% vizsga)
- ZH: 2026.10.??. (??) 18h15-20h
- PZH: 2026.11.??. (??) 18h15-20h

RobonAUT verseny: <https://robonaut.aut.bme.hu/>

---

# 1. Előadás - Robotirányítási alapismeretek (2026-09-08)

Robotkar részei:
- Csuklók
- Szegmensek
- Végberendezés

Csuklótípusok:
- **T**: Transzláció
- **R**: Rotáció

Humaniod robotok a laborban:

|KUKA KR AGILUS-2|Mitsubishi RV-3SDB|
|---|---|
|![alt text](/robotiranyitas/img_orai_jegy/image-1.png)|![alt text](/robotiranyitas/img_orai_jegy/image-2.png)

Jelemzője hogy 6 csukló, 6 szabadság fokkal rendelkezik, és mimikálja az ember test mozgását.

Robotkarok irányítása lehet:
- **Pont-pont irányítás**
    - Koordinálatlan, kiadódó trajektória.
    - Egyes csuklók egymástól függetlenül végrehajtják a mozgást
- **Folytonos pályairányítás**
    - Folyamatos interpoláció, a közbenső pályapontok kiszámítása a mozgás során.

Euler csukó egy speciális eset amikor egy redukálható egy 6 csuklós robot 6×6 mátrix redukálható 4×4-re. Elvileg amikor a csukló rengelyek metszik egymást.




