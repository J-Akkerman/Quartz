Het aangedreven center zal 3 main functies moeten voldoen:
- Pelrol recht houden
  Wordt al gedaan als er gebruik wordt gemaakt van een center vorm.
- Aandrijving vanuit de motor opvangen
- Axiale belasting door geleiden naar het frame
- De rubberen tip aandrijven
### aandrijving van motor opvangen
Dit zal gedaan worden met simpele as-naaf verbinding de [[Pelrol motor]] heeft de optie om een spiebaan toe te voegen, ~~dit zal een goede verbinding garanderen. ~~

Een spiebaan wordt normaal gemaakt door deze te steken. Hiervoor moet je genoeg ruikte hebben in de buis, die is hier simpelweg niet beschikbaar.

Inplaats van een spiebaan in het center kan er wel een gat in zijkant getapt worden, hier kan een schroefje in vastgedraaid worden wat in de spiebaan van de [[pelrol motor]] terecht zal komen. Dit zal waarschijnlijk niet geweldig zijn voor de as van de motor, maar als deze wordt vervormt door deze schroef wordt de verbinding alleen maar sterker wanneer de schroef weer aangedraaid wordt.
![[Pasted image 20260128102157.png]]
### De rubberen tip aandrijven
De [[rubberen tip]] zal niet vast gemonteerd te hoeven worden, dezelfde kracht waar deze mee tegen de pelrol wrijving ontwikkeld ontwikkeld de zelfde wrijving aan deze zijde.
Wel moet het rubber ergens tegenaan kunnen rusten, als het rechtstreeks op een conus neer wordt gezet zal deze uit elkaar geduwd worden wanneer er enige kracht op komt te staan.
Een simpel platformpje voor het rubber zal al meer als zat moeten zijn om alles goed te ondersteunen, de binnenkant klemt ook tegen de (nu as) aan en wordt vanaf hier dus ook ondersteund. 
De diepte die nodig is voor deze cut in al bepaald in [[rubberen tip]], deze tip zal de lengte van de slag moeten uitsteken met de rest van de lengte op het center.
![[Pasted image 20260128101744.png]]
### Axiale belasting door geleiden
Wanner de pelrol geklemd zal zijn zal dit center een hele hoge axiale kracht moeten opvangen als deze direct op het frame gezel zou worden komt hier een hoop wrijving, dit moet zo veel mogelijk voorkomen worden. er zijn een aantal concepten om deze wrijving te verminderen.

- vet in [[center|MT passing]] 
- gladde materialen in [[center|MT passing]] 
- ondersteunen met lagers
- gladde flens bushing

*Waar is de documentatie heen voor alle uitgewerkte concepten?

Een gladde [[flens bushing]] lijkt de beste optie te zijn. Hiermee kan het aandrijf center lekker eenvoudig blijven, makeklijk te vervangen blijven, 
### overig
verder mag het center niet aan de voorkant uit het systeem kunnen vallen. Een simpele borg ring aan de achterkant van de center zou meer als zat moeten zijn.
## oud
### Frame verbinding
Dit center zal redelijk zwaar axiaal belast worden, deze kracht mag niet in de stappenmotor komen. Maar de rotatie van het center moet zo min mogelijk tegen gehouden worden. Dit kan op de volgende manieren:

- vet
  met vet kan het center vastgehouden worden in een conus of een simpele wand aan de achterkant van het center zonder dat dit heel veel wrijving en dus limitatie toe voegt. 
  Ik heb geen ervaring met het ontwerpen voor een vet mechanisme. 
  Rob vind dat dit best mogelijk is met een simpele smeernippel.
- lagers 
  worden snel duur
  zijn ook weer ingewikkeld om te installeren 
  zijn geen groot fan van vieze omgeving
  Kan allemaal rekening eme gehouden worden, maar hoeft niet.
- glad materiaal 
  zou hetzelfde kunnen werken als het vet,
  is goed toe te passen door een bushing aan te brengen

Een glad materiaal in de vorm van een bushing lijkt het meest simpel, vervangbaar en effectief.

omdat er een axiale en radiale kracht moet worden opgevangen moet er een vorm worden gebruikt die beide deze krachten aan kan, dit kan bijvoorbeeld een morseconus zijn, of een flange. een morseconus is moeilijk te produceren uit een glad materiaal dus zullen we voor een flange [[bushing]] gaan. nu is de volgende gekozen omdat deze mooi past [SKF](https://www.skf.com/group/products/plain-bearings/bushings-thrust-washers-strips/bushings/productid-PCMF%20202321.5%20E) had achteraf beter uit een onderdeel van PLM kunnen kiezen.
### borging
de adapter moet niet uit zijn ondersteunende gat kunnen vallen, dus er moet ook nog een manier zijn om dit onderdeel te borgen. Het lijkt simpel om dit te doen met een borgring![[Pasted image 20251022135457.png]]

de einddiameter van het center is nu ongveer 20 mm, de juiste snapring voor deze applicatie is:000370420
### grip verbinding
### motor verbinding

![[glijdende assen]]
Ik ga gebruik maken van de D as met een schroefje in de bovenkant om deze te zekeren deze schroef moet wel goed gezekerd worden 
### motor belasting
**Ik ga de assumtie maken dat de conus alle axialen krachten gaat opnemem**

De motor mag niet axiaal belast worden
omdat de pelrol met behulp van wrijving opgevangen moet worden zal er veel axiale kracht opgevangen moeten worden.
het makkelijkste is om het center niet axiaal te verbinden met de [[Pelrol motor]]. er zijn hier 2 opties voor motor assen
![[Pasted image 20251022133605.png]]
beide opties kunnen op ongeveer dezelfde manier verbonden worden met de center verbinding:[[spieverbinding|geleidingspie]] 
![[glijdende assen]]
op beide manieren zou ik niet weten of en hoe dit te produceren zal zijn 

D as kan, maar inplaats van een D profiel in de as moet er gebruik worden gemaakt van een **schroefje**, het D profiel zelf is niet te maken voor een fatsoenlijke prijs.
[[Pelrol motor]] zal zich moeten aanpassen op het soort as gekozen.

Ik heb net de perfecte schroefjes gevonden: spring plungers. 
de kleinste soort die in PLM te vinden zijn zijn M6. dit past nog goed op de as dus deze wil ik gebruiken. vervolgens de kortste optie met standaard draad: 091400653. **niet te hard aandraaien deze dingen**
(ik denk dat de as niet axiaal kan bewegen waneer deze aan het draaien is gelukkig veranderd de axiale belasting alleen wanneer het systeem stationair is)

het schroefje steekt nogal uit, weet niet in hoeverre dit een probleem is.
(het gat lijkt te groot maar de schroef laat allen kerndiameter zien)
![[Pasted image 20251024092716.png]]
moet wel goed bereikbaar zijn voor aandraaien 

de motor op een klein afstandje van de adapter gemonteerd moet worden zodat de as in en uit kan schuiven om  axiale belasting te voorkomen. [klem center blok]