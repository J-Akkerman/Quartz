---
prod/koop:
  - maak onderdeel
identificatie: "8071218"
kosten/eenheid:
hoeveelheid: 1
---
# aandrijf center
~~om te beginnen zal er eerst gekeken moeten worden naar het [[motor-center adapter]] het concept ziet er als volgt uit:
deze zal simpel ondersteund worden door een conus gat in het center blok. het lijkt handig om de standaard [[center|Morse-conus]] maten aan te houden. Het [[motor-center adapter]] is een MT 4 dus de buitenste conus word een [[center|MT5]] om een fatsoenlijke wanddikte te behouden~~.

~~zoals besproken in [[motor-center adapter]] onder ondersteuning zal~~ het aandrijf center zal ondersteund worden met een bushing: [SKF](https://www.skf.com/group/products/plain-bearings/bushings-thrust-washers-strips/bushings/productid-PCMF%20202321.5%20E). Deze bushing moet juist ondersteund worden en heeft de juiste passing nodig, maar voor de rest word dit een standaard gat.

Het aandrijf center zal twee grote functies moeten voldoen: De pelrol ondersteun en de pelrol aandrijven
## rubberen tip
![[rubberen tip]]
## aangedreven center
![[aandrijf center]]
# spindel grijp mechanisme
![[spindel grijp mechanisme]]

# geleiding
![[geleidingssysteem]]
# kosten
onderdelen:
- klem center assembly 8071218 #materiaal
  - moer 8071218_03 #materiaal 
  - 8071218_08
  - 8071218_05
  - 8071218_09
  - 8071218_11
  - 8071218_07
  - 8071218_10
  - 8071218_01
  - 8071218_02
- Hendel 8071446 #materiaal
  - 8071446_01
  - 8071446_02
- klem center frame 8066262 #materiaal 
  - 8066262_02
  - 8066262_03
  - 8066262_04
  - 8066262_05
  - 8066262_06
  - 8066262_07
- geleiding 3294361 3x #PLM 
  er zijn variërende prijzen
  31.42 p/s
  94.26
- stappen motor #nanotec 
  196,20 euro
- flange bushing #SKF
  4.57 euro
- Hendel Grip 090500145 #PLM 
  7.58 euro
  
# oud

> [!dit wordt niet meer gebruikt] Title
> Dit wordt niet meer gebruikt

## spanplaat verbinding
Deze wil ik vervangbaar hebben voor eventuele aanpassingen in spanning en positie van de hendel. simpel vast schroeven zal zat zijn.
Is het nodig om de positie vast te zetten met de vorm van de plaat of het [klem center blok]? neh, enige afwijking in de [[spindel grijp mechanisme|spanplaat]] zal 5.2x kleiner zijn op de schroef 

er moet nog een .4 afwijking van de moer af, (kijk moergat
## moer gat
moer geleiding moet .8 mm groter als de moer om te voldoen aan ruimteprobleme aangegeven in [[spindel grijp mechanisme]] (bovenste moer gedeelte). om de afwijking aan beide zijdes te minimalizeren zal het gat ook .4mm van de spanplaat af geschoven worden

Ook moet de positie en lengte van het gat nog aangepast worden, maar dat is iets voor later in het ontwerp 
## spindel geleider
[[spindel en aanhang]] het gat moet geschikt zijn voor een Tr24 spindel, dus 24.2mm lijkt goed.
de spindel moet ook op dezelfde horizontale lijn zitten als het center, zo voorkom je onnodige momenten

## verbinding geleidingssysteem
dit zijn standaard schroefgaten gekozen op basis van het gekozen [[geleidingssysteem]]. Het lijkt alsof deze onderop het blok geplaatst moeten worden

deze moeten plat gemonteerd worden zodat ze zichzelf kunnen richten wanneer ze geinstaleerd worden. het liefste ook zo ver mogelijk uit elkaar om moment effectief tegen te werken. ~~ik ga voor nu een plaat aanlassen en daar de geleiding op schroeven, dit kan zeer makkelijk uitweiken mocht dat nodig zijn~~

de borstels moeten nog fatsoenlijk bij de pelrol kunnen, dus moet de geleiding moet zo ver mogelijk naar boven toe staan. 

De geleidings blokken moeten niet gelimiteerd worden door enige wanden, deze moeten zichzelf kunnen uitlijnen wanneer ze gemonteerd worden.
## vorm geving
### hoe verbinden
~~het spindel en moer mechanisme (excl de spanplaat) moeten in hetzelfde blok terecht komen.~~ 
- ~~maar gaat het center gat ook in hetzelfde blok?~~
  ~~neh klinkt als een fabricage probleem, die wil ik zo veel mogelijk voorkomen~~
- ~~word het center gat aan de rest vast gelast?~~
  ~~lijkt de beste optie... maar hoe?~~
- ~~zou ik de spindel boven de center gat kunnen plaatsen?~~
  de spindel zal in de weg zitten van de pelrol

je kan dit berijken door:
- 2 onderdelen aan elkaar te verbinden met plaaten (links) 
  Mogelijk grote tollerantie opbouw
  zoizo maakbaar
  goeie conectie plekken voor andere onderdelen zoals [consideratie punten positioneren|geleiding],[spindel grijp mechanisme|spanplaat]
- de 2 onderdelen vormpassend maken (rechts)
  simpeler te lassen en minder tollerantie opbouw
  hoe zou het blok gefabriceerd worden?- Moet wel kunnen toch?
![[conus-spindelblok verbinding]]
ik ga kiezen voor de vormpassende optie
### welke positie
omdat de \#klemplaat een ongeveer 250 mm lange slag moet hebben word de gehele plaat net zo groot als het gehele systeem tot nu toe. om dit verder te realizeren moet het [[spindel grijp mechanisme]] een dtuk verder naar achter worden geplaatst. naast de motor. 
Ik wil hem precies in het midden hebben van de gehele constructie, dit maakt het afhankelijk van beide de \#pelrol_motor en de \#motor-centeraddapter
## achterste hendel scharnier
- Het gat in het bok moet een M8 draad strak kunnen vasthouden
- de afstand vanaf het moergat is 30mm, dit kan kleiner maar lijkt niet nodig te zijn. 
- \#hendel lijkt nu 330mm lang te worden in deze configuratie
## dimensies spindel blok
- breedte
  is afhankelijk van hoe het [[spindel grijp mechanisme]] past
- diepte
  is afhankelijk van hoe het [[spindel grijp mechanisme]] past
  hoe breeder het geheel hoe beter het geleiding systeem de kracht kan opvangen
- hoogte
  is afhankelijk van hoe diep de [[spindel grijp mechanisme|kogelscharnieren]] in het blok moeten
**Omdat de lengte van [[aandrijf center]] hevig is onderschat zal er een herontwerp moeten komen. De motor zal bijna volledig in het klem center blok opgenomen moeten worden**
~~het klem center blok zal nog steeds vormgelijk moeten zijn als de oude versie, maar deze keer moet de motor zo ver mogelijk naar voren worden geduwd.~~

~~werkt dit ivm de motor voor de kunststuf borstel?.... fuck~~~~
~~om mogelijk alsnog te kunnen passen zal de Pelrol motor naar achter gericht kunnen worden, dit betekend een rechte versnellingsbak. **bestaat niet binnen SEW~~**~~
op het moment van documentatie ziet het klem center blok er als volgt uit:

![[klem center blok herkenning]]
## motor verbinding
het zijn simpele gaten die zorgen dat de motor op zijn plek blijft deze zijn al overeenkomend met de gekozen [*[Pelrol motor]*]. verder zit er aan de andere kant van het center blok een groef zodat de motor perfect tegen het center blok aanpast
## center support
Deze zal een taper hebben zodat het [*[aandrijf center]*] hier goed op kan leunen, alle axiale krachten moeten hierin worden opgevangen zodat de motor niet verkeerd belast word. moet misschien een gladder materiaal zijn . 
## spanplaat verbinding
deze word op het moment verbonden met schroeven die ook gebruikt worden voor het geleiding systeem, het leidingsysteem moet mogelijk verplaatst gaan worden, dus deze gaten veranderen waarschijnlijk nog van positie.
## moer gat
moer geleiding moet .8 mm groter als de moer om te voldoen aan ruimteprobleme aangegeven in [*[spindel grijp mechanisme]*], bovenste moer gedeelte. om de afwijking aan beide zijdes te minimalizeren zal het gat ook .4mm van de spanplaat af geschoven worden

Ook moet de positie en lengte van het gat nog aangepast worden
## verbindingsgaten voor geleidingssysteem
dit zijn standaard schroefgaten gekozen op basis van het gekozen [[geleidingssysteem]]. moeten mogelijk nog verplaatst worden
## gewicht reductie
heb een beetje gekozen wat ik mooi vond zonder het moeilijker te produceren te maken
