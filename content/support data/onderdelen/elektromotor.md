# Elektromotor

Een **elektromotor** is een apparaat dat **elektrische energie omzet in mechanische energie** door middel van elektromagnetische inductie.
## Werkingsprincipe
Het basisprincipe van de elektromotor is gebaseerd op de [[Lorentzkracht]]:  
wanneer een elektrische stroom door een geleider in een magnetisch veld loopt, ondervindt deze een kracht loodrecht op zowel de stroomrichting als het magnetisch veld.

De fundamentele werking wordt beschreven door:
$$F = B \cdot I \cdot L \cdot \sin(\theta)$$
waarbij:  
- $F$ = kracht (N)  
- $B$ = magnetische fluxdichtheid (T)  
- $I$ = stroom (A)  
- $L$ = lengte van de geleider (m)  
- $\theta$ = hoek tussen de stroomrichting en het magnetisch veld
## Hoofdonderdelen

Een typische elektromotor bestaat uit:
- **Stator** – het stilstaande deel met elektromagneten of spoelen  
- **Rotor** – het roterende deel dat de mechanische kracht levert  
- **As** – brengt het koppel over naar het aangedreven systeem  
- **Lagers** – verminderen wrijving tussen rotor en stator  
- **Behuizing** – zorgt voor koeling en bescherming  
- **Ventilator** – voor warmteafvoer bij hogere vermogens  
## Typen elektromotoren

### 1. **Gelijkstroommotor (DC)**
Werkt op **gelijkstroom** en gebruikt vaak borstels en een commutator om de stroomrichting in de rotor te wisselen.  
- Voordelen: nauwkeurige toerentalregeling  
- Nadelen: slijtage van borstels  

**Varianten:**  
- Permanentmagneetmotor  
- Serieschakeling en parallelschakeling  

### 2. **Wisselstroommotor (AC)**
Werkt op **wisselstroom** en wordt het meest gebruikt in industriële toepassingen. 

**Soorten:**
- **Asynchrone motor (inductiemotor)** – meest voorkomende type, zoals bij [[BESEL]] en [[SEW-Eurodrive]] 
- **Synchrone motor** – rotor draait synchroon met het magnetisch veld 
### 3. **Stappenmotor**
Een [[stappenmotor]] beweegt in **discrete stappen** in plaats van continu. Hierdoor is precieze positionering mogelijk zonder feedbacksysteem. 
Wordt vaak gecombineerd met een [[driver]].
### 4. **Servomotor**
Een motor met geïntegreerde terugkoppeling (encoder of resolver) voor **nauwkeurige positie- en snelheidsregeling**.  
Veel gebruikt in automatisering en robotica.

---

## Vermogen en rendement

Het mechanisch afgegeven vermogen wordt berekend met:
$$P = T \cdot \omega$$  
waarbij:  
- $P$ = [[vermogen]] (W)  
- $T$ = koppel (Nm)  
- $\omega$ = hoeksnelheid (rad/s)

Het **rendement** ($\eta$) is het quotiënt van mechanisch en elektrisch vermogen:
$$\eta = \dfrac{P_\text{mechanisch}}{P_\text{elektrisch}}$$

---

## Aansturing en regeling

Voor een optimale werking worden elektromotoren vaak gecombineerd met:
- [[frequentieregelaars]] – voor snelheidsregeling bij AC-motoren  
- [[drivers]] – voor [[stappenmotor]]en  
- [[feedback actuator]]en – voor gesloten regelsystemen  

---

## Koeling en isolatie

Koelmethoden:
- **IC411:** zelfventilerend met externe ventilator  
- **IC416:** geforceerde koeling  
- **IC610:** watergekoeld  

Isolatieklassen volgens IEC 60085:
- Klasse B (130 °C)  
- Klasse F (155 °C)  
- Klasse H (180 °C)  

## Leveranciers
Enkele bekende fabrikanten van elektromotoren zijn:
- [[BESEL]]  
- [[SEW-Eurodrive]]  
- [[SKF]] (lagertechnologie)  
- [ABB](https://new.abb.com/motors-generators)  
- [Siemens](https://new.siemens.com/global/en/products/drives/electric-motors.html)  
- [WEG](https://www.weg.net/)  

