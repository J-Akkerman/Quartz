---
prod/koop: koop onderdeel
leverancier: hepco motion
waar te vinden: "[[QBNL19481.pdf]]"
identificatie: FCC25 351BK1 DR NS CHK LH
kosten/eenheid: 37016
hoeveelheid: 1
---
### belasting
belasting op de kar:
- moment over rail: 4.841Nm
  ![[Rail moment]]de [[swingtool.pdf|swingunit]] heeft samen met de mounting setup een gewicht van 4.2 Kg en dus een neerwaartse kracht van 41.2 N. 
  Deze neerwaartse kracht zal een stuk van de rail af plaatsvinden en zal hier dus een moment creeëren van $41.2\cdot\frac{117.5}{1000}=4.841Nm$
- kracht over de rail:
  De neerwaartse kracht kan worden opgesplitst in krachten in de richting van de rail en krachten haaks op de rail met de volgende formulles:
  ![[rail belasting]]$$F_{t}=\sin\left(\alpha\right)\cdot F_{g}$$$$\sin\left(25\right)\cdot41.2=17.41N$$ $$F_{t}=\cos\left(\alpha\right)\cdot F_{g}$$ $$\cos\left(0\right)\cdot41.2=41.2N$$
    Waarin:
  $F_t$= tangiele kracht op de rail
  $F_h$= de haakse kracht op de rail 
  $F_g$= het gewicht van de [[swingtool.pdf|swingunit]] en het karretje 4.2 Kg
  $\alpha=$ de hoek van de rail, Max 25 graden
### kar keuze
[[No.7-fixed-centre-carriage-with-clamping-brake-02-UK.pdf]]
De karretjez zijn zeer afhankelijk van de [[rail]] die er gebruikt wordt, dit blijk een 159mm rail te zijn. Hierbij is een FCC25 159 nodig. hiervoor moet nog wel het lagertype gekozen worden.
- **FJ** = [[hepco track guide.pdf#page=20|Zelfinstellende lagerunit]]
  HepcoMotion Zelfinstellende lagers bevatten naaldlagers met kooi en zijn ontworpen om een axiale beweging (zelfinstelling) te voorzien van de V positie. Dit is met name van belang waar 2 ringen of V geleidingen parallel gemonteerd worden, zie toepassingsvoorbeeld
- **DR** = [[hepco track guide.pdf#page=19|Dubbelrijige lagerunit]]
  Het Dubbelrijige lager (DR) bestaat uit een buitenring uit één stuk met twee kogelbanen. Dit lager biedt meer belastingscapaciteit, levensduur en stijfheid en is minder gevoelig voor ophoping van vuil. De afmetingen zijn identiek aan het tandemlager. DR lagers zijn gevoeliger voor installatie toleranties en het wordt aanbevolen dat zij besteld worden met CHK optie
De dubbelrijige optie lijkt in dit geval beter omdat deze een hogere stijfheid heeft en minder gevoelig is voor vuil. Hier moet op recomendatie van hepco wel een extera keuring bij (CHK), lijkt verstandig om dit ook te doen.
Verder is er ook een optie voor een extra afdichting tegen vuil (NS) deze wordt ook mee genomen
Ook moet de rem aan de linker kant van de kar zitten om zo de andere onderdelen te ontwijken. dit wordt gedaan met de linkerhandige optie LH

De rest van de opties zijn niet relevant dus is de uiteingelijke keuze voor de kar een:
**FCC25 351BK1 DR NS CHK LH** Met de rem optie.
