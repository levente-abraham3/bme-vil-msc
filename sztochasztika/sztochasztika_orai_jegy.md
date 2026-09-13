# Sztochasztika órai jegyzet

## Adminisztráció és Elérhetőségek

- **Tárgy neve és kódja**: Felsőbb Matematika Villamosmérnököknek - Sztochasztika (BMETE90MX80)
- **Előadó**: Tóth Imre Péter
- **Előadások**:
  - Kedd 10:15–12:00 (IB025 terem)
  - Szerda 8:15–10:00 (IB027 terem)
- **Iroda**: H épület 508
- **Fogadóóra**: Kedd 12:00–14:00
- **Telefon**: +36 20 537 2256
- **Magatartás**:
  - Tegeződés, előadás közben bátran kérdezzünk!
  - Piros pont jár az órai kérdésekért, valamint a jegyzetekben/videókban talált hibák jelzéséért.
- **Oktató honlapja**: <https://math.bme.hu/~mogy/>
- **Tárgy honlapja**: <https://math.bme.hu/~mogy/oktatas/VillamosMSc_Sztoch/VillamosMSc_Sztoch_2026osz.html>


## Követelmények és pontozás (Összesen: 120 pont)
1. **Házi feladatok (Max. 15 pont)**
   - **Megtekintés / beadás**: [VIK Moodle honlap](https://edu.vik.bme.hu)
   - **Formátum**: Online kvízek (számszerű válaszokkal), akárhányszor próbálható.
   - **Határidő és pótlás**: Szabadon pótolható a pótlási hét végéig (2026-12-18).
   - **Értékelés**: A feladatok összpontszáma (max. 45 pont) **elosztva 3-mal** $\rightarrow$ max. 15 pont a végső jegybe.
   - *Megjegyzés*: A ZH-n és a vizsgán a feladatok legalább 20%-a a házi feladatokból származik!

2. **Zárthelyi dolgozat (Max. 45 pont)**
   - **1 db ZH** a félév közepe táján (valamint pótZH és pótpótZH).

3.  **Vizsga (Max. 60 pont)**
    - Írásbeli vizsga a vizsgaidőszakban.

---

**Aláírás feltétele**:
- HF pontszám 40% (min. **6 pont**) **ÉS**
- ZH pontszám 40% (min. **18 pont**).

**Sikeres vizsga feltétele**:
- Vizsgapontszám 40% (min.
**24 pont**).

**Érdemjegyek (Összpontszám alapján)**:
- **0–47 pont:** elégtelen (1)
- **48–67 pont:** elégséges (2)
- **68–87 pont:** közepes (3)
- **88–103 pont:** jó (4)
- **104–120 pont:** jeles (5)

**Megengedett segédeszközök**:
- Kizárólag a honlapon közzétett **hivatalos képletgyűjtemények**, eloszlás-táblázatok, valamint **zsebszámológép**.

---
# Jelölésjegyzék

A tanár így szokta jelölni az ÉS jelet a halmazok között:

$$
A \ \text{és} \ B = A \wedge B = A \cap B = A \cdot B = AB
$$

---

# 1. hét előadás - Val. szám alapok: valószínűség, függetlenség, várható érték, szórás

Szórás definició
$$
D^{2}X=VarX=\mathbb{E}[\left(X-m\right)^{2}]
$$

$$
DX=\sqrt{D^{2}X}=\sqrt{VarX}
$$

Tény: $VarX=\mathbb{E}(X^{2})=(\mathbb{E}X)^{2}$

## Feltételes valószunűség. Függetlenség

Definició: $\Omega$ eseménytéeren legye $A$ $B$ $\subset$ $\Omega$ esemény

Ekkor

$$
\mathbb{P}\left( B|A \right)=\frac{\mathbb{P}\left( A\ és\ B \right)}{\mathbb{P}\left( A \right)}
$$

Legfontosabb definició:

A és B független ha

$$
\mathbb{P}\left( B|A \right)=\mathbb{P}\left( B \right)
$$

Definició: Valószinűségi változók függetlensége

Legyen $\Omega$ eseménytér és $X$ $Y$: