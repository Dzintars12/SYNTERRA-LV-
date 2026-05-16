# ◉SYNTERRA X BLOCK BIZNESA UN SIGNĀLU ARHITEKTŪRA

## Mērķis

Šis dokuments definē X Block kā pirmo praktisko SYNTERRA biznesa un produktu virzienu.

X Block nav viss SYNTERRA projekts.

Tas ir pirmais dzīvais funkcionālais bloks:

```text
AI atbalstīts FX signālu ģenerators
+ privāta trading laboratorija
+ nākotnes traderu kopienas slānis
```

---

# 1. Galvenā Ideja

SYNTERRA sākas ar vienu praktisku problēmu:

```text
atbrīvot cilvēkus no tirgus analītikas rutīnas
```

Traderi pārāk daudz laika pavada:

- skenējot tirgu,
- pārslēdzot timeframe,
- pārbaudot setupus,
- sekojot signālu novecošanai,
- filtrējot tirgus troksni.

X Block mērķis ir samazināt šo rutīnu.

---

# 2. X Block Loma SYNTERRA

X Block kļūst par:

```text
pirmo SYNTERRA biznesa līniju
```

Tā uzdevums:

- ģenerēt FX signālu kandidātus,
- analizēt tirgus struktūru,
- pārbaudīt signālu derīgumu,
- attēlot signālu kvalitāti,
- atbalstīt manuālu vai automatizētu izpildi,
- radīt nākotnes diskusiju vidi ap signāliem.

---

# 3. Pamata Tehniskā Plūsma

```text
MT5 / Broker Data
↓
Python Analīzes Dzinējs
↓
AI Interpretācijas Slānis
↓
Signāla Kandidāts
↓
SYNTERRA X Block
↓
Lietotāja Lēmums
↓
Manuāla Izpilde / MT5 EA Izpilde
```

SYNTERRA darbojas kā koordinācijas mezgls.

MT5 nodrošina live tirgus datus un izpildi.
Python aprēķina.
AI interpretē.
Lietotājs saglabā kontroli.

---

# 4. Signālu Sektori

Signāli tiek sadalīti trīs sektoros.

---

## 4.1 Swing Sektors

Tipiskie timeframe:

```text
W1 / D1 / H4
```

Mērķis:

- ilgtermiņa signāli,
- augstā timeframe struktūra,
- lielākas kustības,
- mazāks troksnis.

---

## 4.2 Daytrade Sektors

Tipiskie timeframe:

```text
H4 / H1 / M15
```

Mērķis:

- intraday setupi,
- London / New York sesiju loģika,
- dienas tirgus struktūra,
- kontrolēta izpilde.

---

## 4.3 Scalp Sektors

Tipiskie timeframe:

```text
M5 / M1
```

Mērķis:

- ātri setupi,
- mikro struktūra,
- īss signāla dzīves ilgums,
- ātra izpildes loģika.

---

# 5. Signāla Dzīves Cikls

Katram signālam jābūt dzīves ciklam.

Iespējamie statusi:

```text
NEW
ACTIVE
AGING
WEAKENING
INVALIDATED
EXPIRED
COMPLETED
```

Katram signālam jāietver:

- izveides laiks,
- signāla vecums,
- expiration loģika,
- sektors,
- derīguma statuss,
- statusa maiņas iemesls.

---

# 6. Signālu Derīguma Dzinējs

X Block nedrīkst tikai ģenerēt signālus.

Tam arī jāpārbauda vai signāls vēl ir derīgs.

Derīguma pārbaude:

```text
Esošais Signāls
↓
Live MT5 Dati
↓
Python Derīguma Pārbaude
↓
AI Konteksta Pārbaude
↓
Signāla Statusa Atjauninājums
```

Python pārbauda objektīvos nosacījumus:

- cena aizgājusi pārāk tālu,
- entry vairs nederīgs,
- risk/reward izmainījies,
- tirgus struktūra salauzta,
- spread pieaudzis,
- volatility izmainījusies,
- signāls novecojis.

AI pārbauda kontekstu:

- vai tirgus loģika vēl derīga,
- vai scenārijs vēl aktīvs,
- vai setups nav kļuvis vājš,
- vai vajadzīgs jauns signāls.

---

# 7. Confidence Score

Katram signālam tiek piešķirts kvalitātes vērtējums:

```text
CONFIDENCE: 0–100%
```

Confidence var ietvert:

- higher timeframe alignment,
- struktūras kvalitāti,
- liquidity confirmation,
- order block kvalitāti,
- BOS kvalitāti,
- risk/reward kvalitāti,
- spread,
- session timing,
- volatility,
- news risk,
- vēsturisko rezultativitāti,
- AI konteksta confidence.

---

# 8. Personīgais Confidence Filtrs

Katrs lietotājs pats izvēlas minimālo confidence līmeni.

Piemēram:

```text
Minimum confidence: 80%
```

Tiek izmantoti tikai signāli virs 80%.

Vai:

```text
Minimum confidence: 50%
```

Tiek izmantots vairāk signālu, bet ar lielāku risku.

Tas ļauj katram lietotājam definēt savu riska personību.

---

# 9. Izpildes Režīmi

X Block atbalsta trīs izpildes līmeņus.

---

## 9.1 View Only

Lietotājs tikai redz signālus un pats manuāli izpilda tos savā terminalī.

Tas ir drošākais un bezmaksas piekļuves līmenis.

---

## 9.2 Manuāla Izpilde No X Block

Lietotājs pieslēdz savu MT5 caur SYNTERRA EA vai bridge.

Lietotājs redz signālu un spiež:

```text
APPROVE / EXECUTE
```

SYNTERRA nosūta komandu uz lietotāja MT5 terminali.

---

## 9.3 Automātiska Izpilde

Signāli tiek automātiski izpildīti lietotāja MT5 terminalī pēc viņa iestatījumiem.

Auto execution nekad nedrīkst būt noklusētais režīms.

Tam nepieciešams:

- lietotāja aktivizācija,
- risk settings,
- confidence filtrs,
- atļautie sektori,
- atļautie simboli,
- max daily loss,
- emergency stop.

---

# 10. Pakešu Struktūra

X Block var sastāvēt no trīs piekļuves līmeņiem.

---

## 10.1 Free Pakete

```text
View Only
```

Ietver:

- signālu redzamību,
- AI paskaidrojumus,
- confidence score,
- signālu statusus.

Izpilde notiek manuāli ārpus SYNTERRA.

---

## 10.2 Plus Pakete

```text
Manual Execution
```

Ietver Free funkcijas plus:

- MT5 savienojumu,
- manuālu approve no X Block,
- orderu nosūtīšanu uz MT5 EA,
- execution logus.

---

## 10.3 Premium Pakete

```text
Full Control Layer
```

Ietver:

- auto execution,
- confidence filtrus,
- sektoru filtrus,
- risk profiles,
- advanced AI analysis,
- signal personalization,
- execution settings,
- advanced logs,
- nākotnes private community funkcijas.

---

# 11. Biznesa Modelis

X Block atbalsta divus monetizācijas virzienus.

---

## 11.1 Affiliate Modelis

Lietotājiem kuri:

- vēl nav pie brokeriem,
- vai ir gatavi atvērt jaunus kontus.

Iespējamās affiliate kategorijas:

- brokeri,
- prop firms,
- VPS pakalpojumi,
- trading instrumenti,
- data provideri.

---

## 11.2 Abonēšanas Modelis

Lietotājiem kuri:

- jau ir brokeros,
- un nevar kļūt par affiliate lietotājiem.

Viņi var maksāt simbolisku platformas maksu par:

- signāliem,
- execution rīkiem,
- AI analīzi,
- automatizācijas iespējām,
- kopienas piekļuvi.

---

# 12. Nākotnes Chat Block

Otrais nākotnes SYNTERRA bloks var kļūt par privātu chat/community slāni.

Mērķis:

- apspriest signālus,
- analizēt signālu kvalitāti,
- dalīties ar market idejām,
- salīdzināt rezultātus,
- veidot uzticību starp dalībniekiem.

Signāli piesaista cilvēkus.
Kopiena notur cilvēkus.

---

# 13. Drošības Princips

X Block nav finanšu konsultācija.

Tā ir privāta AI-assisted trading analysis un execution vide.

Sistēmai:

- jāparāda uncertainty,
- jāizvairās no overconfidence,
- jāseko signālu novecošanai,
- jāatbalsta risk control,
- jāsaglabā lietotāja kontrole.

---

# 14. Galvenais Noslēguma Princips

X Block ir pirmā praktiskā SYNTERRA biznesa līnija.

Tā sākas ar vienu reālu vērtību:

```text
atbrīvot traderus no tirgus analītikas rutīnas
```

Ilgtermiņa virziens:

```text
AI-assisted trading intelligence infrastructure
```

nevis vienkāršs signālu kanāls.
