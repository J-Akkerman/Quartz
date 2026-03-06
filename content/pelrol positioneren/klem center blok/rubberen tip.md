---
prod/koop:
  - sub-part
identificatie: 8071218_02
---
in [[pelrol positioneren concept]] is er al gekeken naar mogelijke opties om te zorgen dat het center genoeg grip heeft met de pelrol.![[Pasted image 20251021134527.png]]
de opties die overwogen zijn zijn als volgt:
- hoge wrijving
  Met behulp van een rubberen "ring" rond de conus kan er een hoop wrijving ontstaan tussen het center en de pelrol.
- face driver
  Een face driver zet tanden in de face waar het vlak waar de center tegenaan word geklemd. word wel heel erg positie gevoelig.
- vertanden contour
  Er kan een vertanding in het center gefreesd worden, deze vertanding word dan in het centergat geperst. word wel positie gevoelig.
- draad over center plaatsen
  door draad over het center te plaatsen krijg je hetzelfde effect als vertanding contour, maar dan mogelijk wat simpeler
Er is gekozen voor hoge wrijving omdat dit minder locatie gevoelig is. Het huidige systeem is meer afgesteld op "hoeveelheid kracht" en niet op locatie. *Is achteraf mogelijk niet de beste keuze maar is destijds wel volledig uitgewerkt*
### grip materiaal
[[Rubber]] lijkt het meest voor de hand liggende materiaal te zijn. Ik heb contact opgenomen met [Van Willigen – Rubbertechniek](https://www.vw-rubber.nl/) om de opties te vergelijken en de beste optie voor deze applicatie te kiezen. 
Uit een telefoongesprek met Van Willigen werd aangeraden om een natuurrubber te gebruiken, deze kunnen de hoogste wrijving realizeren. Ook is de E modulus van deze rubber heel makkelijk aan te passen.
### klemkracht
De wrijving op het rubber is afhankelijk van het soort rubber en de kracht waarmee je de pelrol aanduwt. De aanduw kracht is in dit geval de variabele die aangepast kan worden. Hieronder is de formule te zien die gebruikt zal worden om

Het moment wat de pelrol moet overbrengen zal gelijk zijn aan het moment wat de kunststof borstel in de pelrol opwekt. De [[- definitie borstel#motor keuze|borstel motor]] heeft een kip koppel van 14.2 Nm. De radius van de kunststof borstel is op zijn kleinste (door slijtage) 0.09m wat betekend dat de pelrol word belast met 158 N. De dikste pelrol zal het grootste moment ervaren, dit is een 27mm pelrol $158*0.027=$**4.26Nm** wat de pelrol moet kunnen opvangen

![[Picture-1.png]]
[Natuurkunde.nl - Wrijving tussen twee draaiende schijven](https://www.natuurkunde.nl/vraagbaak/79361/wrijving-tussen-twee-draaiende-schijven)
de bovenstaande uitleg definieert $M=\frac23\cdot\mu\cdot F_{N}\cdot r_{gem}$ deze formule is vervolgens om te schrijven naar: $$\frac{M}{\frac23\mu\cdot r_{gem}}=F_{N}$$
$$\frac{4.26}{\frac23\cdot1.2\cdot11.5}=463N$$
waarin:
- M= het benodigde moment, hierboven gedefineerd als 4.26Nm
- $r_{gem}$= 11.5mm, de gemidelde radius van de ring ($\frac{\left(r_{uitwendig}+r_{inwendig}\right)}{2}$)
- $\mu$= 1.2 het [[wrijvingscoëfficiënt]] tussen de pelrol en het grip materiaal
De wrijvingscoëfficiënt is gebaseerd op de volgende sites:
[Wrijvingscoefficient](https://www.werktuigbouw.nl/abc/cof.htm) [Table of Friction Coefficient| Technology & Engineering](https://www.scribd.com/document/71374514/Table-of-Friction-Coefficient) [Wrijvingskracht berekenen - Uitleg, formules en wrijvingscoëfficiënten](https://roybosch.nl/wrijvingskracht-berekenen/) [ocw.tudelft.nl_Wrijving.pdf](https://ocw.tudelft.nl/wp-content/uploads/12._Wrijving.pdf) 
### rubber vervorming

> [!note] bereken assumpties
> deze berekeningen houden er geen rekening mee dat het rubber niet alleen vanaf de achterkant wordt geduwd maar ook vanuit het gedeelte wat rond het aangedreven center zin.
> Hierdoor zal de vervorming minder zijn als dat er wordt berekend

de [[vervorming]] van dit onderdeel kan berekend worden met een simpele formule:

$$\Delta L = \dfrac{F \cdot L}{A \cdot E}$$

waar: 
- $\Delta L$ = de vervorming
- $F$ = klemkracht 463N
- $L$ = originele lengte 
- $A$ = doorsnede-oppervlak 
- $E$ = [[elasticiteitsmodulus]] van het grip materiaal
ik wil uiteindelijk dat het onvervormde materiaal net achter de punt uitkomt:
$$L-\Delta L=7.8mm$$
waarin:
- $L$ = originele lengte 
- $\Delta L$ = de vervorming
- 7.8mm = de lengte die is uitgesneden uit de punt van het aandrijf center
deze 2 formules kunnen samengevoegd worden voor:
$$L=\frac{F\cdot7.8}{A\cdot E}+7.8$$
omdat de [[elasticiteitsmodulus]] niet goed bekend is word er gekozen om een schatting te maken met de minimum gevonden E modulus voor rubber wat niet extreem flexibel is (4Mpa) en het maximum E modulus (10Mpa)
$$\frac{463\cdot7.8}{162.577\cdot10}+7.8=10\operatorname{mm}$$
$$\frac{463\cdot7.8}{162.577\cdot4}+7.8=13.35\operatorname{mm}$$
Dit betekend dat het rubber in totaal tussen de 5.55 mm en de 2.2 mm zal vervormen. dit zal dus ook gelijk de slag zijn die de moer moet maken. Dit is ook hoe ver het rubber aan de voorkant van het center zal moeten uitsteken