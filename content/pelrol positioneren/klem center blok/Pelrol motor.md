---
prod/koop: koop onderdeel
leverancier: nanotec
waar te vinden: "[Product Configurator | Nanotec](https://www.nanotec.com/eu/en/products/product-configurator/580::114_580:2902/)"
identificatie: ST8918L6708-A
kosten/eenheid: 196.2
hoeveelheid: 1
---
# specs eisen
- De pelrol in de afbraam cel draait met een snelheid van **4RPM**, dit wil ik ook gaan nabootsen binnen de backup
- in [[spindel en aanhang]] is berekend dat wanneer de pelrol motoren het maximale koppel gebruiken (dit zal nooit gebeuren) de pelrol word belast met **47.75N** met de dikste pelrol van 28mm word het moment $47.75\cdot0.028=$ **1.337Nm**. Dit houd ruim rekening met pelrol belasting, maar niet met wrijving. 
  Om de wrijving te verminderen zal er bij de wrijvende gedeeltes gebruik worden gemaakt van glad materiaal in het [[- definitie klem center blok]].
  Omdat dit een groot onbekend iets is ga ik kiezen voor een motor met minimaal **7 Nm** draaikracht
# pelrol motor
Ik heb met Roy gesproken, hij gaf aan dat je met een frequentie regelaar de motor prima kan limiteren tot 4RPM. Hij zal binnen het magazijn gaan kijken wat de opties zijn. Maar Marel werkt bijna exclusief met Grote motoren, dus het word even kijken wat er uiteindelijk nodig blijkt te zijn. 

[[Stappenmotor]] blijkt bij ver de beste keuzen te zijn, word allen nooit gebruikt binnen Marel dus zou apart besteld moeten worden.
De stappen van een stappenmotor zullen zorgen voor een inconsistente snelheid in de pelrol. dit kan effect hebben op het [[afbramen concept]]. Om dit te verminderen de stap grootte zo klein mogelijk zijn, of er moet gebruik gemaakt kunnen worden van Microstepping

mogelijkheden:
op deze site [ST8918 - Stepper mot...](https://www.nanotec.com/eu/en/products/566-st8918-stepper-motor-nema-34) zijn NEMA 34 motors te vinden
![[Pasted image 20251022130640.png]]
- ST8918M6708-A [ST8918M6708-A - Step...](https://www.nanotec.com/eu/en/products/574-st8918m6708-a)
  zal met de gewilde RPM ongeveer 6.4 Nm torque hebben
  dit is met hele stappen, als je halve stappen zou willen toepassen zal je een hogere motor moeten hebben
  deze motor is 125 euro
- ST8918L6708-A
  zal met de gewilde RPM ongeveer 8.8 Nm torque hebben
  dit is met hele stappen, als je halve stappen zou willen toepassen zal je een hogere motor moeten hebben
  deze motor is 160 euro
er is ook gekeken om nog een tandwielenkast te gebruiken, maar deze beginnen vanaf 200 euro

een key aansluiting in de as is een extra 36 euro, wat het waard is om de aandrijf center betrouwbaarder te maken.

Omdat dit een belangrijk gedeelte is van het systeem wil ik deze motor liever te sterk hebben als te zwak, daarom kies ik voor de ST8918L6708-A motor [Product Configurator...](https://www.nanotec.com/eu/en/products/product-configurator/580::114_580:2902/)
![[Pasted image 20251022131955.png]]
## Motor Driver
Omdat nanotec geen goede opties heeft voor drivers ga ik deze kiezen van [StepperOnline](https://www.stepperonline.nl/stappenmotor-driver-controller) (waar ook de spindel motor is gekozen). De motors die gebruikt gaan worden Hebben een Current per Winding van 6.7A, de driver moet deze stroom comfortabel kunnen leveren op 24-48V. Met deze eisen blijven er 4 toepasbare opties over:
- [Closed Loop Stepper Driver V4.1 0-8.0A 24-48VDC - CL57T-V41](https://www.stepperonline.nl/closed-loop-stepper-driver-v4-1-0-8-0a-24-48vdc-voor-nema-17-23-24-stepper-motor-cl57t-v41)
- [Closed Loop Stepper Driver 0-8.2A 18-80VAC/24-110VDC - CL86T](https://www.stepperonline.nl/closed-loop-stepper-driver-0-8-2a-18-80vac-24-110vdc-voor-nema-34-stappenmotor-cl86t)
- [Closed Loop Stepper Driver V4.1 0-8.2A 18-80VAC/24-110VDC - CL86T-V41](https://www.stepperonline.nl/closed-loop-stepper-driver-v4-1-0-8-2a-18-80vac-24-110vdc-voor-nema-34-stepper-motor-cl86t-v41)
- [Stepper-driver met gesloten lus 0-8.0A 24-48VDC - CL57T](https://www.stepperonline.nl/stepper-driver-met-gesloten-lus-0-8-0a-24-48vdc-voor-nema-17-23-24-stappenmotor-cl57t)
optie 2(CL86T) lijkt hetzelfde merk te zijn als de motor gekozen voor de [[spindel en aanhang]], dit is ook de driver met de breedste specs. Ik ga deze kiezen om deze redenen.
# oudere overwegingen
## ~~poging 2 motor~~
De motor die de pelrol gaat aandrijven moet: 
- met 4RPM draaien
- een uptime rating van 40% of hoger 
- de aandrijving moet een gat zijn ipv. een as (zie [[aandrijf center]])
hiervoor gaat er gekeken worden binnen [[sew-eurodrive]]:
**dit bestaat niet dirrect koopbaar uit SEW, wat betekend dat er of een connectie gemaakt moet worden tussen een as en een [[aandrijf center]], de motor en de gearbox appart gekocht moeten worden. of de motor moet naar de zijkant gericht worden** 

een rechte [[hollow center gearbox]] kan goed gekocht worden bij [[apex dynamics]]. hier zou dan de beste keuze zijn een "PD + attachment" gearbox, deze lijkt het kleinste lichtste en geodkoopste te zijn. maar deze heeft wel maar een overbrengverhouding van maximaal 100. dus de motor zal moeten draaien op maximaal 400 RPM, wat niet mogelijk lijkt binnen de SEW collectie. Verder zijn er nog een paar opties gevoenden die kunnen voldoen aan eisen:
[PFII series - Straig...](https://www.apexdyna.nl/en/products/pfii-series)
[MGOH Series - High T...](https://www.apexdyna.nl/en/products/mgoh-series)
[MGOHC Series - High ...](https://www.apexdyna.nl/en/products/mgohc-series)
de laatste 2 drijven een flange aan, hiervoor zal een extra onderdeel ontworden moeten worden.
==**Ik zat vast in het idee van een motor met een tanswielkast, dit is niet een goede optie**==
## ~~oude motor~~
**moet veranderd worden ivm. ruimte limitaties gecreëerd door een vernieuwd [[- definitie klem center blok]]**
De motor die de pelrol gaat aandrijven moet: 
- met 4RPM draaien
- een uptime rating van 40% of hoger 
- als deze een versnellingskast gebruikt moet deze haaks zijn om momenten te verminderen
- lekker goedkoop zijn
- de aandrijving moet een gat zijn ipv. een as (zie [[aandrijf center]])
dit geeft 2 opties:
~~binnen PLM: 4724786~~
~~... kost 5000 euro.~~
~~![[Pasted image 20251021132159.png]]~~
buiten PLM: WA49R17DR2S56M4 van SEW 
deze lijkt goed te zijn, de prijs is maar 548 euro
![[Pasted image 20251021133735.png]]