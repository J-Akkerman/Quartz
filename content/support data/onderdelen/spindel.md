# **Spindel**

Een **spindel** is een mechanisch component dat een roterende beweging omzet in een **lineaire verplaatsing**. Spindels worden gebruikt in machines voor nauwkeurige positionering, krachtopbouw en herhaalbare lineaire bewegingen. 

## wrijving



# gpt
## **Werking**

Een spindel werkt door rotatie van een as die voorzien is van schroefdraad. In combinatie met een **moer** (lineaire lagering) ontstaat er een axiale verplaatsing. 

De basisrelatie is: 
$s=p\cdot n$ 
waar:
- $s$ = verplaatsing
- $p$ = spoed (mm/omw)
- $n$ = aantal omwentelingen
## **Belangrijkste soorten spindels**

### **1. Gewone trapeziumspindel (Tr-spindel)**

- Voordelig en robuust
    
- Geschikt voor middelmatige snelheden
    
- Zelfremmend bij lage spoed
    
- Hogere wrijving → lager rendement
    

**Toepassingen:** schroefpersen, eenvoudige lineaire actuatoren, verstelmechanismen.  
**Gerelateerde pagina:** [[lineaire actuator]]

---

### **2. Kogelomloopspindel (ballscrew)**

- Kogels rollen tussen schroefdraad en moer
    
- Hoog rendement (tot 95%)
    
- Lage wrijving → minder warmte
    
- Niet zelfremmend
    

**Voordelen bij ontwerp:**

- Hoge nauwkeurigheid en herhaalbaarheid
    
- Hoge snelheid bij lage weerstand
    
- Lage backlash bij voorbelaste moeren
    

**Toepassingen:** CNC-frezen, 3D-printers, precisieautomaten.

---

### **3. Rollerspindel / Rollerscrew**

- Gebruik van rollende cilindrische rollichamen
    
- Extreem hoge krachtcapaciteit
    
- Nauwkeurigheid vergelijkbaar met ballscrews
    

**Toepassingen:** zware industriële lineaire actuatoren, perssystemen, geavanceerde robotica.

---

## **Belangrijke parameters**

### **1. Spoed (pitch) $p$**

- Verplaatsing per omwenteling
    
- Grotere spoed → hogere snelheid, lagere kracht
    
- Kleinere spoed → hogere kracht, lagere snelheid
    

### **2. Efficiency (η)**

Gewone spindels: 30–70%  
Kogelomloopspindels: 85–95%  
Rollerspindels: 90–98%

### **3. Backlash**

De speling tussen moer en draadprofiel.  
Lagere backlash → hogere precisie.  
Kan worden gereduceerd met voorbelasting.

### **4. Kritische draaisnelheid**

Bij hoge rotatiesnelheid gaat de spindel trillen of doorbuigen.  
$ n_{krit} $ hangt af van:

- diameter
    
- lengte
    
- lagering
    
- materiaal
    

### **5. Stijfheid**

Welk deel van de totale stijfheid bepaalt verplaatsingsnauwkeurigheid onder belasting:

- spindelstijfheid
    
- moerstijfheid
    
- lagerstijfheid
    

---

## **Krachtberekeningen**

### **Axiale kracht (bij rendement η)**

[  
F = \frac{2 \pi, T, \eta}{p}  
]  
waar:

- $T$ = aangedraaid koppel
    
- $p$ = spoed
    
- $\eta$ = rendement
    

### **Benodigde motor voor gewenste verplaatsingssnelheid**

[  
v = n \cdot p  
]  
[  
n = \frac{v}{p}  
]

---

## **Voordelen en nadelen per type**

### **Trapeziumspindel**

- Goedkoop
    
- Zelfremmend
    
- Eenvoudige montage  
    − Hoge wrijving  
    − Minder geschikt voor hoge cycli
    

### **Kogelomloopspindel**

- Zeer lage wrijving
    
- Hoge nauwkeurigheid
    
- Hoge snelheid  
    − Duur  
    − Niet zelfremmend (rem nodig)
    

### **Rollerspindel**

- Zeer hoge krachten
    
- Extreem lange levensduur  
    − Duurste oplossing  
    − Complexe moeren
    

---

## **Typische toepassingen**

- CNC-routers en freesmachines
    
- Precisietafels
    
- Lineaire actuatoren ([[lineaire actuator]])
    
- Optische en meetapparatuur
    
- Zware perssystemen
    
- Robotica en automatisering
    

---

## **Leveranciers**

- **HIWIN** — kogelomloopspindels en lineaire systemen
    
- **THK** — high-end ballscrews
    
- **Bosch Rexroth** — lineaire techniek
    
- **NSK** — precisiespindels
    
- **SKF** — spindels en lageroplossingen
    

---

Als je wilt kan ik ook aparte pagina’s maken voor **kogelomloopspindels**, **trapeziumspindels**, of een pagina met **volledige berekeningen en ontwerpregels**.