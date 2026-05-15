# ◉SYNTERRA SISTĒMAS ARHITEKTŪRA

## Mērķis

Šis dokuments definē SYNTERRA galveno tehnisko arhitektūru.

◉SYNTERRA nav tikai mājaslapa vai spēle.

Tā tiek projektēta kā:

```text
mērogojama digitālās civilizācijas infrastruktūra
```

kur cilvēki, AI sistēmas, termināļi, integrācijas, servisi un nākotnes pasaules slāņi var sadarboties drošā un modulārā vidē.

---

# 1. Galvenais Arhitektūras Princips

SYNTERRA tiek būvēta kā daudzslāņu sistēma.

```text
Vienkārša Virsma
↓
Pasaules Interfeiss
↓
Piekļuves Slānis
↓
Backend Kodols
↓
AI Sistēmas
↓
Sandbox / Izpildes Slānis
↓
Ārējās Integrācijas
↓
Civilizācijas Atmiņa
```

Lietotājs redz vienkāršu pasauli.

Sistēmas dziļākie slāņi paliek:

- modulāri,
- droši,
- un mērogojami.

---

# 2. Frontend Slānis

Frontend ietver:

- ieejas lapas,
- First Contact sistēmu,
- World Hub,
- AI Gida interfeisu,
- identitātes sistēmu,
- termināļa interfeisu,
- zināšanu sektoru,
- portālus,
- nākotnes marketplace un servisu interfeisus.

Frontend nedrīkst saturēt:

- slepenās API atslēgas,
- brokeru piekļuves datus,
- maksājumu slepenos datus,
- privātās AI piekļuves,
- nedrošu izpildes loģiku.

Frontend galvenais uzdevums ir:

```text
prezentācija un mijiedarbība
```

---

# 3. Piekļuves Slānis

Piekļuves slānis definē:

```text
kas ir dalībnieks
```

Piekļuves līmeņi:

```text
Guest
Registered
Verified
Trusted Participant
Builder / Organization
Infrastructure Admin
```

Piekļuves slānis kontrolē:

- ko lietotājs redz,
- ko lietotājs drīkst darīt,
- kādas sistēmas var aktivizēt,
- kādas integrācijas var pieslēgt,
- kādas AI iespējas kļūst pieejamas.

---

# 4. Backend Kodols

Backend kodols nākotnē pārvaldīs:

- autentifikāciju,
- lietotāju kontus,
- e-pasta apstiprināšanu,
- 2FA,
- datubāzes operācijas,
- sesiju pārvaldību,
- API maršrutēšanu,
- AI maršrutēšanu,
- permissions sistēmu,
- audit logus,
- servisu koordināciju.

Backend ir:

```text
SYNTERRA aizsargātais centrs
```

---

# 5. AI Sistēmu Slānis

SYNTERRA AI nav viens čatbots.

Tā ir:

```text
specializētu AI sistēmu ekosistēma
```

Nākotnes AI sistēmas:

- AI Gids,
- Biznesa AI,
- Mūzikas AI,
- Trading AI,
- Izglītības AI,
- Radošais AI,
- Coding AI,
- Drošības AI,
- Organizāciju AI.

AI Gids ir pirmais orientācijas slānis.

Specializētie AI tiek aktivizēti caur:

- routing sistēmu,
- permissions,
- piekļuves līmeņiem.

---

# 6. Termināļa Slānis

SYNTERRA terminālis ir:

```text
universālais civilizācijas komandu interfeiss
```

Tas nākotnē var pārvaldīt:

- AI sistēmas,
- projektus,
- API integrācijas,
- Python izpildi,
- automatizāciju,
- biznesa sistēmas,
- radošās darba plūsmas,
- tirgus analīzi,
- infrastruktūras procesus.

Terminālis vienmēr darbojas caur:

```text
Permission Layer
↓
Backend Core
↓
Sandbox / Execution Layer
```

---

# 7. Sandbox / Izpildes Slānis

Šis slānis droši izpilda potenciāli riskantas darbības.

Piemēri:

- Python skripti,
- backtesti,
- aprēķini,
- AI automatizācija,
- trešo pušu kods,
- trading stratēģijas,
- datu apstrāde.

Sandbox galvenie principi:

- izolēta izpilde,
- resursu limiti,
- laika limiti,
- permissions pārbaude,
- audit logi,
- aizsardzība pret ļaunprātīgu izmantošanu.

---

# 8. Ārējo Integrāciju Slānis

SYNTERRA nākotnē var integrēt:

- TradingView,
- brokeru API,
- tirgus datu sistēmas,
- maksājumu sistēmas,
- AI API,
- datubāzes,
- automatizācijas platformas,
- komunikācijas servisus,
- creator tools,
- biznesa infrastruktūru.

Visas integrācijas tiek vadītas caur:

```text
drošu backend gateway sistēmu
```

---

# 9. Civilizācijas Atmiņa

Nākotnē civilizācijas atmiņa var ietvert:

- lietotāju progresu,
- identitātes vēsturi,
- projektu vēsturi,
- AI mijiedarbību,
- organizāciju vēsturi,
- pasaules notikumus,
- ekonomikas notikumus,
- audit trail sistēmas.

Atmiņai jābūt:

- permission-aware,
- privacy-aware,
- drošai,
- un mērogojamai.

---

# 10. Drošības Pamati

Drošības principi:

1. Nekādi slepenie dati frontendā.
2. API atslēgas tikai backend vault sistēmās.
3. E-pasta verifikācija aktīvai dalībai.
4. 2FA augstāka riska darbībām.
5. Trading sistēmām nepieciešama papildus aizsardzība.
6. Python un automatizācija darbojas sandbox vidē.
7. AI sistēmas ievēro permissions.
8. Kritiskās darbības tiek logotas.
9. Riskantas darbības prasa apstiprinājumu.
10. Platformas stabilitāte ir svarīgāka par haotisku brīvību.

---

# 11. Guest un Aktīvais Dalībnieks

## Guest

Var:

- izpētīt pasauli,
- lasīt,
- novērot,
- uzdot ierobežotus jautājumus,
- saprast sistēmu.

Nevar:

- veidot pastāvīgas sistēmas,
- pieslēgt API,
- izpildīt kodu,
- izmantot trading sistēmas,
- piekļūt privātai infrastruktūrai.

---

## Registered / Verified Participant

Pakāpeniski iegūst piekļuvi:

- identitātei,
- projektiem,
- AI sistēmām,
- integrācijām,
- servisiem,
- ekonomikai,
- termināļa funkcijām.

---

# 12. AI Routing Sistēma

AI Router nosaka:

```text
kurš AI palīdz konkrētajā situācijā
```

Piemērs:

```text
Lietotājs: “Gribu veidot biznesu”
→ Business AI

Lietotājs: “Palīdzi rakstīt mūziku”
→ Music AI

Lietotājs: “Analizē EURUSD”
→ Trading AI

Lietotājs: “Palaid Python aprēķinu”
→ Python Sandbox
```

Routing balstās uz:

- nodomu,
- piekļuves līmeni,
- risku,
- integrācijām,
- permissions.

---

# 13. Attīstības Fāzes

## Phase 1 — Static World MVP

Pašreizējā stadija:

- statisks frontend,
- GitHub Pages,
- onboarding,
- valodu sistēma,
- AI Guide prototips,
- dokumentācijas pamati.

---

## Phase 2 — Identity MVP

- reģistrācija,
- e-pasta apstiprināšana,
- piekļuves līmeņi,
- guest vs registered modelis,
- pamata profili.

---

## Phase 3 — Backend Core

- autentifikācija,
- datubāze,
- sesijas,
- API gateway,
- permission engine.

---

## Phase 4 — AI Router

- routing sistēma,
- specializētie AI,
- dokumentācijā balstītas atbildes,
- permissions.

---

## Phase 5 — Termināļa Izpildes Slānis

- sandbox komandas,
- Python vide,
- projektu darba telpas,
- API manager.

---

## Phase 6 — Marketplace un Ekonomika

- creator economy,
- servisi,
- subscriptions,
- organizācijas,
- marketplace infrastruktūra.

---

# 14. Galvenais Princips

◉SYNTERRA jāpaliek:

```text
vienkāršai virspusē
modulārai vidū
drošai kodolā
atvērtai malās
cilvēkcentrētai visur
```

Šis ir pamats:

```text
pārvērst SYNTERRA no eksperimenta
par dzīvu digitālās civilizācijas infrastruktūru
```
