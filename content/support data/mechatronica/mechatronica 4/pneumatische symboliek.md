**Pneumatische symboliek** is een gestandaardiseerde manier om componenten en functies in [[pneumatiek|pneumatische]] schema's grafisch weer te geven. Deze symbolen maken het mogelijk om systemen eenvoudig te analyseren, ontwerpen en begrijpen zonder de fysieke onderdelen te zien.
## Doel
- Eenduidige communicatie tussen ontwerpers, technici en monteurs
- Snelle interpretatie van functies en verbindingen
- Standaardisatie volgens normen zoals ISO 1219
## symboliek
- Symbolen geven **functie**, niet vorm of afmetingen weer  
- Pijlen geven **stroomrichting** van lucht aan  
- Vierkanten worden gebruikt om **ventielstanden** weer te geven  
- Elke lijn stelt een **verbinding of leiding** voor
### Ventielen

**Ventielsymbolen worden getekend als meerdere vierkanten naast elkaar**, waarbij:
- Pijlen de stroomrichting aangeven  
- Blokken de ventielstanden tonen  
- bediening (zoals drukknoppen, spoelen of veerretour) aan de zijkanten worden getekend
De benaming van een ventiel word geschreven als (hoeveelheid aansluitingen)/(hoeveelheid standen). een ventiel met 3 aansluitingen en 2 standen is dus een 3/2 ventiel.

Hieronder staan een paar voorbeelden van symbolen
![[Pasted image 20250609155510.png|400]]
#### 3/2-wegventiel
- 3 poorten, 2 standen  
- Wordt vaak gebruikt voor het sturen van enkelwerkende cilinders
#### 5/2-wegventiel
- 5 poorten, 2 standen  
- Toegepast bij dubbelwerkende cilinders
### bediening
bedieningen bepalen de standen van ventielen, samen met de ventielen kan hiermee complexe logica opgebouwd worden. hieronder zie je een paar voorbeelden van bediening. 
![[Pasted image 20250609160056.png|500]]
#### veer
De veer zal een ventiel altijd van zich weg duwen, behalve als de andere kant geactiveerd word. Dit zorgt ervoor dat het ventiel dus [[mono-stabiel]] is
#### lucht
wanneer er lucht vanaf de zijkant in het ventiel word geperst word het ventiel weg geduwd.
### actuatoren
![[Pasted image 20250615133054.png|400]]
bekijk [[cilinder]] voor verduidelijking van onderdelen
### logica
![[Pasted image 20250610135159.png]]
### overig
![[Pasted image 20250610133308.png|500]]
#### terugslagklep (met veer)
![[Pasted image 20250610134914.png|200]]
Laat het gas maar een kant op lopen. wanneer het symbool zoals hierboven geplaatst is zal het gas alleen naar links toe kunnen vloeien. de eventuele veer zal er voor zorgen dat de klep beter dicht blijft. (tegen zwaartekracht werkend bijv.) 
#### geluidsdemper
![[Pasted image 20250610134938.png|200]]
werkt als een outlet voor de lucht, dempt het lawaai wat hierbij kan ontstaan.
#### compressor
![[Pasted image 20250610135110.png|200]]
Er zijn 3 opties voor het tekenen van [[lucht compressor|compressors]], ze kunnen allemaal worden toegepast.
De rechter twee zijn ook inclusief [[luchtverzorging]].

## Inbouwvoorbeeld
### Of systeem
in het onderstaande voorbeeld is een systeem te zien waarin de zuigerstang van de [[cilinder]] alleen naar buiten gaat wanneer er een van de twee knoppen geactiveerd word.(bekijk [[pneumatische symboliek]])
![[Pasted image 20250615183137.png|700]]
### En systeem
in het onderstaande voorbeeld is een systeem te zien waarin de zuigerstang van de [[cilinder]] alleen naar buiten gaat wanneer beide knoppen geactiveerd worden.(bekijk [[pneumatische symboliek]])
![[Pasted image 20250615183638.png]]
### oefening 2
- in rust bevindt de cilinder zich in.
- Wanneer ventiel A wordt bediend (en direct wordt losgelaten) of ventiel B wordt bediend loopt de cilinder uit. 
- De uitgaande cilinderslag bediend ventiel C.
- Wanneer ventiel C wordt bediend zal de cilinder inlopen.
- De uitgaande snelheid wordt gesmoord!![[Pasted image 20250615184049.png]]
  (er zou eigenlijk ook een [[Smoring]] op de linker kamer van de [[cilinder]] moeten zitten) 
### oefening 3
- Op een startsignaal beweegt cilinder A uit
- Als cilinder A uit is blijft deze uit EN gaan B en C ook uit
- Cilinder C gaat direct in nadat hij uit gegaan is (A en B blijven dan uit)
- Als cilinder C weer in is, gaan A en B ook weer in
- Het systeem bevind zich nu weer in de uitgangspositie (alle drie de cilinders IN)![[Pasted image 20250615184312.png]]