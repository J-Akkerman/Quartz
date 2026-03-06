# concept analyse
in [[pelrol positioneren concept]] is er onder "pelrol axiaal verplaatsen" gekozen voor een mechanisme waarbij een van de centers (waar de pelrol tussen gespannen zal worden) losgekopeld kan worden van de spindel.
Door deze actie kan dit center vrij bewegen van de spindel waar het andere center nog op vast zit. Hierdoor kun je de afstand tussen de twee centers wijzigen om pelrollen te plaatsen, verwijderen en verschillende lengtes op te vangen.
Dit mechanisme moet buiten los en vast koppelen van het draad ook de centers naar elkaar toe kunnen klemmen. Dit betekend dat je met een hendel-effect de lengte tussen de centers moet kunnen aanpassen wanneer beide centers op de spindel zitten. zie hieronder een schets:
![[spindel grijp concept|spindel grijp concept]]
om dit te realiseren zijn er een aantal [[schetsen axiale verplaatsing|schetsen]] gemaakt die op deze pagina verder uitgewerkt zullen worden.
## positioneren
Om het gehele klem center blok te positioneren moet deze voor en achteruit bewogen kunnen worden wanneer de hendel omhoog staat. Wanneer de hendel omhoog wordt bewogen moet deze zo vastgehouden worden zodat deze niet meer kan draaien, zo kan het gehele blok bewogen worden door aan de hendel te trekken.
## contact maken met spindel
om de moer van en op de spindel te tillen kan de hendel waarmee deze ook wordt geklemd omhoog getild worden.
## klemmen
het klemmen van dit systeem zal gedaan worden met een profiel wat door de hendel gedraaid wordt en hierdoor de moer naar achter duwt. Denk aan een enkele tand van een tandwiel.
![[klem profiel mechanisme]]
## vasthouden
~~het klem profiel die voor het klemmen gebruikt wordt kan ook het systeem geklemd houden, wanneer deze verder draait als de max zal deze automatisch verder geduwd worden.~~
![[klem profiel mechanisme]]
Er is uiteindelijk gebleken dat de kracht waarmee het profiel vastgehouden zou worden te klein zou zijn om het mechanisme veilig vast te houden. Dit vast houden zou nu met een strakkere passing gedaan worden in het draaiende gedeelte van de hendel.
# klem profiel
![[klem profiel]]
# klem moer
![[klem moer]]
# hendel
![[hendel]]
%% # oud 
## ~~hendel definitie~~
**OUD**
er zijn 3 contactpunten met de hendel:
- De spanplaat
- Het moer scharnier
- Het center scharnier
De hendel zal er als volgt uitzien (totaal niet op schaal)
![[hendel kennismaking]]

er zijn 3 aangrijppunten op de hendel
1. De spanplaat
2. Moer scharnier
3. center scharnier
de positie van deze aangrijppunten hebben invloed op de volgende dingen:
- kracht geleverd op de moer ($F_{moer}=F_{hand}*(1-3)/(1-2)$)
  hoe **langer** de afstand tussen 1 en 3 hoe sterker de kracht
  hoe **korter** de afstand tussen 2 en 3 hoe sterker de kracht
- hoeveelheid verplaatsing van 2 ($s_{moer}=s_{hand}/(1-3)*(1-2)$)
  hoe **langer** de afstand tussen 1 en 3 hoe korter de radiale verplaatsing
  hoe **korter** de afstand tussen 2 en 3 hoe korter de radiale verplaatsing
- axiale afwijking (in relatie tot hendel) van de moer
  hoe **langer** de afstand tussen 2 en 3, hoe minder axiale afwijking 
- hoeveelheid materiaal gebruikt in [[- definitie klem center blok]]
  hoe **korter** de afstand tussen 2 en 3, hoe minder materiaal nodig is
- gemak van installatie (minimaal 30mm nodig)
  hoe **langer** de afstand tussen 2 en 3, hoe meer ruimte voor de moer

de gewenste slag van de moer is uiteindelijk \#klemkracht 2.2-5.5 mm en om een comfortabele hand beweging te krijgen wil ik deze beweging vergroten naar ongeveer 200mm. dit betekend dat de afstand van 1-2 90-36.36x langer met zijn als de afstand tussen 2-3. Deze verhouding kan aangepast worden door andere "hefboom" mechanismes in het systeem te verwerken.
### 
Het gaat hier niet perse om een hefboom mechanisme, meer een mechanisme om de slag van de hendel te vergroten. 

Er zijn een paar concepten om dit te realiseren:[[hefboom concepten]]
Uit deze concepten is er gekozen uit het "moer wegduwen met hendel profiel" concept. Dit concept lijkt et meest compact te kunnen zijn en simpel te zijn

Wanneer dit systeem in de huidige situatie word geplaatst kan het er als volgt uit komen te zien
![[hefboom vormgeving]]
~~De lengte van stuk 1-2 is op het moment 139-145 mm lang ik zit liever aan de kortere kant wat betekend dat het onderste hefboomprofiel tussen de 1.544mm en de 3.822mm van het centerpunt van de verticale hendel. Waarschijnlijk is dit te klein om een goede stijfheid te realizeren~~ 
**gaat over lengte 1-3**

## ~~moer verbinding~~
**OUD**
De moer moet aan de hendel gemonteerd worden om verticaal omhoog geplaatst te worden. Deze verbinding met de hendel moet echter niet beïnvloed worden door de bewegingen die deze maakt tijdens de klem actie. 

Dit kan gedaan worden door een pin door de hendel heen plaatsen wat zo los zit dat deze alleen naar beneden gedrukt word. De opties voor deze functie worden bekeken in [[bovenste moer scharnier concept]] hier word uiteindelijk gekozen voor het profiel onder de hendel met aparte scharnier punten:![[Pasted image 20251215132424.png]]

### axiale afwijking van moer
mijn volgende grootste zorg is de axiale afwijking van de vork, als deze te erg is kan het mogelijk enorm klemmen op de spindel. om dit te voorkomen moet het \#spindelgat ingesteld worden dat als de hendel in rust ingeschakeld is, deze geen afwijking heeft axiaal op de hendel.
de axiale afwijking kan op de volgende manieren worden beïnvloed:
![[axiale afwijking analyse]]
de axiale afwijking is ook te berekenen met:
$$g=r-\sqrt{r^2-\left(\frac12s\right)^2}$$
waarin:
- g= axiale afwijking in vork
- r= de afstand 2-3
- s= de slag die de moer moet maken
de minimale lengte tussen 2 en 3 is dus afhankelijk van de **gewilde slag** en de **maximale axiale afwijking**.

de gewilde slag word 5mm, wat de volgende formule ontwikkeld:
![[Pasted image 20251027113713.png]]
er is heir te zien dat het verlengen van lengte r een steeds lager rendement levert, dit is ook te zien in de afgeleide formule:$1-\frac{(2x)}{\sqrt{(-25+4x^{2})}}$ 
![[Pasted image 20251027114115.png]]
na ongeveer 10mm word de verbetering zo klein dat het eigenlijk amper relevant is,
#### gewenste slag
vanuit de werkplaats word er gezegd dat het center ongeveer 6mm diep in het werkstuk komt te zitten. als ik dan een 5 mm slag pak is de pelrol waarschijnlijk makkelijker te positioneren wanneer in gebruik. (het center zal de pelrol centereren)
### achterste hendel_scharnier
~~dit moet een 16mm kogelscharnier worden om alle assen te kunnen draaien ik wil het ook een male hebben voor makkelijke montage: 400019228~~
hetzelfde mechanisme word gebruikt als # spindel_contact_bovenste_moer met een gegenereerde bout

### spindel contact
#### onderste moer gedeelte
de moer is gekozen in [[spindel en aanhang]. 3993196 ziet er als volgt uit: 
![[Pasted image 20251020124709.png]]
met deze aansluiting kan de hoogte van dit blok ingesteld worden door de moer op en af te draaien vanuit het bovenste gat. hieronder is hiervan een schets te zien.
er zal een klem moer nodig zijn om te zorgen dat de spindel moer niet los komt tijdens gebruik.
![[moer bevestiging]]
verder zal er ook nog een moer nodig zijn om de spindel moer vast te klemmen, dit moet een zo laag mogelijke moer zijn die geschikt is om te klemmen. Dus:
- M14 draad
- ~~locknut~~ bestaat niet ~~==misschien wel 090100657 gebruikt kan worden in "bovenste moer gedeelte"== ~~
  
  
  
- ~~dunner als 10 mm~~ is niet meer nodig in de vernieuwde versie
~~dit word dan automatisch 6393550. een 4.8 mm dikke M14 moer. ~~

~~omdat dit geen lock nut is wil ik graag een ringete tussen de twee moeren om een goede connectie te garanderen. de keuze is dan tussen een nut type of een tooth type. de tooth is bekender, dus die word gekozen. de enige optie is dan 3338116, deze staat op het moment op rood, maar is ook makkelijk bij te bestellen. of er moet gekozen worden om een M14 lock nut van dunner als 10 mm bij te kopen. maar daar ga ik nu niet verder op in.~~

#### bovenste moer gedeelte
De bovenkant van dit mechanisme moet ook nog aan de hendel verbonden worden. als diet gedaan word met een vaste verbinding moet er rekening gehouden dat de moer ook mee zal draaien wanneer de hendel draait. Deze afwijking is zo groot dat de moer door de spindel heen zou moeten om los te komen. Er moet dus ergens in de verbinding aan de moer een scharnierpunt komen. het liefste bopvenaan. dit scharnier moet vrije rotatie hebben over de x as en de y as.

hieronder zijn 2 situaties gesimuleerd waarbij de bovenste verbinding een scharnierpunt is.
- hendel onder
  ![[Screenshot 2025-10-20 150705.png]]
- hendel boven
  ![[Pasted image 20251020151038.png]]
in de 2e situatie zit de moer 0.87 mm in de muur. Dit is zo een klein verschil dat de geleider gat voor de moer vergroot kan worden om dit te laten passen. Dit heeft effect op het moer geleiding gat in het [[klem center blok]. word ook enorm beïnvloed door [[spindel grijp mechanisme|spanplaat].

#### clevis fork

eisen:
- Het gehele mechanisme moet de structurele stijfheid van de hendel niet benadelen (dus geen gat door de hendel heen)
- de hendel moet minimaal 16 mm zijn, en de fork moet hier dus omheen passen
- de aangrijppunten van de fork moeten op de zijkanten van de hendel zijn om momenten effectiever tegen te werken
- de fork moet zo stijf mogelijk zijn
- de as (of schroef) die onder uit de fork komt moet vrij te draaien zijn 
(**het draaien van de stang moet nog gelimiteerd worden**) 
gewilde mecahnisme:
![[moer scharnier concept]]
maar hoe ga je dit monteren, als de de assn vastlast krijg je de vork er niet meer overheen... en de vork wil je het liefste zo dicht mogelijk op de hendel hebben, dus dit achteraf lassen word ook moeilijk.

je kan de vork zelf lassen... of zou je deze ook anders kunnen verbinden? denk dat lassen het veel makkelijker maakt.
Waar kan de las het beste gelegd worden? Ik wil goed weg blijven van de schroef, dus aan de buitenkant van de vork? en dan 3 aparte platen. want dat is lekker simpel. 
Ik zie ook geen nadeel in dikke platen gebruiken, dus ik ga waaarschijnlijk kiezen voor de 5mm.**is 5mm handig of mis ik dingen?**
eene Y las zou ideaal zijn, maar kun je deze platen daar goed op voorbereiden? vlakke las zou volgens rob ster zat zijn, maar ik wil voor de zerkheid hoeklassen gaan gebruiken, hiervoor zou de onderste plaat groter moeten zijn. zo kun je ook de maten mooi afronden

welke pinnen zullen er gebruikt worden? Ik wil de pin goed dik hebben vanwegen het onvoorspelbare moment wat er gaat spelen. 7-8 mm lang lijkt ideaal ivm. de plaatdikte die ik wil gebruiken
![[Pasted image 20251024101239.png]]
![[Pasted image 20251024101336.png]]
647075 lijkt de beste optie te zijn

er word een stukje van de as afgevlakt zodat deze cilinders goed vastgelast kunnen worden
![[Pasted image 20251024102019.png]]

en dan moet er nog een schroef in komen, 
- de onderkant moet M14 zijn ivm de gekozen [[spindel en aanhang|moer]]. 
- verder moet de kop tussen de platen passen (16.2 mm gebaseerd op een moer die later gekozen word) ~~terwijl deze nogsteeds vrij kan draaien~~
- de bovenkant word M8 schroefdraaad 
- de lengte is nog niet vastgesteld
M14 bouten lijken zeer schaars te zijn binnenn Marel, dus ik maak wel mijn eigen asje.

als ik toch een eigen asje ga maken kies ik ervoor om het bovenste gat kleiner te maken. zo heb ik meer mogelijk conact oppervlak met de plaat. het word een 8 mm gat zodat er meer contact oppervlak is met de plaat(en moer). (er word een moer gebruikt omdat anders de as niet past). deze moet vrij ge grootste locknut die vrij kan draaien is (**000163350**) een 8 mm hooge M8 bout en op zijn breedste punt 15mm

#### kogel scharnier
**concept gaat ten onder door het moer moment**

==met het herontwerp van het [[klem center blok], kan er waarschijnlijk beter gebruik worden gemaakt van een M14 kogelscharnier die rehtstreeks in de moer gemondteerd word== maar kan ik 090100657 gebruiken hiervoor? hij is namelijk rood maar wel beschikbaar **KAN BEST, vraag petrick van aar**
##### pre-herdefinitie van klem center blok
om deze scharnier te realiseren word er gebruik gemaakt van een kogel scharnier. hiervoor zijn 3 opties die de juiste interne diameter hebben
![[Pasted image 20251020155943.png]]
de mannelijke versies zijn niet lang genoeg zijn om in de moer te schroeven zoals besproken in "onderste moer gedeelte". hierom zal er een extra tussenstuk moeten komen. 
~~om dit ontwerp zo makkelijk mogelijk te houden is het gewenst dat de draad zo kort mogelijk is*. alle opties blijken even lang te zijn.~~
090100651 lijkt te passen op de hendel en het meeste ruime over te houden tot de moer, omdat deze vrouwelijks getapt is. 

het concept zal er als volgt uit zien
![[moer hendel connect]]
met deze instructies is het volgende ontwerp gerealiseerd. dit heeft echter ook nog problemen.
![[Pasted image 20251021092504.png]]
##### moer moement
![[moer moment]]
de kracht van de hendel (groen) creëert samen met de kracht van de spindel (oranje) een moment (rood). Op het moment word dit moment alleen tegengewerkt door de normaalkracht tussen de moer en het frame. Omdat ik verwacht dat krachten groen en oranje groot zullen worden, en deze een veel grotere arm hebben als blauw moet hier iets aan gedaan worden.

- draaiing in balschijf limiteren
  Hoe wil je dat doen zonder de andere vrijheidsassen tegen te werken?
  De hendel draait zelf ook nog, maar achterste scharnier is ook limiteerbaar
- **extra ondersteunend onderdeel vanaf de stang**
  bevestingen met klem? 
  De hendel draait zelf ook nog, maar achterste scharnier is ook limiteerbaar
- de blauwe pijl sterker maken
  slijtvrije ondergrond en langere arm 
- positie van de spindel aanpassen 
  hoe hoger de spindel zit hoe kleiner de armen van oranje en groen zijn.
  zo ontstaat er wel een extra moment in de geleiding...
  hiervoor zou ik een kogel lager moeten hebben met een M14 mannelijk schroefraad, OF het schroefdraad bovenin de moer kunnen aanpassen op de gewilde mannelijke schroefdraad van de kogel scharnier. 

==na wat schetsen in [[rotatie limitatie]] is er uiteindelijk gekozen voor het volgende concept:==
==![[Pasted image 20251021111849.png]]==
==dit systeem zal op beide het moer scharnier als de hendelscharnier geplaatst moeten worden.==

==het materiaal word uiteraard uit PLM gehaald, hiervoor word 400016323 gebruikt, dit is de dikste buis met de juist interne diameter.==

==eigenlijk is langs de hendel niet de juiste as om te blokken, je moet altijd haaks op de spindel het moment tegen houden...==

### hendel aagnrijppunten
er zijn 3 aangrijppunten op de hendel
1. de spanplaat
2. spindel contact vork
3. achterste kogelscharnier
de positie van deze aangrijppunten hebben invloed op de volgende dingen:
- kracht geleverd op de spindel ($F_{spindel}=F_{hand}*(1-3)/(1-2)$)
  hoe **langer** de afstand tussen 1 en 3 hoe sterker de kracht
  hoe **korter** de afstand tussen 2 en 3 hoe sterker de kracht
- hoeveelheid verplaatsing van 2 ($s_{spindel}=s_{hand}/(1-3)*(1-2)$)
  hoe **langer** de afstand tussen 1 en 3 hoe korter de radiale verplaatsing
  hoe **korter** de afstand tussen 2 en 3 hoe korter de radiale verplaatsing
- axiale afwijking van de vork (minimaal 10 mm nodig)
  hoe **langer** de afstand tussen 2 en 3, hoe minder axiale verplaatsing 
- hoeveelheid materiaal gebruikt in klem blok
  hoe **korter** de afstand tussen 2 en 3, hoe minder materiaal nodig is
- gemak van installatie (minimaal 30mm nodig)
  hoe **langer** de afstand tussen 2 en 3, hoe makkelijker de moer in het moergat geplaatst word 
- dimensies van de klemplaat 

de gewenste slag van de moer is uiteindelijk 5 mm en om een comfortabele heldenbeweging te krijgen wil je deze bewegin vergroten naar ongeveer 250mm... FUCK alles is veel te klein.

==het kogelscharnier gaat zo dicht mogelijk tegen de moer aanmoeten om een realistische hendelslag te realizeren== [[klem center blok]
#### gemak van instalatie
de eerste 4 van deze effecten zijn constant variabel. De gemak van installatie heeft een minimum wat deze nodig heeft om het geheel überhaupt te assembleren. dit word verder besproken in het "**hendel montage**" hoofdstuk 
lengte 2-3 moet voor de montage lang genoeg zijn om een moer op de kogelscharnier te plaatsen, dit vereist een lengte van ongeveer 30mm
#### axiale afwijking van vork
mijn volgende grootste zorg is de axiale afwijking van de vork, als deze te erg is kan het mogelijk enorm klemmen op de spindel. om dit te voorkomen moet het \#spindelgat ingesteld worden dat als de hendel in rust ingeschakeld is, deze geen afwijking heeft axiaal op de hendel.
de axiale afwijking kan op de volgende manieren worden beïnvloed:
![[axiale afwijking analyse]]
de axiale afwijking is ook te berekenen met:
$$g=r-\sqrt{r^2-\left(\frac12s\right)^2}$$
waarin:
- g= axiale afwijking in vork
- r= de afstand 2-3
- s= de slag die de moer moet maken
de minimale lengte tussen 2 en 3 is dus afhankelijk van de **gewilde slag** en de **maximale axiale afwijking**.

de gewilde slag word 5mm, wat de volgende formule ontwikkeld:
![[Pasted image 20251027113713.png]]
er is heir te zien dat het verlengen van lengte r een steeds lager rendement levert, dit is ook te zien in de afgeleide formule:$1-\frac{(2x)}{\sqrt{(-25+4x^{2})}}$ 
![[Pasted image 20251027114115.png]]
na ongeveer 10mm word de verbetering zo klein dat het eigenlijk amper relevant is,
#### gewenste slag
vanuit de werkplaats word er gezegd dat het center ongeveer 6mm diep in het werkstuk komt te zitten. als ik dan een 5 mm slag pak is de pelrol waarschijnlijk makkelijker te positioneren wanneer in gebruik. (het center zal de pelrol centereren)
### hendel montage
de hendel moet goed gemonteerd worden, maar er zijn hier een paar restricties:
- het kogellager word geschroefd gemonteerd(kan ook andere oplossing voor komen)
- het kogellager kan maar een bepaalde hoeveelheid draaien
- de moer zal axiaal variëren van locatie wanneer de hendel omhoog staat
![[Pasted image 20251027100730.png]]
#### lager anders monteren
het lager hoeft niet perse in het blok geschroeft te worden, het kan ook onderaan worden vastgehouden met een moer. 
- Dit verminderd het gewicht van het blok
- maakt montage gegarandeerd makkelijker
- minder moeilijke variabelen
![[Pasted image 20251027101536.png]]
[[klem center blok] moet er rekening mee houden dat er hier een moer moet passen



de diameter word bepaald op basis van het kogel scharnier wat in de [[klem center blok] gemonteerd is. En is grotendeels gedementioneerd op goed gevoel.
### gemak van instalatie
de eerste 4 van deze effecten zijn constant variabel. De gemak van installatie heeft een minimum wat deze nodig heeft om het geheel überhaupt te assembleren. dit word verder besproken in het "**hendel montage**" hoofdstuk 
lengte 2-3 moet voor de montage lang genoeg zijn om een moer op de kogelscharnier te plaatsen, dit vereist een lengte van ongeveer 30mm