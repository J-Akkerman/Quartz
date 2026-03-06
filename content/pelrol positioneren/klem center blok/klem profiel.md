---
prod/koop:
  - sub-part
identificatie: 8071218_05
kosten/eenheid:
productie kosten:
hoeveelheid: 1
---
![[klem profiel mechanisme|700x400]]
Hierboven is het concept van het klem profiel te zien. Hoewel deze simpel te tekenen is heeft elke maat een groot impact op:
- de hoeveelheid dat het [[aandrijf center]] naar voren beweegt 
- De slag die de hendel moet maken
- De startpositie van de hendel (en dus ook de eindpositie)
Hieronder is te zien hoe dit onderdeel getekend is en welke maten wat bepalen

Geklemde toestand is na berekeningen niet handig gebleken
# tekeningen
![[Pasted image 20260127133947.png]]
hierboven is de eerste schets van onderdeel 8071218_05 te zien. 
- 5.500 bepaald de slag wat het [[aandrijf center]] gaat bewegen. Hoe kleiner deze slag is hoe lichter het werk zal zijn 
- 60.000 Is de directe hoek die de hendel zal moeten draaien. 

![[Pasted image 20260127135257.png]]
hierboven staat de 2e schets, deze bepaald waar de [[hendel]] begint en eindigt in zijn slag. Met 0 staat deze recht naar achter wanneer het systeem los staat. UPDATE: Het is beter om 
het [[hendel]] draaipunt aan te passen op dit onderdeel 
# kracht berekeningen
**Let op** *deze berekeningen gaat ervan uit dat het profiel altijd contact heeft met het uiterste puntje. Dit is in werkelijkheid niet 100% correct. Ook is er geen rekening gehouden met wrijving. hierdoor zullen de benodigde krachten altijd een klein beetje hoger is als de berekeningen.*
De kracht die op de hendel uitgeoefend wordt kan berekend worden met de volgende formule:
$$F_{h}=\frac{L_{s}\cdot\cos\left(90-\alpha_s+\alpha_{h}\right)}{L_{h}}\cdot F_{k}$$
waarin:
$F_{h}$= De kracht van de hand
$L_{s}$= De slag die het [[aandrijf center]] maakt 
$\alpha_{s}$= De hoek die de hendel moet afleggen
$\alpha_{h}$= De hoek die de hendel al heeft gemaakt
$L_{h}$= De lengte van de [[hendel]] 
$F_{k}$= de klemkracht op de moer in de huidige positie. berekend met:
$$\frac{F_{k-max}}{\sin\left(90-\alpha_{s}+\alpha_{h}\right)}$$
waarin:
$F_{k-max}$= de maximale [[rubberen tip#klemkracht|klemkracht]] 
**Let op** *deze berekening gaat ervan uit dat de E module van het rubber constant is een zijn elastische toestand. Dit klopt niet volledig* [[Rubber]]
Deze formules kunnen en desmos geplugd worden met $\alpha_{h}$ als de variabelen voor de volgende grafiek:
![[Pasted image 20260127145210.png]]
