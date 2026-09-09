# Sztochasztika órai jegyzet

# Adminisztráció
Tóth Imre Péter

+36 20 537 2256

H épület 508

Fogadó óra: Kedd 12-14

Tanár kérte hogy **tegeződjünk** és bátran kérdezzünk előadás közben!

Piros pontokat oszt a tanár ha kérdezünk

Tanár Honlapja: <https://math.bme.hu/~mogy/>

Tárgy Honlapja: <https://math.bme.hu/~mogy/oktatas/VillamosMSc_Sztoch/VillamosMSc_Sztoch_2026osz.html>


Követelmények:
- 2db ZH (Házi feladat kérdések lesznek)
- Online házi feladatok moddleban (kicsi lesz a házi feladat súlya AI miatt)
- Vizsga

Cheat sheet hozható - csak a hivatalos hozható

---

# Jelölés

A tanár így szokta jelülni az ÉS jelet a halmazok között:

$$
A\ és \ B=A \wedge B = A \cap B = A \cdot B = AB
$$

---


# 1. Előadás - (2026.09.08)

# 1.2. Előadás - (2026.09.09)

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