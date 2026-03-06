Een **stappenmotordriver** stuurt de spoelen van de motor volgens een vooraf bepaald patroon. 
Elke puls van de besturingseenheid zorgt voor één stap van de motor.

**PAGINA IS EEN ROTZOOI**
# selectie
## Stappen Motor Specs

 **Rated current per phase**
- The driver moet minimaal deze [[stroom]] aan kunnen 
- pak 20-30% speelruimte tussen de driver en stappenmotor (getal van AI)
- voorbeeld: 1.5 A motor → min stroom driver ≥2.0 A

**Motor voltage** heeft invloed op het moment van de motor in hogere toeren, hoger voltage leidt tot hogere koppel. Het voltage toepasbaar zijn met het aanvoer voltage.

## Match Voltage and stroom Ratings

### 🔹 Supply voltage

Common ranges:
- Small motors: **8–35 V**
- Larger motors: **24–60 V**

Higher voltage helps with:
- Faster acceleration
- Less torque drop at speed

### 🔹 Current rating

- Check **continuous current**, not peak
- Ensure adequate cooling (heatsink/fan if needed)
  
## Microstepping

Microstepping improves smoothness and noise.

Popular choices:

- **A4988**: up to 1⁄16
    
- **DRV8825**: up to 1⁄32
    
- **TMC drivers**: up to 1⁄256 (interpolated)
    

---

## 5. Control Interface Compatibility

Make sure it works with your controller:

- **STEP / DIR** → Arduino, CNC, 3D printers (most common)
    
- **SPI / UART** → advanced configuration (TMC drivers)
    
- **Standalone** → DIP switches (TB6600-style)
    

---

## 6. Noise, Smoothness & Efficiency

If noise or vibration matters:

- Choose **Trinamic (TMC)** drivers
    
    - StealthChop → ultra-quiet
        
    - SpreadCycle → higher torque
        

If noise doesn’t matter:

- TB6600 / DM542 are rugged and simple
    

---

## 7. Protections & Reliability (don’t skip this)

Look for:

- Overcurrent protection
    
- Thermal shutdown
    
- Undervoltage lockout
    
- Short-circuit protection
    

Good drivers protect both the motor **and** your controller.

---

## 8. Typical Recommendations (Quick Picks)

### 🔹 Small NEMA 17 (3D printers, robots)

- **TMC2209** (best all-around)
    
- **DRV8825** (budget, higher voltage)
    
- **A4988** (basic, cheap)
    

### 🔹 Medium motors (CNC, camera sliders)

- **TB6600**
    
- **DM542**
    

### 🔹 High-performance / quiet motion

- **TMC5160**
    
- **TMC2130**
    

---

## 9. Common Mistakes to Avoid ❌

- Underrating current (causes missed steps)
    
- Using low supply voltage
    
- No heatsinking
    
- Using H-bridge drivers instead of chopper drivers
    

---


## driver aanstuuring
De driver ontvangt:
- **Step-signaal** → bepaalt het aantal stappen 
- **Direction-signaal** → bepaalt de draairichting 
- **Enable-signaal** → activeert of deactiveert de motor 

De driver genereert vervolgens de juiste **stroomverdeling over de fasen** van de motor.
## Microstepping
Moderne drivers gebruiken **chopper-regeling** en **sinusvormige stroommodulatie** om microstappen te maken. 
Hierbij wordt elke volledige stap verdeeld in meerdere kleinere stappen (typisch 8, 16, 32 of 256), wat resulteert in:
- Soepelere rotatie 
- Minder trillingen en resonantie 
- Hogere positioneringsresolutie 
## Aansturingsmethoden
| Type                     | Omschrijving                                        | Voordelen                                 | Nadelen                         |
| ------------------------ | --------------------------------------------------- | ----------------------------------------- | ------------------------------- |
| **L/R driver**           | Eenvoudige spanningsaansturing via serieweerstanden | Goedkoop, eenvoudig                       | Inefficiënt, beperkt toerental  |
| **Chopper driver**       | Pulsbreedtemodulatie (PWM) voor stroomregeling      | Hoog koppel bij hoge snelheden, efficiënt | Complexer, duurdere componenten |
| **Microstepping driver** | Continue stroomregeling met sinusvormige golf       | Zeer nauwkeurig, stil                     | Lager piekkoppel                |
## Ontwerp- en dimensioneringscriteria
Bij het kiezen of ontwerpen van een driver moet rekening worden gehouden met:
- **Nominale spanning** (V): afgestemd op motorwikkeling  
- **Maximale fase-stroom** (A): bepaalt koppel  
- **Microstepping-instelling**: resolutie vs. ruis  
- **Frequentiecapaciteit**: bepaalt maximaal toerental  
- **Koeling en behuizing**: passief, actief of via koelprofiel  
- **Communicatie-interface**: digitale of analoge sturing  

### Dimensionering voorbeeld
Voor een stappenmotor van 3 A per fase, 48 V voeding:
- Driver met minimaal 3 A RMS en 50 VDC voeding vereist.  
- Microstepping instellen op 1/16 voor balans tussen soepelheid en koppel.  
- Signaalbron: [[PLC]] of [[Arduino]] met step/dir-uitgang.

---

## Leveranciers en fabrikanten
Enkele toonaangevende producenten van motor drivers:

| Fabrikant                     | Specialisatie                                             | Website                                           |
| ----------------------------- | --------------------------------------------------------- | ------------------------------------------------- |
| **Trinamic (Analog Devices)** | Geavanceerde microstepping drivers en IC’s                | [trinamic.com](https://www.trinamic.com/)         |
| **Leadshine**                 | Industriële stepper- en servo drivers                     | [leadshine.com](https://www.leadshine.com/)       |
| **Oriental Motor**            | Compleet aanbod motoren met geïntegreerde drivers         | [orientalmotor.eu](https://www.orientalmotor.eu/) |
| **Nanotec**                   | Compacte, programmeerbare drivers voor [[stappenmotor]]en | [nanotec.com](https://en.nanotec.com/)            |
| **SEW-Eurodrive**             | Industriële servo- en frequentiedrives                    | [sew-eurodrive.nl](https://www.sew-eurodrive.nl/) |
| **Yaskawa**                   | Servo- en motion control systemen                         | [yaskawa.eu.com](https://www.yaskawa.eu.com/)     |
| **Delta Electronics**         | Servo drivers en frequentieregelaars                      | [deltaww.com](https://www.deltaww.com/)           |

### Dimensionering voorbeeld
Voor een stappenmotor van 3 A per fase, 48 V voeding:
- Driver met minimaal 3 A RMS en 50 VDC voeding vereist.  
- Microstepping instellen op 1/16 voor balans tussen soepelheid en koppel.  
- Signaalbron: [[PLC]] of [[Arduino]] met step/dir-uitgang.

---

## Leveranciers en fabrikanten
Enkele toonaangevende producenten van motor drivers:

| Fabrikant | Specialisatie | Website |
|------------|----------------|----------|
| **Trinamic (Analog Devices)** | Geavanceerde microstepping drivers en IC’s | [trinamic.com](https://www.trinamic.com/) |
| **Leadshine** | Industriële stepper- en servo drivers | [leadshine.com](https://www.leadshine.com/) |
| **Oriental Motor** | Compleet aanbod motoren met geïntegreerde drivers | [orientalmotor.eu](https://www.orientalmotor.eu/) |
| **Nanotec** | Compacte, programmeerbare drivers voor [[stappenmotor]]en | [nanotec.com](https://en.nanotec.com/) |
| **SEW-Eurodrive** | Industriële servo- en frequentiedrives | [sew-eurodrive.nl](https://www.sew-eurodrive.nl/) |
| **Yaskawa** | Servo- en motion control systemen | [yaskawa.eu.com](https://www.yaskawa.eu.com/) |
| **Delta Electronics** | Servo drivers en frequentieregelaars | [deltaww.com](https://www.deltaww.com/) |


## selectie
[Choosing the Right Stepper Motor Driver - YouTube](https://www.youtube.com/watch?v=LcE9TwGck0U)

Kies voordat je een driver gaat selecteren een [[stappenmotor]] die goed aan jouw eisen voldoet. 

> LET OP
> De datasheet klopt vaker niet als wel, gebruik deze meer als een richtlijn als voor definitieve data
### inputs en outputs

**input voltage** is afhankelijk van:
- de voltages die er in jouw systeem beschikbaar zijn
- de gekozen motor
  de aanvoer voltage is vaak een stuk hoger als de rated voltage van de motor.

**output current** moet aanzienelijk hoger zijn als de stroom waarmee je de motor wil aandrijven

**Logic inputs** zijn hoe je de driver aanstuurt, deze kunnen veel verschillen tussen verschillende versies. let op dat de aanvoer voltage overeen (kan) komen met jouw systeem.
### Driver features
**internal current sensing and regulation** zorgt dat je ene constante stroom in je stappenmotor behoud, bijna elke moderne stappenmotor heeft dit.

**step modes** geven aan hoeveel stappen er tussen je motors standaard stappen geplaatst kunnen worden. Als je bijvoorbeeld een motor hebt die stappen maakt van 1.8$\degree$ kun je met halve stappen 0.9$\degree$ stappen maken. Dit kan varieren van 1/2 stappen tot 1/24 stappen.

**Automatic current decay** [AN120\_Understanding\_MP6500.pdf](https://media.monolithicpower.com/document/AN120_Understanding_MP6500.pdf)

**Protections** Er zijn een hoop verschillende beschermingen, kies welke jij denkt dat nodig is

### current en voltage

**Low on resistance** geeft aan hoeveel weerstand de driver levert, dit is 