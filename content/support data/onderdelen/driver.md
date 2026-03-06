# Driver (Stappenmotor- en Servoantrieb)
Een **driver** (ook wel **motor driver**, **aandrijfversterker** of **regelunit**) is het elektronische systeem dat de elektrische aansturing van een [[stappenmotor]] of [[servomotor]] verzorgt. 
De driver vormt de **tussenlaag** tussen de besturing (zoals een [[PLC]] of microcontroller) en de motor, en bepaalt daarmee het gedrag, de snelheid, richting en nauwkeurigheid van de aandrijving.
## Functie
De primaire taak van een driver is het **omzetten van stuursignalen** (vaak digitale pulsen of analoge spanningen) in **gestuurde stromen** naar de motor. 
Hierbij regelt de driver:
- De **stroomsterkte** (bepaalt koppel en snelheid) 
- De **fasering** (bepaalt draairichting en stappositie) 
- De **microstepping of feedbackregeling** 
- De **beveiliging** (overstroom, temperatuur, spanningsval)

Drivers worden ontworpen voor specifieke motortypen, zoals:
- [[Stappenmotor]]en → **stepper drivers** 
- [[Servomotor]]en → **servo drivers** 
- [[DC-motor]]en → **PWM-drivers of H-bruggen**
## Drivers voor stappenmotoren
## stappenmotor driver
![[stappenmotor driver]]
## Drivers voor servomotoren
Een **servodriver** werkt in **gesloten regelkring** met een feedbacksensor (zoals een [[encoder]] of resolver).  
Het doel is om een exacte **positie, snelheid of koppel** te handhaven.

### Regelstructuur
Een servodriver bevat doorgaans:
1. **Positieregeling** (bepaalt gewenste positie)  
2. **Snelheidsregeling** (regelt de rotatiesnelheid)  
3. **Stroomregeling** (stuurt de wikkelingen aan)  

De driver vergelijkt continu de gemeten feedback met het ingestelde commando en corrigeert afwijkingen in real time.

### Communicatie
Servodrivers ondersteunen vaak industriële communicatieprotocollen:
- **CANopen**, **EtherCAT**, **PROFINET**, **Modbus**, **EtherNet/IP**  
Dit maakt integratie in geautomatiseerde [[CNC]]- en [[robotica]]-systemen mogelijk.

---

## Beveiliging en diagnostiek
Drivers zijn uitgerust met talrijke beveiligingen:
- Overstroombeveiliging (bescherming van spoelen)  
- Overspanningsbeveiliging (bij regeneratieve energie)  
- Thermische beveiliging (tegen oververhitting)  
- Onder- en overspanningsdetectie  
- Detectie van motorfouten (open fase, kortsluiting, stalls)

Veel moderne drivers hebben ook **diagnosefuncties**:
- USB- of seriële verbinding voor monitoring  
- Temperatuur- en stroomlogging  
- Automatische afstemming van parameters (“auto-tuning”)  

---

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

---

## Toepassingen
Drivers worden toegepast in uiteenlopende systemen:
- [[CNC]]-machines en positioneertafels  
- [[3D-printers]]  
- [[Robotica]] en pick-and-place systemen  
- Geautomatiseerde transportsystemen  
- Medische en laboratoriumapparatuur  
- Precisie-optische positionering  

---

## Zie ook
- [[stappenmotor]]  
- [[servomotor]]  
- [[CNC]]  
- [[PLC]]  
- [[encoder]]  
- [[motion control]]
