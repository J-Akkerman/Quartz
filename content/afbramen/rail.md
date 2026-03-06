---
prod/koop: koop onderdeel
leverancier: hepco motion
waar te vinden: "[[QBNL19481.pdf]]"
identificatie: RES351 R180
kosten/eenheid: 296.87
hoeveelheid: 1
---
### belasting
belasting op de rail:
- moment over rail: 4.841Nm
  ![[Rail moment]]de [[swingtool.pdf|swingunit]] heeft samen met de mounting setup een gewicht van 4.2 Kg en dus een neerwaartse kracht van 41.2 N. 
  Deze neerwaartse kracht zal een stuk van de rail af plaatsvinden en zal hier dus een moment creeëren van $41.2\cdot\frac{117.5}{1000}=4.841Nm$
- kracht over rail:
  De neerwaartse kracht kan worden opgesplitst in krachten in de richting van de rail en krachten haaks op de rail met de volgende formulles:
  ![[rail belasting]]$$F_{t}=\sin\left(\alpha\right)\cdot F_{g}$$$$\sin\left(25\right)\cdot41.2=17.41N$$ $$F_{t}=\cos\left(\alpha\right)\cdot F_{g}$$ $$\cos\left(0\right)\cdot41.2=41.2N$$
    Waarin:
  $F_t$= tangiele kracht op de rail
  $F_h$= de haakse kracht op de rail 
  $F_g$= het gewicht van de [[swingtool.pdf|swingunit]] en het karretje 4.2 Kg
  $\alpha=$ de hoek van de rail, Max 25 graden
### rail keuze
benodigde diameter van de rail
ik wil de rail graag direct achter de swingunit gemonteerd hebben.
Verder moet het centerpunt van de rail precies op de juiste locatie van het slijpschijfje liggen.
Deze restricties zorgen ervoor dat de radius van de rail gelijk moet zijn als de lengte van de swingunit arm. Deze kan lichtjes aangepast worden door de slijpschijf een stukje verder uit te schuiven, maar het liefste houden we de lengte die in de cel word gebruikt zo goed mogelijk aan. 
Dit geeft een radius van 159 mm

Tussen de geleidingsringen is er keuze uit 3 soorten:
- Dubbelzijdige Geleideringen
  ![[Pasted image 20251118121626.png]]
- ~~Uitwendige Enkelzijdige Geleideringen~~ hier passen geen karretjes op
  ![[Pasted image 20251118121645.png]]
- ~~Inwendige Enkelzijdige Geleideringen~~ hier passen geen karretjes op
  ![[Pasted image 20251118121705.png]]

![[Pasted image 20251118121950.png]]

na verdere opmetingen te maken in CAD is er gekozen voor: RES351 R180 (Q$^*$).[[hepco track guide.pdf#page=15]
$^*$ Q is alleen nodig wanneer er gebruik word gemaakt van een aangedreven systeem. (is uiteindelijk niet voor gekozen)
### rail hoek
180 graden van deze rail is te veel voor de huidige situatie, deze zal dus ingekort moeten worden. om de juiste hoeken te beslissen zijn de volgende berekeningen gemaakt:
![[afbraam rail dimensies]]
Voor de bovenstaande schets is te berekenen dat:
- $P_{R}$= 54.26= de minimale [[pelrol dimensionering|rechter pitch]], deze heeft het meeste rail nodig
- $P_{L}$= 54.26= de minimale [[pelrol dimensionering|linker pitch]], deze heeft het meeste rail nodig
- $A_1$= $\tan^{-1}\left(80.527/159\right)=26.86\degree$
- $A_2$=$\tan^{-1}\left(81/159\right)=27\degree$
- $B1=P_{r}-A1=54.26-26.86=27.4\degree$ 
- $B2=P_{L}-A_2=54.26-27=27.26\degree$ bepaald de *positie* van de rail op de [[- definitie afbramer#mountplate|mountplate]]
- $A=180-B_1-B_2=180-27.4-27.26=125.34\degree$

Ik ga dit vergroten naar **130 graden** zodat er extra tolerantie is.