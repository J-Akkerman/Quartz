---
prod/koop: koop onderdeel
leverancier: SEW_eurodrive
waar te vinden: "[sew-eurodrive.nl](https://www.sew-eurodrive.nl/os/catalog/default.aspx?language=en_US&country=NL)"
identificatie: DRN90S2/FI
kosten/eenheid: 197.93
hoeveelheid: 2
---

> [!NOTE] LET OP BIJ KOPEN
> de stroomkast moet op 180 graden liggen (aan de andere kant als stanaard)
### Cel motor
de motor die in de cel word gebruikt is de **[[3SIEK 80X-2C2]]** van [[BESEL]], Dit is een 1.5 Kw motor die niet meer geproduceerd lijkt te worden door BESEL. De enige plek waar deze motor te krijgen lijkt te zijn is: [3SIEK 80X-2C2 BESEL ...](https://www.tme.eu/no/en/details/3siek80x-2c2/electric-motors/besel/3siek-80x-2c2/). 
 [[BESEL]] lijkt wel een soortgelijke motor te produceren, dit is mogelijk de geupdate versie van de huidige motor: [[2SIE80x-2C]].
 
Alternatieven zijn mogelijk goedkoper, [[sew-eurodrive]] produceert een motor die soortgelijk lijkt te zijn: [[DRN90S2 FI]] 

### motor evaluatie
De actuele motoren zijn allemaal 1.5 Kw, dat klinkt naar mijn mening als een veel te zware motor.

Wanneer er online word gekeken lijkt het benodigde vermogen slechts 3/4 Hp (0.56 kW) te zijn: [Abrasive Wheel Brush...](https://www.tanisbrush.com/brushes-101/abrasive-wheel-brush-guidelines), [Brush Research](https://www.brushresearch.com/engineering-guide.php), [[brush power guide.pdf]] 

Een motor met een lager vermogen zal een stuk goedkoper en lichter zijn. Beide factoren zijn zeer gewild in de actuele situatie.

**volgens Frank is een 1.5 kW motor wel nodig**
### motor keuze
Dus de motors voor de borstels moeten 1.5 Kw zijn. de motors die in PLM te vinden zijn lijken duurder als nodig en het origineel is niet meer te verkrijgen. Er word hierdoor gekozen om van [[sew-eurodrive]] een motor te kopen.

Om met de SEW product configurator een product te selecteren worden de volgende factoren ingevuld:
![[Pasted image 20251112102839.png]]
- vermogen
  moet 1.5 zijn zoals geconcludeerd in "motor evaluatie"
- efficiëntie
  er word nu gekozen voor premium efficiëntie omdat er geen standaard effectief bestaat met een uptime hoger als 70%
- hoeveelheid polen
  omdat er 3000 RPM nodig is word er automatisch gekozen voor een 2 polige [[elektromotor]]
- duration factor
  de motoren zullen niet 100% van de tijd draaien, 70% klinkt als een goed minimum.
deze keuzes wijzen naar een [[DRN90S2 FI]]

De mounting methode en positie zullen gebaseerd worden op de \#borstel_inbrengen, hier is destijds een voet configuratie gekozen.

**IVM. met het frame moet de motor van de kunststof borstel de Terminal box position aanpassen naar 180 graden (tegenover de standaard positie). omdat het simpeler is om 2 identieke motors te kopen word er gekozen om beide motors op deze manier te bestellen.**
