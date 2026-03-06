---
prod/koop:
  - koop onderdeel
leverancier: Trapeziumdraad.NL
waar te vinden: https://www.trapeziumdraad.nl/product/trapeziumdraad-spindel-rvs-tr12x2/
identificatie: SPR 12x2
kosten/eenheid: 25.75
hoeveelheid: 1
---
De spindel zal zorgen dat de pelrol axiaal verplaatst zal worden. De eisen van deze spindel zijn asl volgt:
- moet de [[- definitie klem center blok#klemkracht|klemkracht]] op de pelrol aan kunnen
- Moet Tr draad hebben
- (wens) spoed moet zorgen dat de [[spindel en aanhang#spindel_motor|spindel motor]] het juiste toerental draait.
Ik wilde mezelf graag limiteren binnen de opties vanuit PLM, deze zijn echter allemaal te dik met een te grote pitch.

In dit systeem zal er slijtage plaatsvinden, deze slijtage zal in de spindel zitten of in beide moeren. Het vervangen van beide moeren is waarschijnlijk duurder is als het vervangen van de spindel. Daarom wil ik zorgen dat het materiaal van de spindel slijt, hierdoor zal het materiaal van de moeren bespaard worden. 
Er moet wel rekening gehouden worden dat de spindel verwijderd moet kunnen worden. #frame

Er is voor nu gekozen voor een [Trapeziumdraad spindel RVS TR12x2](https://www.trapeziumdraad.nl/product/trapeziumdraad-spindel-rvs-tr12x2/). 

De diameter is gekozen omdat de standaard spindel maten een diameter van 14mm overslaat, en ik het idee heb dat 16 mm een te dik draad zal zijn.
De spoed (2mm) is semi standaard. ik heb deze gekozen over de 3 mm omdat een kleinere spoed waarschijnlijk prettig is voor de spindel motor en het spindel grijp mechanisme.

## berekeningen
De spindel zal enkel de [[rubberen tip#klemkracht|klemkracht]] klemkracht moeten opvangen. De interne stress van een onderdeel kan als volgt berekend worden.

$$\sigma=\frac{F}{A}$$
$$\frac{463}{46.7}=9.9Mpa$$
waarin:
- F= de [[rubberen tip#klemkracht|klemkracht]] 463N
- A= De kerndoorsnede van de spindel: 46.7mm^2

9.9 Mpa is ver onder de vloeigrens, de spindel zal dus geen enkel probleem hebben met deze krachten opvangen

