**Pneumatiek** is een techniek waarbij perslucht (samengeperste lucht) wordt gebruikt om mechanische bewegingen of krachten op te wekken en te regelen. Het wordt veel toegepast in industriële automatisering en machinebouw.
## Basisprincipe
Pneumatische systemen maken gebruik van de eigenschappen van samendrukbare gassen, meestal lucht. De [[druk]] van de lucht wordt gebruikt om arbeid te verrichten via cilinders, motoren of ventielen. Om hieraan te rekenen word er gebruik gemaakt van de [[wet van pascal]].
## Belangrijke kenmerken
- **Medium**: Lucht (vaak gefilterd en soms geolied)
- **Werkdruk**: Typisch tot max 10 bar (300 bar kan worden gebruikt in bijv. scuba flessen). Als er meer kracht nodig is moet je [[hydrauliek]] gebruiken.
- **Snelheid**: Hoge reactiesnelheid
- **Veiligheid**: Minder explosiegevaar en brandgevaar dan [[hydrauliek]]
- **Compressibiliteit**: Lucht is samendrukbaar. Dit betekend dat het gas eerst een beetje als een kussen reageert wanner deze word samengedrukt. 
- al het lucht wat gebruikt word moet voorbereid worden 
## Componenten
Een pneumatisch systeem bestaat meestal uit:
- [[lucht compressor]]: Levert samengeperste lucht
- **Luchttank**: Buffertank om druk te stabiliseren
- [[luchtverzorging]]: maakt de lucht geschikt voor gebruik
- [[Ventielen]]: Regelen de richting en hoeveelheid luchtstroom
- [[actuator]]: Zet luchtdruk om in beweging
- **Slangen en** [[koppeling|koppelingen]]: Voor transport van lucht, er word meestal gebruik gemaakt van twee soorten leidingen
  **Starre** (harde) leidingen worden vooral gebruikt In grote fabriekshallen – zogenaamde ringleidingen
  **Flexibele** leidingen worden voornamelijk gebruikt in het laatste deel, naar een betreffende machine of installatie.
- **luchtuitlaat en [[dempers]]**: worden gebruikt om lucht weer terug de omgeving in te sturen.


Al deze onderdelen kunnen schematisch getekend worden [[pneumatische symboliek]]
## Vergelijking met [[hydrauliek]]

| Kenmerk       | Pneumatiek  | Hydrauliek       |
| ------------- | ----------- | ---------------- |
| Medium        | Lucht (gas) | Olie (vloeistof) |
| Compressibel  | Ja          | Nee              |
| Typische druk | 6–8 bar     | 100–300 bar      |
| Precisie      | Lager       | Hoger            |
| Kosten        | Lager       | Hoger            |
## pneumatische systeem
Met [[pneumatische symboliek]] is het heel gemakkelijk om een systeem te ontwerpen, natuurlijk moet er wel rekening gehouden worden met een paar dingen:
### besparen op perslucht
Perslucht is kostbaar het is dus beter om perslucht te besparen. dit kan op de volgende manieren:
- Gebruik enkelwerkende cilinders als de toepassing dit toelaat
- Verminder de kans op luchtlekkage
- Verlaag de werkdruk
- Verminder de wrijving
## rekenen aan pneumatiek
maak onderandere gebruik van de [[wet van pascal]]
### luchtverbruik en inhoud van een cilinder
![[Pasted image 20250616105434.png]]
Voor de uitgaande slag geldt: $V=\frac14\cdot\pi\cdot D^2\cdot s\cdot\left(p+1\right)$
Voor de ingaande slag geldt:$V=\frac14\cdot\pi\cdot\left(D^2-d^2\right)\cdot s\cdot\left(p+1\right)$
waarin:
- Pascal
  V = volume in m3 = kubieke meter
  D = boring in m
  d = diameter van de zuigerstang in m
  s = slag in m
  p = werkdruk in Pa
- Bar
  V = volume in dm3 = Liters
  D = boring in dm
  d = diameter van de zuigerstang in dm
  s = slag in dm
  p = werkdruk in Bar
wanneer de inhoud van de [[cilinder]] vermenigvuldigd word met hoeveel slagen die er worden voltooid in een hoeveelheid tijd voor een algemeen [[debiet]]/luchtverbruik
#### voorbeeld
Stel: we hebben een dubbelwerkende cilinder met een boring (zuigerdiameter) van 50 mm en een zuigerstang van 20 mm. de slag is 200 mm en de werkdruk is 6 bar. De cilinder beweegt 20x per minuut. Bereken het luchtverbruik voor die ene minuut.
![[Pasted image 20250616110129.png]]
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
## LET OP
- [[slipstick]]
  Bij lage druk hebben we te maken met verschil tussen statische en dynamische wrijving tussen de zuiger en de cilindermuur, wat voor een schokkerig bedrijf kan zorgen. dit kan voorkomen worden met een [[snelheidsregelventiel]].