# positie en beweging analyse
Nadat de borstels gedefinieerd zijn is er besloten dat de afbramer aan de linkerkant van het systeem geplaatst zal worden. Dit is ook de kant waar het klem center blok zit, wat ervoor zorgt dat er goed rekeningen gehouden moet worden met beschikbare ruimte.

Om te kijken hoeveel ruimte er beschikbaar is heb ik in creo een mockup gemaakt die op de juiste positie staat voor de meest "extreme" pelrol spoed. Hiermee kan gekeken worden hoe de omgeving van de swingunit eruit zal zien
## mogelijke positie analyse
### situatie 1, horizontaal op de pelrol
Horizontaal op de pelrol geplaatst kunnen worden lijkt de ideale situatie te zijn. Dit is het meest vergelijkbare met de geautomatiseerde cel.
![[Pasted image 20251114121905.png]]
Er is makkelijk te zien dat deze configuratie geen optie is ivm. het geleiding systeem.
### situatie 2, verticaal op de pelrol
De tool zal in deze configuratie aan 2 kanten van de pelrol contact kunnen maken
achteraan: (afstand tot de spindel kan aangepast worden in het [[- definitie klem center blok]])
![[Pasted image 20251114122322.png]]
vooraan: 
![[Pasted image 20251114122542.png]]
De beweging van de swingunit zal mogelijk complexer zijn in deze configuratie. Heb wel al ideeën om dit op te lossen$\delta$
### situatie 3, iets ertussenin
![[Pasted image 20251114124607.png]]
![[Pasted image 20251114124648.png]]


## concept keuze
Ik zie op het moment van ontwerp 3 type oplossingen die hieronder (links in tekening) zijn omschreven:
![[afbramer wegrtekken]]
- optie 1, de spindel verplaatsen en het gehele systeem linear in en uit verplaatsen
  zeker de meest simpele en betrouwbare optie. Houd wel rekening mee dat het [[- definitie klem center blok]] dan niet voorbij de swingtool kan bewegen.
- optie 2, een punt linear laten verplaatsen en de rest mee trekken langs een pivot blok.
  heeft veel valkuilen:
  - buigkracht in de cilinder
  - slijpschijf kan niet los hangen omdat deze aangeduw moet worden
  - waar haal je de ruimte vandaan
  - hoe ga je dit kunnen verstellen
    allemaal op te lossen, maar word wel snel complex
- optie 3, wegdraaien net zoals de [[- definitie borstel]] scharnieren
  - Neemt veel ruimte in waarvan ik niet zeker ben dat deze bestaat, 
  - onhandig met kap, 
  - dicht op klem center blok
  - schuin over meerdere assen is verwarrend en dus een vergroote kans op fouten


Dus optie 1 lijkt bij ver de beste keuze te zijn en gaat verder uitgewerkt worden.
# Hoek positionering
Ik wil gebruik gaan maken van [[hepco track guide.pdf|gebogen track guides]] om de positie van de swingunit te bepalen. [[slijphoek instellen]]
## rail
![[rail]]
### mountplate
De mountplate moet zorgen dat de rail (en dus ook de swingtool) in de juiste positie geplaatst kan worden. Deze moet hierop:
- De rail kunnen monteren
- een klein beetje naar boven beneden en de zijkanten afgesteld worden.
- stijf genoeg zijn om eventuele trillingen op te vangen
- verplaatst kunnen worden over de x as door de [[- definitie afbramer#axiale aandrijving|axiale aandrijving]]
- het karretje limiteren zodat deze niet van de rail af kan vallen
![[Pasted image 20260116111203.png]]
hier wordt gebruik gemaakt van een 3mm dikke plaat die gekant is rond een aluminium profiel, zo ontstaat er zo veel mogelijk stijfheid om eventuele trillingen tegen te gaan.
verder is de plaat afgesteld zodat de afbraam schijf op de ideale locatie zit, er is wel genoeg tolerantie ingebouwd dat deze 1mm all kanten op kan bewegen
verder zijn er stukken gezet die het karretje tegen gaan houden. Deze zijn zo afgemeten dat deze niet in contact kunnen komen met het [[- definitie klem center blok]].
### verbinding naar actuator
de mountplate kan vastgemaakt worden aan het alu profiel met [[bl_aluprofilsystem_en.pdf#page=87|stot stone -N- 4006201]]. Deze worden ook gebruikt voor het [[- definitie borstel#frame verbinding]], omdat deze in bulk ingekocht moeten worden lijkt het handig om deze te blijven gebruiken.
Voor de rest wordt er direct in de actuator geschroefd.
## karretje
![[carrige]]
### swingtool aan kar monteren
om de swingtool aan de kar te monteren wordt het onderstaande ontwerp gebruikt. Omdat dit een gekante plaat is is dit sterk zat om het gewicht van de [[swingtool.pdf]] te ondersteunen. Verder zorgt dit onderdeel ervoor dat de swingtool op de juiste afstand van de pelrol zit. dit kan ook gedaan worden door de lineaire actuator te verplaatsen, maar dan ontstaan er problemen met de rail mountplate die tegen het klem center blok aan komt. 
![[Pasted image 20260116135153.png]]
# slijpschijf inbrengen
## lineaire actuator
![[lineaire actuator afbramer]]
## frame verbinding
Het systeem zal aan het frame vast gemonteerd moeten worden, dit moet een stevige connectie zijn om te zorgen dat alle krachten goed doorgeleid kunnen worden naar het frame. het frame en de geleiding hebben beide een f30 profiel. 

Het blijkt dat rose+kruger hier geen oplossing voor heeft, een custom connector optie is gelukkig niet moeilijk te maken.
![[Pasted image 20260107134201.png]]
Dit onderdeel past in de groef van het f30 profiel. het word eerst tegen de lineaire actuator aangeschroefd met [[bl_aluprofilsystem_en.pdf#page=87|stot stone -N- 4006201]], en vervolgens aan het frame met dezelfde stenen.
## motor(verbinding)
Omdat er geen specifieke eisen zijn waar deze motor aan moet voldoen ga ik kiezen voor dezelfde stappenmotor als die van [[spindel en aanhang]]. 

Het verbinden van deze motor aan het mechanisme te verbinden blijkt nog een kleine uitdaging te zijn. Er is namelijk niet genoeg ruimte om de motor in het verlengde van de spindel te monteren.
![[{32B9D9CD-5F06-4B98-A8EC-8B21CFBB1EB4}.png]]
Om dit alsnog op te lossen zal de motor naar boven verplaatst worden, Hiermee word de verbinding wel ingewikkelder als een simpele as-as verbinding. Het meest handige idee lijkt een tandriem te zijn. Met het gebruik van een tandriem kan de motor boven de spindel geplaatst worden waardoor deze uit de weg blijft van alle andere onderdelen.![[{875A33C8-DD77-41AA-87DB-28023B49C3F9}.png]]
In deze oriëntatie is er een minimale as-afstand van 44 mm. Het is handig om hier wel een paar mm boven te zitten om de riem nog wel te kunnen plaatsen. 
### pulleys
![[pulleys]]
### riem
![[riem]]
### spannen en asafstand
Omdat de riem langer is als nodig in de huidige situatie moet de asafstand verlengd worden. Deze afstand word berekend met:
$$e=\frac{L_{d}}{4}-\frac{\pi}{8}\cdot\left(d_{g}+d_{k}\right)+\sqrt{\left\lbrack\frac{l_{d}}{4}-\frac{\pi}{8}\cdot\left(d_{g}+d_{k}\right)\right\rbrack^2-\frac{\left(d_{g}-d_{k}\right)^2}{8}}$$
$$\frac{187.5}{4}-\frac{\pi}{8}\cdot\left(42.97+12.7\right)+\sqrt{\left\lbrack\frac{182.5}{4}-\frac{\pi}{8}\cdot42.97+12.7)\right\rbrack^2-\frac{\left(42.97-12.7\right)^2}{8}}=46.23\operatorname{mm}$$

waarin:
- $L_d$ = definitieve riemlengte 182.5mm
- $d_g$= diameter van grote pulley: $\frac{54\cdot2.5}{\pi}=42.97mm$ 
- $d_k$= diameter van kleine pulley:$\frac{16\cdot2.5}{\pi}=12.7\operatorname{mm}$
### motor mountplate (en spanner)
Om te zorgen dat de riem goed opgespannen kan worden laat ik de gaten voor de bouten onderaan een stukje groter (4.6mm voor M4 bout). Zo kunnen de bouten schuin beginnen in de gaten. Wanneer het plaatje zichzelf recht trekt door de bouten aan te draaien komt de band ook onder spanning. De asafstand moet wel verhoogd worden met de extra ruimte die de radius van de gaten hebben (.3mm) voor een totaal van 46.53mm

uiteindelijk ziet het geheel er als volgt uit:![[Pasted image 20260116141119.png]]
De extra plaat aan de voorkant is verantwoordelijk voor het vasthouden van de pulleys
# kosten
onderdelen:
- [[swingtool.pdf|swingtool]] #kosten
- [[- definitie afbramer#swingtool monteren|swingtool mountplate]]  #materiaal
- [[- definitie afbramer#karretje|kar]] #hepco_motion
- [[- definitie afbramer#rail|rail]] #hepco_motion
- [[- definitie afbramer#mountplate|rail mountplate]] #materiaal
- [[- definitie afbramer#mountplate|mountplate alu profiel]] #rose_kruger
- [[- definitie afbramer#verbinding naar actuator|moutplate-actuator adapter]] #materiaal
- [[- definitie afbramer#slijpschijf inbrengen|lineaire actuator]] #rose_kruger
- [[- definitie afbramer#spannen en asafstand|motor mountplate]] #materiaal
- [[- definitie afbramer#pulleys|pulleys]] #materiaal
- [[- definitie afbramer#riem|tandriem T2.5/182.5 SFX]] #tyma
   6.45 euro
- [[- definitie afbramer#motor(verbinding)|stappenmotor]] #nanotec
  70,70 euro
  [Product Configurator \| Nanotec](https://www.nanotec.com/eu/en/products/product-configurator/483::114_483:1056/)

#  oud en ongebruikt
De enige variable waarop er aanpassingen gemaakt moet worden is de pitch van de pelrollen. De mogelijke spoedhoeken zijn te vinden in [[pelrol dimensionering]] en zijn als volgt: 66.16 rechtsom, 63.28 Rechtsom, 54.26 Rechtsom, 54.26 Linksom, 63.28 Linksom en 66.24 (rechtsom?) . 

Om de gaten op de juiste plek te krijgen word er opgemeten wat de afmetingen zijn tussen de monteer gaten en de punt van d. deze word vervolgens "gesimuleerd" in creo.
![[Pasted image 20251107153522.png]]
op deze manier kan voor elke hoek een gat op de juiste plek geplaatst worden door de hoek tussen de as en de x as te veranderen naar 90-spoedhoek, kun je elk benodigd gat krijgen. Met alle benodigde hoeken ontstaat de volgende plaat:
**deze hoeken moeten nog gecontroleerd worden** 
![[Pasted image 20251107161102.png]]

### ruimte maken
waneer dit gedaan is ontstaat de volgende situatue:
![[Pasted image 20251111140934.png]]
Het rode gebied komt tegen de geleiding rails aan, en het gele gedeelte komt tegen het klem center blok aan.
om te voorkomen dat er problemen ontstaan in het gele gebied moet de lang genoeg zijn dat het gehele klem center blok uit de weg beweegt.

om te zorgen dat het rode gebied geen probleem word moet de gehele gedraaid worden zodat deze geen contact meer zal maken met het geleidingsysteem. Om hier zo veel mogelijk ruimte te creeeren word de mountplate zo gedraaid dat de binnenste hoeken op hetzelfde globale vlak staan, in dit geval is dat een hoek van 6.55 graden![[Pasted image 20251111141826.png]]![[Pasted image 20251111141952.png]]
om er voor te zorgen dat de schijf alsnog in dezelfde hoek zal staan moet de  een hoekafwijking hebben van 6.55 graden in de gaten @

