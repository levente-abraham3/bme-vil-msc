# Kvantuminformatika és -kommunikáció órai jegyzet

# Adminisztráció

|Oktatók|Email|Terem|Titulus / Tanszék|
|---|---|---|---|
|**Dr. Imre Sándor**|<imre@hit.bme.hu> <br> <imre.sandor@vik.bme.hu>|IB122|MTA rendes tag, egyetemi tanár (BME HIT)|
|Dr. Bacsárdo László|bacsardi@hit.bme.hu|IB121|Egyetemi docens (BME HIT)|

**Tantárgyi honlapok**:
- Kurzus weboldala: <https://www.mcl.hu/education/vihima18/>
- Quantum weboldal: <https://www.mcl.hu/quantum/>

**Kérdés és kapcsolat**:
- Központi kurzus email: <kvantumkurzus@mcl.hu> (az oktatók közösen olvassák)
- Hivatalos kommunikációs csatornák: **Microsoft Teams** és **Neptun**
- Konzultációk: Órák előtt/után, illetve előre egyeztetett időpontban

**Tanórák és időpontok**:
- **Előadás**: Hétfő 10:15–12:00 (IB025) és Csütörtök 14:15–16:00 (IE007).
- **Gyakorlat**: **Páros** heteken csütörtökönként 14:15–16:00 (IE007)

**Segédanyagok**:
- Moodle előadás diák (átismétlésre jók, de a teljes megértéshez az órai részvétel is szükséges)
- Ajánlott szakirodalom (könyvtárból kölcsönözhető és online megtalálható): ***Sándor Imre, Ferenc Balázs: Quantum Computing and Communications***.

**Követelmények és számonkérés**:
- **Házi feladat (1 db)**: Kiadás szeptember közepén, beadás **november közepén** Moodle-ban.
- **Zárthelyi dolgozat (ZH)**: **2026. december 7.** (óra közben?)
- **Kritérium / Minimumkövetelmény**: Mind a ZH-ból, mind a házi feladatból külön-külön el kell érni a **minimum 40%-ot** a félév elfogadásához!
- **Pótlási lehetőség (PZH)**: *"Dupla vagy semmi"* alapon javítható vagy pótolható a ZH.
- **Nagy házi feladat (NHF) kiváltása**: Kiváltható egy frappáns **versenyfeladat** kiagyalásával.
- **Vizsgaidőszak**: Szóbeli vizsga **2 tétellel** (*"egy könnyebb és egy még könnyebb"*).
- *Jótanács*: Az órai jelenlét előnyt jelent a vizsgakérdéseknél. Nem a pontos levezetések bemagolása a cél, hanem a protokollok és algoritmusok működési logikájának megértése.

**MI általános használata**:
- A VIK hivatalos ajánlása érvényes: <https://vik.bme.hu/hallgatoknak/altalanos/mi-hasznalat-ajanlasok>

**Kapcsolódó szabadon választható tárgyak**:
- **Kvantumszámítógépek programozása** (VIHIAV52): Őszi félév, 2 kredit, heti 90 perc (Qiskit, Q#, Azure Quantum, Cirq, Strawberry Fields)
- **Optikai kvantumkommunikációs rendszerek** (VIHIAV46): Őszi félév, 2 kredit, heti 90 perc
- **Optikai távközlési rendszerek** (VIHIAV50): Tavaszi félév, 4 kredit, heti 2×90 perc

---
# 1. Előadás - Bevezetés (2026-09-07)

## Fizikai korlátok és a kvantuminformatika születése 
- **Moore-törvény telítődése**: A transzisztorok méretének csökkenésével a nanométeres tartomány alatt a klasszikus fizika törvényei már nem érvényesülnek maradéktalanul.
- **Skálázhatósági kérdés (Slide 65)**: Elértük-e azt a megbízható alapegységet (transzisztorkaput), amely még hatékonyan skálázható klasszikus alapon.
- **Moore-törvény 2.0 (Qubit skálázódás)**: A kvantumos hardverek exponenenciális qubit-növekedést mutatnak. <br> (pl. IBM fejlesztési útiterv: 2016 Canary – 5 qubit, 2021 Eagle – 127 qubit, 2022 Osprey – 433 qubit, 2023 Condor – 1121 qubit)

## Kriptográfia és a kvantumos áttörés
- **Szimmetrikus titkosítás**: Ugyanazt a kulcsot használja mindkét fél; elméletileg abszolút biztonságos, de a kulcsmegosztás biztonságos csatornát igényel.
- **Aszimmetrikus titkosítás (RSA)**: Rivest–Shamir–Adleman algoritmus. Nyilvános titkosító és titkos fejtőkulcsot használ, melyek két nagy prímszám szorzatán ($N = p \cdot q$) alapulnak. Feltörése a prímtényezős felbontáson múlik.
- **Klasszikus vs. Kvantumos komplexitás**:
  - Klasszikus számítógéppel egy 300 jegyű szám prímtényezős felbontása kb. **152 000 évig** tartana
  - **Shor-algoritmus**: Kvantumszámítógépen $O(\log^3(N))$ időkomplexitással, mindössze kb. **1 másodperc** alatt képes feltörni az RSA-t.

## Fejlesztőkörnyezetek és nyelvek
Használt keretrendszerek: **Qiskit**, **Cirq**, **Q#**, **OPENQASM 2.0**

---
# 2 Előadás - Kvantuminformatika jelölésrendszere és posztulátumai (2026-09-10)

Ennek az órai anyaga benne szokott lenni a vizsgában, ne csak átpörgessük.

Posztulátom != Axioma

Különbség a mérnöki és fizika között

1. posztulátom: $\Phi(r,t)$ hely és idő
2. posztulátum: 

klasszik vs kvantum informácio közötti különbség

0 vagy 1  VS 0 és 1

Dirac bevezette a dirac formalizmust 

$$
\braket{0|0}
\bra{0} \ket{0}
$$

Hilbert tér: végtelen dimenzióu euklideszi tér

Azért mert szeretnénk a bizonytalan álapotoknak hosszat rendelni/mérni.

Plank állandó

és redukált plank állandó jelölés

Szuperpozició: egy időpillanatban egyszerre mindkét állapotban van.

Hadamard kapú: superpocicióba hozzak egy kvantum álapotot

Hadamart adjugált = önmaga

HH=I

Érdemes megjegyezni egyenletek:


Hadamard ker 0 az a 45°ba elforgatott bázis. Itt bármelyuk állapotba billenhet

justqlab folyamatosan forgat, nem a nullából indul

Mérési posztulátum kapcsolatot teremt klaszikus és kvantum állapot között. Miután megméred, utána fixen tudod az állapotát

Tenzor szorzás

SZámolás

## Kérdések:
Mi az a hullám operátor

Mi az a hermetikus?

Mi az az unitér? és unitér transformáció

# Verseny feladat

EA1 végén

Nyitott feladat keresés: Találni olyan feladatot ami Klasszikus és Kvantum között különbséget mutat.

---

# Túrórudi számláló

A tantárgy során az órai aktivitásért (kérdésekre válaszolásért vagy jó kérdések feltevéséért) pontok gyűjthetők, amiket ezen a tárgyon **"túrórudinak"** neveznek. A félév végén a tanszék beváltja a gyűjtött pontokat.

**Ábrahám Levente táblázata**:

|Dátum|Mennyi|Indok|
|---|---|---|
|2026.00.00|0|kérdeztem|

