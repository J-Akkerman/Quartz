---
prod/koop: koop onderdeel
leverancier: festo
waar te vinden: PLM
identificatie: "400008451"
kosten/eenheid: 26.65
hoeveelheid: 2
---
~~de benodigde beweging realiseren lijkt het makkelijkste met een luchtcilinder, deze cilinders kun je ook instellen op een bepaalde druk waarbij ze altijd de correcte hoeveelheid kracht leveren op de pelrol, ongeacht diameter en slijtage van de borstels.~~

~~de factoren die belangrijk zijn bij het kiezen van een cilinder zijn als volgt:~~
- ~~stroke~~
	~~moet lang genoeg zijn om de verschillen in diameter van de pelrollen en slijtage van de borstel op te vangen.~~
	- ~~verschil in diameters: 7mm
	  het grootste verschil in diameter blijkt [[pelrol dimensionering|7mm]] te zijn (is wel de externe diameter, dus zal mogelijk iets kleiner verschil zijn)~~
	- ~~slijtage van staalborstel: 15mm
	  de gebruikte staalborstel die ik van Pieter heb gekregen is 30 mm kleiner als wat het origineel was. Om met deze slijtage alsnog contact te houden moet de borstel 15mm dichterbij bewogen kunnen worden. ~~
	~~dit betekend dat er een minimale slag van 22 mm nodig zal zijn wanneer de motor lineair verplaatst zou worden. Er is verder ook nog extra slag nodig zodat de borstel de pelrol wat meer ruimte kan geven , en er is minder slag nodig omdat er gebruik wrodt gemaatk van een scharnierend mechanisme.
	Omdat er zoveel variabelen zijn wordt er voor nu gezocht naar een cilinder met ongeveel 30mm slag (of meer)~~
- ~~connecties~~
  ~~Ik wil aan beide kanten graag verbinden aan een rear hitch om te zorgen dat er geen momenten in de cilinder komen-~
- ~~double of single acting
  Voor dit gebruik zal een single acting cilinder zat zijn, deze zijn vaak ook goedkoper. maar je kunt ook gewoon een kant open laten op een dubbele cilinder. **maakt dus niet uit**
3222510 lijkt het beste aan deze eisen te voldoen~~

~~de druk die er standaard word gebruikt in de fabriek is 6 Bar, de gekozen cilinder heeft een zuigerdiameter van 10mm en kan daarmee volgens de [[wet van pascal]] $p\cdot a=\left(6\cdot10^5)\cdot\left(\left(\pi\cdot5^2\right)\cdot10^{-3\cdot2}\right)\right)=47N$ liften.~~ Dat is veel te laag voor wat nodig is

Een snelle analyse van de benodigde kracht lijkt handig te blijken. 
met de onderstaande analyse kan er een cilinder uit PLM worden gekozen die voldoet aan:
- De minimum zuigerdiameter
  Is onder [[- definitie borstel#"snelle" analyse]] gedefineerd
- De minimum slaglengte
  Is onder [[- definitie borstel#"snelle" analyse]] gedefineerd
de volgende nummers zijn overwogen
-  090255827
  Voldoet bijna exact aan de slag, 5 mm extra op de diameter![[Pasted image 20251113153609.png]]![[Pasted image 20251113153712.png]]
- 3300322
  voldoet niet aan minimale slag op optimale punt, maar diameter is zo veel groter als nodig dat het ideale punt niet gebruiken niet nodig is![[Pasted image 20251113153919.png]]![[Pasted image 20251113154015.png]]
- ~~400004729~~
  voldoet niet aan minimum diameter
  ![[Pasted image 20251113154206.png]]
- 090255817
  voldoet ruim![[Pasted image 20251113154415.png]]![[Pasted image 20251113154354.png]]
- 400008451
  Voldoet ruim op de slag en met 3.5mm op de diameter![[Pasted image 20251113154912.png]]![[Pasted image 20251113154924.png]]
Ik ga kiezen voor 400008451 omdat deze mooi aan alle eisen lijkt te voldoen

er zijn later in het proces nog berekeningen gemaakt voor deze cilinder in [[- definitie borstel#aangrijppunt/kracht verstellen|dit hoofdstuk]]
#### "snelle" analyse
Deze analyse is niet voldoende voor de eindopstelling, deze worden puur gebruikt om (voor nu) een cilinder uit te kiezen die hoogswaarschijnlijk ook gebruikt blijft worden. **deze blijft inderdaad gebruikt worden** 
##### zuigers diameter op basis van de cilinder lengte
uiteindelijk moet de benodigde zuigerdiameter uitgerekend worden. De formules die uiteindelijk ingevuld moeten worden zijn als volgt:
$$D=\sqrt{A\cdot4}$$
waarin:
$A$=de benodigde oppervlak van de cilinder (in m^2), berekend met: $$A=F_c/p*1000$$waarin
p= druk in pascal = 600000 Pa
$F_c$ = de kracht op de cilinder in de situatie hieronder te zien
![[cilinder berekeningen]]
$$F_{c}=\frac{F_{cy}}{\cos\left(\alpha\right)}$$
waarin:
$M_{s}=F_{d}\cdot a+F_{g}\cdot b-F_{cy}\cdot x=0$
$$F_{cy}=\frac{F_{d}\cdot a+F_{g}\cdot b}{x}$$
$$\alpha=\sin^{-1}\left(\frac{x}{c_{l}}\right)$$
waarin:
- $a$ = de afstand tussen het scharnier en de borstel
- $b$ = de afstand tussen het scharnier en het massamiddenpunt van de motor
- $x$ = de afstand tussen het scharnier en de cilinder
- $C_l$ = de lengte van de cilinder
- $F_d$ = de kracht waarmee de borstel op de pelrol word geduwd
- $F_g$ = het gewicht van de motor
wanneer al deze formules in Desmos geplugd worden ontstaan de volgende grafieken:
![[Pasted image 20251112174125.png]]
het laagste punt op de deze grafiek geeft de ideale afstand van het scharnier op de x as en de minimale zuigerdiameter die hierbij nodig is.

##### benodigde slag op basis van de cilinder lengte
Voor elke lengte cilinder zal er een nieuwe situatie ontstaan die voor een verschillende slag zal vragen, dit is gelukkig geen complexe berekening:
![[cilinder berekeningen]]

$$\Delta C_{y}=\frac{\Delta B_{y}}{a}\cdot x$$
waarin:
- $x$ = de afstand tussen de cilinder en het scharnier
  word een variabel in de grafiek, maar word definitief besloten op basis van zuiger diameter hoofdstuk
- $a$ = de afstand tussen de borstel en het scharnier
- $\Delta B_{y}$ = Het verschil in hoogte van de borstel
  Aan het begin van dit hoofdstuk als minimaal 30mm gedefineerd
- $\Delta C_{y}$ = Het verschil in hoogte van de cilinder
$$\Delta C_{l}=\frac{\Delta C_{y}}{\cos\left(\alpha\right)}$$
waarin:
- $\Delta C_{l}$ = het minimale verschil in cilinder lengte (ookwel slag genoemd)
- $\alpha=\sin^{-1}\left(\frac{x}{c_{l}}\right)$
**Let op, deze berekeningen houden er geen rekening mee dat de motor verplaatst**
met deze formules ontstaan de volgende grafiek:
![[Pasted image 20251113094102.png]]

