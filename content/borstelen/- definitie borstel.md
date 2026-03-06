de generale positie van de borstels zal afhankelijk van op welke manier de pelrollen ingeklemd worden. De kant waar de bramen verwijderd zullen worden zal ook de kant zijn waar de staalborstel gemonteerd moet worden.

~~omdat het afbraam systeem ook nog overwogen moet worden wil ik deze zo veel mogelijk ruimte geven. Het zal dus ideaal zijn als de staalborstel met dit systeem aan de meeloop center kant gemonteerd kunnen worden.~~

![[Pasted image 20251114100713.png]]
zoals in de foto hierboven te zien is er te weinig ruimte om de kunststof borstel onder de stappenmotor te plaatsen. Hierom moet de kunststof aan de rechterkant worden geplaatst. 
![[Pasted image 20251114103908.png]]
### afstanden
om de juiste afstand tussen de borstels te kiezen zal er rekeningen worden gehouden met 16666 en16665. deze meoten tegelijkertijd afgebraamd en geborsteld kunnen worden. Hieronder staat een analyse.
![[onderdeel positie]]
### oriëntatie
de kunststof borstel zal haaks op de pelrol moeten staan terwijl de staalborstel in dezelfde lijn moet staan als de pelrol. Dit betekend dat de motor van de staalborstel naar voor of achter gericht zal moeten worden terwijl de kunststof borstel in de lijn van de pelrol gemonteerd zal worden
## borstel inbrengen
de borstels zullen scharnieren ingebracht worden, om dit te realiseren zullen er 5 onderdelen nodig zijn: een scharnier war de motor overheen draait. 2 cilinder scharnieren (boven en onder), een cilinder en een frame om het allemaal bij elkaar te houden
### bovenste scharnier
#### positie keuze
deze positie word op basis van de [[- definitie borstel#scharnier positie keuze|staalborstel]] gedefinieerd
##### relatie tot motor
aan de achterkant van de motor zal een scharnier gemonteerd moeten worden om de juiste beweging te realiseren. Dit scharnier kan aan de bovenkant of onderkant van de motor gemonteerd worden. 
- bovenkant
  als er aan de bovenkant gescharnierd word kan dit zorgen voor een kleinere axiale afwijking van de borstel op de pelrol. Maar aan de bovenkant van de motor is minder ruimte als aan de onderkant
- onderkant
  meer axiale afwijking van de borstel op de pelrol
  meer ruimte als aan de bovenkant
omdat ik verwacht te weinig ruimte aan de bovenkant te hebben zal ik voor de onderkant/achterkant ontwerpen.

Hieronder is een schets van hoe de axiale afwijking (rood) zal plaats vinden. In deze schets is te zien dat er minder afwijking plaats zal vinden wanneer het scharnier hoog zit in relatie tot de motor. Het scharnier kan dus beter bovenaan gemonteerd worden.
![[borstel axiale afwijking]]
##### hoogte op frame
Met de hoogte van dit scharnier worden er 2 belangrijke factoren beïnvloed. 1 is de axiale afwijking die de borstel maakt tijdens rotatie, Als hiervoor geoptimaliseerd word blijkt het echter dat Het frame in de weg staat [[- definitie borstel#~~axiale afwijking optimalisatie~~]]. Deze afmeting moet dus gekozen worden op basis van wat er past na de aanpassingen die gemaakt zijn in het [[- definitie frame#staal borstel problemen|frame]].
![[Hoogte scharnier berekeningen]]
Hierboven staan een hoop maten gedefinieerd die gebruikt gaan worden om de maximale hoek (Alpha) te berekenen (gelimiteerd door het frame). Er zijn al een paar gegevens Bekend:
- P2y
  de verticale afstand tussen de scharnier en het contact punt van de versleten borstel (r=90mm) = **32.58 
- P2x
  De horizontale afstand tussen de borstel en het scharnier = **378.8mm**
- P1=P2 en worden dus P genoemd
  De afstand naar P1 is gelijk aan de afstand naar P2
- O1=O2 en worden dus O genoemd
  De afstand naar O1 is gelijk aan de afstand naar O2
- PO1y
  De verticale afstand tussen P en O = **11.3 mm**
- PO1x
  De horizontale afstand tussen P en O = **126.2 mm**
- O2y
  De verticale afstand tussen het scharnier en de bovenkant van de motor = **26.58 mm**
###### maximale hoek
![[Hoogte scharnier berekeningen]]
$$\alpha=\gamma-\beta$$
waarin:
$$\gamma=\tan^{-1}\left(\frac{O1_{y}}{O1_{x}}\right)$$
- $O1_{y}=P1_{y}-PO1_{y}$
- $O1_{x}=P1_{x}-PO1_{x}$
$$\beta=\tan^{-1}\left(\frac{O2_{y}}{O}\right)$$
- $O=\sqrt{O1_{y}^2+O1_{x}^2}$
Met deze formules blijven er nog maar 2 onbekende over: P1x en P1y, deze kunnen aan elkaar afhankelijk gemaakt worden met de volgende formules:
$$P1_x=\sqrt{P^2-P1_{y}^2}$$
waarin:
$$P=\sqrt{P2_{y}^2+P2_{x}^2}$$
En zo blijft er nog maar 1 variable over: P1y (en $\alpha$)
###### benodigde hoek
![[Hoogte scharnier berekeningen]]
De maximale hoek (alpha) zal vergeleken moeten worden met de benodigde hoek (Delta). Deze berekeningen zullen heel erg vergelijkbaar zijn met de maximale alpha berekeningen. 
$$\Delta=\zeta-\epsilon$$
waarin:
$$\zeta=\tan^{-1}\left(\frac{p1_{y}}{p1_{x}}\right)$$
$$\epsilon=\tan^{-1}\left(\frac{p2_{y}}{p2_{x}}\right)$$

###### grafiek en keuze
wanneer de benodigde hoek binnen de maximale hoek valt heb je een situatie die mogelijk is binnen de limitaties van het frame. Dit blijkt te zijn wanneer de scharnier 62.9mm (verticaal) van het contactvlak met de pelrol af zit (73.4 tot center van pelrol). Op deze positie moet het scharnier 374.36mm (horizontaal) van de pelrol af zitten.
![[Pasted image 20260109094329.png]]
###### ~~axiale afwijking optimalisatie~~
De hoogte van het scharnier zal ook invloed hebben op hoeveel axiale afwijking er zal plaatsvinden. Het is gewenst om de motor zo horizontaal mogelijk te houden. Omdat de pelrollen in diameter verschillen en de borstel kleiner word met gebruik zal er een positie moeten worden gekozen waar de uiterste maten de motor zo horizontaal mogelijk plaatsen. Deze uiterste maten zullen zijn bij: 
- de dunste pelrol en de meeste borstel slijtage
  de dunste pelrol (te vinden in [[pelrol dimensionering]]) heeft een radius van 10.5mm. De borstels worden in de afbraam cel vervangen wanneer deze een radius hebben van 90mm. dit is bij elkaar (min de hoogte van de tanden 1.9mm) 98.6mm
- de dikste pelrol met een verse borstel
  de dikste pelrol is te vinden in [[pelrol dimensionering]], deze heeft een radius van 13.5 mm. De borstel heeft vers een radius van 100mm, wat betekend dat de as van de motor 113.5mm onder de pelrol zit.
Als de as (wanneer deze horizontaal is) op $\frac{88.6+113.5}{2}=101.05\operatorname{mm}$ van de pelrol vandaan zit zal de motor zo horizontaal mogelijk zitten in de meeste situaties.

De juiste horizontale afstand tussen Het bovenste scharnier en de pelrol is:
de ideale afstand van de pelrol tot de as (101.05mm) - de verticale afstand tussen de as en het scharnier (57.42mm). **$101.05-57.42=43.63\operatorname{mm}$**
**MET DEZE MAAT KOMT DE MOTOR TE VEEL IN CONTACT MET HET FRAME DEZE MAAT MOET DUS ANDERS GEKOZEN WORDEN**


#### scharnier keuze
![[bovenste scharnier]]
#### frame verbinding
Omdat verbinden met het aluminium profiel met een M8 bout moet moet het scharnier nog aangepast worden om deze bouten aan te kunnen

![[frame strong stone]]
### borstel cilinder
![[borstel cilinder]]
### cilinder verbinding
De cilinder moet alleen axiaal belast worden, dit kan bereikt worden door beide verbindingspunten van de cilinder te verbinden met een scharnier. een standaard enkel assige scharnier aan de eindes van de cilinder moet voldoende zijn. hiervoor is een rear hinge goed geschikt. 

verder kan er door de aangrijppunten van de cilinder verstelbaar te maken de duwkracht op de pelrol aangepast worden. Omdat deze duwkracht grotendeels op goed gevoel gedefinieerd is klinkt dit wel als een goede extra feature. 
#### bovenste cilinder scharnier
![[bovenste cilinder scharnier]]
##### aangrijppunt/kracht verstellen
Om de vork goed te verbinden met het motor platform komt er een balk onder dit platform, deze balk zal de plaat verstevigen en een goed aangrijppunt maken voor de vork. 

De kracht die de borstel op de pelrol kan ingesteld worden op basis van de horizontale afstand tussen het aangrijppunt en de onderste scharnier. Om de juiste afstand per kracht te defineren kan er een formule opgesteld worden: ![[cilinder berekeningen]]
$$F_{d}=\frac{F_{g}\cdot b-F_{cy}\cdot x-F_{cx}\cdot d}{-a}$$
waarin:
$F_d$=de kracht op de pelrol
$F_g$= het gewicht van de motor (191.3 N)
a= de horizontale afstand tussen het onderste scharnier en de borstel (376mm)
b= de horizontale afstand tussen het onderste scharnier en het massamiddenpunt (330 mm)
d= de verticale afstand tussen het bovenste frame scharnier en de bovenste cilinder scharnier (164mm)
$F_{cy}$ & $F_{cx}$=de y en x kracht van de cilinder, berekend met:
$$F_{cy}=F_{c}\cdot\cos\left(\alpha\right)$$$$F_{cx}=F_{c}\cdot\sin\left(\alpha\right)$$
waarin:
F_c= 754N de kracht van de cilinder (te vinden in PLM)
$\alpha$= de hoek tussen de cilinder en de wand te berekenen met:
$$\alpha=\tan^{-1}\left(\frac{x_2}{C_{y}}\right)$$
$x_2$ = de horizontale afstand tussen het onderste en bovenste cilinderscharnier
$$x_2=x-17.5$$
$C_y$= de verticale afstand tussen het onderste en bovenste cilinderscharnier
$$C_{y}=\sqrt{c_{L}^2-x_2^2}$$
$C_{L}$= de lengte van de cilinder in de huidige situatie (140-640mm)
 de cilinder zal een maximale en een minimale lengte hebben. Er moet rekening gehouden worden met het feit dat de cilinder nog een stuk korter en langer moet kunnen worden vanuit de huidige situatie. De hoeveelheid dat deze moet kunnen veranderen is afhankelijk van de positie van beide scharnieren en zal in CAD gecontroleerd worden.

Voor de rest kunnen de bovenstaande formules in een grafiek gezet worden om hieruit de juiste posities van de scharnieren te berekenen.
![[{1813344E-4795-433F-B383-5501DD42793B}.png]]
Uit deze grafiek is te zien dat de ideale positie van de cilinder (wanneer deze 270mm lang is) ligt op x=228mm dit legt $C_y$ automatisch op 161mm

#WIP **wil ik later nog optimaliseren zodat de drukkracht verstelbaar is, maar ivm. tijd wordt dat nu nog niet gedaan**
#### onderste cilinder scharnier
![[onderste cilinder scharnier]]
## motor en mountplate
![[borstel motor]]
### motor mountplate
#docu doe documenteren welke beslissingen er zijn gemaakt
## borstel motor verbinding
![[borstel-motor adapter]]
## kosten
onderdelen:
- [[- definitie borstel#motor|motor]] *180 graden gedraaide stroom kast* 2x #SEW_eurodrive
  197.93 p/s
  395.86 euro
- [[- definitie borstel#motor mountplate|motor mountpalte]] #materiaal 8091965
- [[- definitie borstel#borstel cilinder|cilinder]] 2x #PLM #festo 400008451 
  26.65 p/s
  *53.3 euro totaal*
- [[- definitie borstel#scharnier keuze|bovenste scharnier]] 2x  #PLM 3845904
  32.28 p/s
  64.56 euro
- [[- definitie borstel#onderste cilinder scharnier|onderste cilinder scharnier]] 2x #materiaal 8083909
- [[- definitie borstel#bovenste cilinder scharnier|cilinder scharnier boven ]] 2x #PLM #festo 091400835
  30,57 p/s
  61.14 euro
- [[- definitie borstel#borstel motor verbinding|borstel motor verbinding]] 2x #materiaal 8082660
- [[- definitie borstel#frame verbinding|frame-scharnier verbindingen]] 4006243 16x #rose_kruger
  worden apart gerekend in [[TOTALE KOSTEN]]