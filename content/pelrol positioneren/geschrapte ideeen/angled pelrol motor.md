# angled pelrol motor
de enige motor die in PLM in de buurt komt van 4 RPM is (624569)
dit is een 0.18KW motor (wat waarschijnlijk meer als genoeg is), deze motor draait met 4.7 RPM, maar dit kan zo nodig versneld worden met een frequentie regelaar.
![[Pasted image 20251016091621.png]]

## hoe snel moet de pelrol bewegen?
- de pelrol willen we zo snel mogelijk verplaatsen, maar we willen ook een goedkope optie hebben. Om toch een keuze te maken kan er zo veel mogelijk vanuit PLM gekozenen worden.

## hoeveel kracht moet er geleverd worden?
- de enige kracht die opgevangen moet worden is van de staalborstel. Deze kracht zal in stilstand opgevangen moeten worden.

volgens [[PLM motor]] heeft de motor een koppel van 4,775Nm. Wanneer dit gedeeld wordt door de radius van de borstel(.1m) krijg je een axiale as belasting van **47.75 N**. 
In het echt zal deze kracht nooit behaald worden sinds het volledige moment van de motor nooit bereikt zal worden.

benodigde moment: [[beweging schroef]]
$$T=F\cdot\frac{d_2}{2}\cdot\tan\left(\phi\pm\rho^{\prime}\right)$$
waarin 
T = moment
F = kracht van de pelrol = 47.75N
$d_2$ = de [[flankdiameter]] = 0.018 m (*mogelijk veranderd met verandering in moet en spindel*)
$\Phi$ = de [[spoedhoek]]= 4 (*mogelijk veranderd met verandering in moet en spindel*)
$\rho^{\prime}$ = de [[schroefdraadwrijvingshoek]] =10 (*mogelijk veranderd met verandering in moet en spindel*)
$$47.75\cdot\frac{0.018}{2}\cdot\tan\left(4+10\right)=0.107 Nm$$
==**0.107Nm houdkracht