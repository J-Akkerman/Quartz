---
prod/koop: koop onderdeel
leverancier: Nanotec
waar te vinden: "[ST5909S1008-A - Stepper motor](https://www.nanotec.com/eu/en/products/483-st5909s1008-a)"
identificatie: ST5909S1008-A
kosten/eenheid: 70.7
hoeveelheid: 2
---
## soort motor
De motor voor de spindel heeft een aantal eisen:
- moet (redelijk) goedkoop zijn
  servo motoren vallen dus automatisch af
- moet zijn eigen positie kunnen bijhouden
  Ik wil geen gebruik maken van externe sensoren om positie te beredeneren. (met uitzondering van een eventuele "home" sensor)
- moet de slee kunnen vervoeren met circa 1 m/s
  is zwaar afhankelijk van de gekozen [[spindel]], maar word waarschijnlijk een relatief laag toerental
Op basis van deze criteria is een [[stappenmotor]] de duidelijke keuze
## belasting
(de volgende berekeningen komen uit rolof/matek tabellenboek/formuleboek)
### axiale kracht op spindel
De motor moet goed in staat zijn om de pelrol stil te houden wanneer deze bewerkt word. In dit geval is het enige kracht wat het spindel draad (stationair) moet opvangen de kracht van de staalborstel motor. (deze berekeningen zijn gemaakt in een situatie waar de pelrol geen extra spanning op levert) 

De [[borstel motor]] heeft een kip koppel van 14.2Nm. Wanneer dit gedeeld wordt door de radius van de borstel(.1m) krijg je een axiale as belasting van **142N**. 
In het echt zal deze kracht nooit behaald worden sinds het volledige moment van de motor nooit bereikt zal worden.

benodigde moment: [[support data/onderdelen/spindel]]
$$T=F\cdot\frac{d_2}{2}\cdot\tan\left(\phi\pm\rho^{\prime}\right)$$
$$142\cdot0.0105\cdot\tan\left(3.46+0.4658\right)=0.102-0.07798Nm$$
waarin 
T = moment
F = kracht van de borstel = 142N
$d_2$ = de [[flankdiameter]] van de [[spindel]]  = 0.0105 m 
$\Phi$ = de [[spoedhoek]] van de [[spindel]] = $\tan^{-1}\left(\frac{P}{d_2\cdot\pi}\right)=\tan^{-1}\left(\frac{2}{10.5\cdot\pi}\right)=3.46$ 
$\rho^{\prime}$ = de schroefdraadwrijvingshoek van de [[pelrol positioneren/spindel|spindel]] en de [[klem moer]]
$$\rho^{\prime}=\frac{\mu_{g}}{\cos\left(\frac{\beta}{2}\right)}$$$$\frac{0.45}{\cos\left(\frac{30}{2}\right)}=0.4658$$
waarin: 
- $\mu_{g}$ = [[wrijvingscoëfficiënt]] in schroefdraad bij de bronze moer: 0.45
- $\beta$ = [[flank angle]] is voor trapeziumdraad altijd 30 graden
### wrijving van het spindeldraad
Er zal een hoop wrijving plaatsvinden tussen de moeren en de spindel. Om de pelrol te verplaatsen moet de motor deze wrijving kunnen overkomen.

$$T=F\cdot\frac{d_2}{2}\cdot\tan\left(\phi\pm\rho^{\prime}\right)$$
$$463\cdot\frac{0.0105}{2}\cdot\tan\left(3.46+0.4658\right)=0.1668Nm$$
waarin:
- F= de  [[rubberen tip#klemkracht|klemkracht]] van 463N 
- $d_2$ = de [[flankdiameter]] van de [[spindel]]  = 0.0105 m 
- $\Phi$ = de [[spoedhoek]] van de [[spindel]] = $\tan^{-1}\left(\frac{P}{d_2\cdot\pi}\right)=\tan^{-1}\left(\frac{2}{10.5\cdot\pi}\right)=3.46$ 
- $\rho^{\prime}$ = de schroefdraadwrijvingshoek tussen de [[spindel]] en de [[klem moer]]/[[meeloop moer]]. De voorheen berekende getallen kunnen hiervoor gebruikt worden. Dit kan omdat we voor beide moeren hetzelfde materiaal gebruiken en er verder geen factoren anders zijn als het hoofdstuk hierboven
## motor keuze 
[[pelrol motor]] maakt al gebruik van een [[stappenmotor]] van [Nanotec](https://en.nanotec.com/), deze stappenmotor zal ook vanuit Nanotec geselecteerd worden. de motor moet aan de volgende eisen voldoen:
- minimaal moment hebben van 0.2 Nm (graag meer richting 0.6)
- passen aan de (([[aandrijf center]])) zijde 
De volgende motoren zijn met elkaar vergeleken:
![[Nanotec_Compare-1.pdf]]
Omdat het wenselijk is om de motor zo langzaam mogelijk te kunnen draaien lijkt SCA5618X4204-A de beste optie te zijn. Wanneer deze echter in de assembly geplaatst word blijkt deze te breed te zijn. de volgende optie met het meeste bereik is de ST5909S1008-A of de ST5918X3008-A. Omdat het verschil in prijs maar 20 euro is kies ik voor de sterkere [ST5909S1008-A](https://www.nanotec.com/eu/en/products/483-st5909s1008-a) met een D as voor de extra betrouwbaarheid.
### stappenmotor driver
Omdat nanotec geen goede opties heeft voor drivers ga ik deze kiezen van [StepperOnline](https://www.stepperonline.nl/stappenmotor-driver-controller). De motors die gebruikt gaan worden Hebben een Current per Winding van 1A, de driver moet deze stroom comfortabel kunnen leveren op 24-48V. Met deze eisen blijven er 3 toepasbare opties over:
- [Closed Loop Stepper Driver 0-3.0A 24-48VDC - CL42T](https://www.stepperonline.nl/closed-loop-stepper-driver-0-3-0a-24-48vdc-voor-nema-11-14-17-stepper-motor-cl42t)
- [Closed Loop Stepper Driver V4.1 0-3.0A 24-48VDC - CL42T-V4.1](https://www.stepperonline.nl/closed-loop-stepper-driver-v4-1-0-3-0a-24-48vdc-voor-nema-11-14-17-stepper-motor-cl42t-v41)
- [Y-serie gesloten-lus stappenmotor driver V2.0 0-2,2A 24-50VDC - CL42Y-V20 ](https://www.stepperonline.nl/y-serie-gesloten-lus-stappenmotor-driver-v2-0-0-2-2a-24-50vdc-voor-nema-17-stappenmotoren-cl42y-v20)

Dit zijn allemaal closed loop systemen, dit betekend dat er gemeten kan worden ofdat de motor wel alle benodigde rotaties maakt of niet. Dit is zeker een failsafe waar ik gebruik van wil maken.

optie 2 (CL42T-4.1) lijkt de breedste specs te hebben, en een modernere versie te zijn van de 1e optie. Ik ga deze kiezen omdat ik hoop dat deze voordelen helpen met mogelijke problemen die ik nu niet kan voorzien.
### ~~nanotec driver~~
De motor driver zal net zoals de motor bij [Nanotec](https://en.nanotec.com/) gekozen worden. Om te zorgen dat de goede gekozen word blijf ik filters aanpassen totdat er een keuze uit komt. [Brushless DC & Stepper Motor Controllers/Drives \| Nanotec](https://www.nanotec.com/eu/en/products/158-motor-controllers-drives)
- Matching Motors
  Er word gezocht naar een steppermotor driver
- Encoder input
  Ik wil er liever geen hebben, maar dan blijft er slechts een optie over. Er word ook nog gekeken naar een encoder driver combi.
- Operating Voltage
  kijkend naar het moment grafiek de motor ([ST5909S1008-A](https://www.nanotec.com/eu/en/products/483-st5909s1008-a)) is te zien dat een minimum van 24V parallel en 48V single verstandig lijkt.
Alle opties die uit deze zoekopdracht komen zien er vreemd uit. Ik weet niet of deze wel of niet goed zijn maar ik ga het er niet op gokken.