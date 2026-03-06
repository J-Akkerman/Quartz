# Stappenmotor
Een **stappenmotor** is een [[elektromotor]] die elektrische pulsen omzet in **rotatiestappen**. In tegenstelling tot een gewone [[elektromotor]], die continu draait, beweegt een stappenmotor in nauwkeurig gecontroleerde hoeken. Hierdoor kan de positie, snelheid en richting van de as **zonder terugkoppeling**([[open-loop besturing]]) worden geregeld.

## Werkingsprincipe
De motor ontvangt pulsen vanuit een [[stappenmotor driver]]. elke puls word  omgezet naar een specifieke hoeveelheid rotatie, ookwel staphoek genoemd.
Door in een specifieke volgordepulsen te sturen roteert de motor in kleine, vaste stappen.

De **staphoek** wordt bepaald door:
$$\theta = \frac{360°}{N_p \times N_f}$$
waarbij:
- $N_p$ = aantal poolparen van de rotor 
- $N_f$ = aantal fasen van de stator 

Typische staphoeken zijn **1,8° (200 stappen per omwenteling)** of **0,9° (400 stappen per omwenteling)**. Deze staphoek word eigenlijk altijd aangegeven op de stappenmotors
## Typen stappenmotoren
### 1. Permanente magneet (PM)
- Rotor bevat permanente magneten.  
- Eenvoudig ontwerp, relatief lage resolutie (7,5° – 15° per stap).  
- Toepassing: eenvoudige positionering, printers, kleinschalige aandrijvingen.
### 2. Variabele reluctantie (VR)
- Rotor bestaat uit zacht ijzer met tanden; geen permanente magneten.  
- Lage koppel maar hoge precisie door kleine tandstappen.  
- Wordt vaak gebruikt in meetinstrumenten en lichte positioneringssystemen.

### 3. Hybride stappenmotor
- Combineert eigenschappen van PM en VR.  
- Zeer hoge precisie (1,8° of kleiner), hoog koppel en goede dynamische eigenschappen.  
- Veel gebruikt in [[CNC]]-machines, 3D-printers, en [[robotica]].

## Aansturing
Stappenmotoren worden bestuurd door een **[[stappenmotor driver]]** die de stroompulsen naar de spoelen regelt. Verschillende aansturingsmethoden beïnvloeden de resolutie en soepelheid:
### 1. Volstapmodus
Elke spoel wordt volledig bekrachtigd. 
→ Maximale kracht, maar minder soepele rotatie.
### 2. Halfstapmodus
Wisselt tussen het bekrachtigen van één of twee spoelen. 
→ Verdubbelt het aantal stappen, resulteert in een vloeiendere beweging.
### 3. Microstepping
De stroom door de spoelen wordt sinusvormig gemoduleerd. 
→ Zeer soepele rotatie, hogere resolutie (tot 256 microstappen per stap). 
→ Minder koppel per microstap, maar ideaal voor nauwkeurige positionering.
## Koppelkarakteristiek
Het **koppel** van een stappenmotor is frequentieafhankelijk. 
Bij hogere stapfrequenties neemt het beschikbare koppel af door inductieve reactantie in de spoelen.

- **Holding torque** – maximaal koppel bij stilstand. 
- **Pull-in torque** – maximaal koppel bij directe acceleratie.  
- **Pull-out torque** – maximaal koppel zonder stappenverlies tijdens rotatie.  

Grafisch wordt dit weergegeven in een *[[koppel-frequentiekromme]]*, die essentieel is bij motorselectie.
## Beperkingen
- Geen feedback: bij overbelasting kunnen stappen verloren gaan. 
- Beperkt toerental: efficiënt bij lage snelheden (<1000 rpm). 
- Resonanties: mechanische vibraties bij bepaalde frequenties.  
- Hoog stroomverbruik bij stilstand (voor behoud van houdkoppel).
## Voordelen
- Hoge positioneringsnauwkeurigheid zonder [[encoders]] (in open-loop).  
- Eenvoudige regeling via digitale pulsen. 
- Hoge betrouwbaarheid door afwezigheid van borstels. 
- Goed voorspelbaar dynamisch gedrag.
## Vergelijking met andere motoren
| Eigenschap               | Stappenmotor       | [[Servomotor]]               | [[DC-motor]]     |
| ------------------------ | ------------------ | ---------------------------- | ---------------- |
| Besturing                | Open-loop          | Gesloten-loop (met feedback) | Analoge regeling |
| Precisie                 | Hoog               | Zeer hoog                    | Matig            |
| Koppel bij lage snelheid | Hoog               | Hoog                         | Laag             |
| Koppel bij hoge snelheid | Laag               | Hoog                         | Hoog             |
| Kostprijs                | Laag tot gemiddeld | Hoog                         | Laag             |
## Leveranciers
Enkele bekende fabrikanten en leveranciers van stappenmotoren zijn:
- [Oriental Motor](https://www.orientalmotor.eu/) – specialist in stappenmotoren en drivers voor automatisering.  
- [Nanotec](https://en.nanotec.com/) – levert hybride en precisie-stappenmotoren met geïntegreerde besturing.  
- [Phytron](https://phytron.eu/) – stappenmotoren voor extreme omgevingen (zoals cryogene of vacuümtoepassingen).  
- [Sanyo Denki](https://www.sanyodenki.com/) – hoge betrouwbaarheid, veel gebruikt in industriële automatisering.  
- [Trinamic (Analog Devices)](https://www.analog.com/en/brand/trinamic.html) – produceert geavanceerde aansturings-IC’s en modulaire oplossingen.  

