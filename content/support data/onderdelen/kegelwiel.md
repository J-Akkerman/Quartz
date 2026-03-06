---
aliases:
  - bevel gear
---
# Kegelwiellen
Een **kegelwieloverbrenging** (ook wel **conische tandwieloverbrenging, bevel gear**) is een overbrengingssysteem waarbij twee assen onder een hoek (meestal 90°) vermogen overdragen door middel van conische tandwielen. Deze worden veel gebruikt in machinebouw en aandrijftechniek waar een compacte haakse overbrenging gewenst is.
![[image-1.jpg]]
## Type kegelwiellen
Kegeltandwielen worden onderverdeeld op basis van de tandvorm en tandopstelling. De belangrijkste types zijn:

- Rechte kegeltandwielen
- Spiraalvormige kegeltandwielen
- Zerol kegeltandwielen
- Kruiskegelwielen / Miter gears
- Hypoïde tandwielen

Elk type heeft unieke eigenschappen en toepassingsgebieden.
### rechte vertanding

![[Untitled-1 1.jpeg]]

Recht vertande kegeltandwielen worden meestal toegepast bij **lage toerentallen**, bijvoorbeeld in:
- handelgedreven machines
- schuifhaspels
- kranen
- **Snelheid**: tot ca. **6 m/s** bij standaard tanden, en tot ca. **20 m/s** bij [[geslepen tanden]].
- **Voordeel**: eenvoudig te produceren en veroorzaken **geen axiale stuwkracht**.
---
### Spiraalvormige kegeltandwielen

![[Untitled-1 2.jpeg]]

Spiraalvormige kegeltandwielen hebben gebogen tanden die langs kromme lijnen op een steekkegel zijn geplaatst.

**Eigenschappen**:
- Langzamere tand-ingang → gelijkmatiger contact
- Soepele en stille werking, zelfs bij hoge snelheid
- Hogere efficiëntie dan rechte kegeltandwielen
**Toepassingen**:
- auto-overbrengingen
- machinegereedschap
- reductiekasten voor hoge prestaties
---
### Zerol kegeltandwielen

![[images.jpeg]]
Zerol kegeltandwielen hebben tanden met een cirkelvormige boog in het midden.

- De tanden zijn **gebogen maar niet gekanteld**.
- Gecombineerd voordeel: eenvoud van rechte kegeltandwielen + soepele werking van spiraalvormige kegeltandwielen.
- Worden geproduceerd met het [[spiraal snijproces]], maar leveren een uniek tandprofiel.

**Eigenschappen**:

- nauwkeurige en efficiënte krachtoverdracht
- minder trillingen en geluid
---
### Miter gears (Kruiskegelwielen)

![[Untitled-1 3.jpeg]]

**Miter gears** zijn een speciale vorm van kegeltandwielen met een **1:1 overbrengingsverhouding** (evenveel tanden op beide wielen).

**Eigenschappen**:
- draaien de rotatierichting 90°
- geen verandering in snelheid of koppel

**Voordelen**:
- eenvoudige constructie
- compact en efficiënt
- lage kosten
**Nadelen**:
- beperkte belastbaarheid
- geschikt voor matige snelheden en koppels
**Toepassingen**:
- aanrijfsysteme
- versnellingsbakken
- mechanische richtingsverandering
---
### Hypoïde tandwielen
![[Untitled 1.jpeg]]
Hypoïde tandwielen lijken op spiraalvormige kegeltandwielen, maar de assen kruisen elkaar **niet**: ze zijn **verschoven** (offset).

**Eigenschappen**:
- maken compactere constructies mogelijk
- stiller en sterker bij hoge belastingen
- vaak gebruikt in differentieelsystemen van auto’s

## geometrie en naamgeving

![[Pasted image 20250918115813.png]]
![[Pasted image 20250918115505.png]]
- buitenste modulus $m_e$
  vaak bepaald volgens NEN 1630 (DIN 780)
- gemiddelde modulus $m_m$
  vaak bepaald volgens NEN 1630 (DIN 780)
- iets modulus ??? $m_r$
- aantal tanden *z*
- kroonwielsteek $p_r$ 
  $m_r \cdot \pi$
- normale steek $p_m$
  $p_{m}=m_{m}\cdot\pi$
- tanddikte op de steekcirkel $s_r$
  $(m_r \cdot \pi)/2$
- kuilwijdte op de steekcirkel $e_r$
  $(m_r \cdot \pi)/2$
- drukhoek $\alpha_r$ 
  $20^\circ$(standaard)
- tandkophoogte $h_{ar}$
- tandvoethoogte $h_{vr}$
- totale tandhoogte $h_r$
  $h_{ar} + h_{vr}$
- topafname (tandspeling)$c_r = (0,1 \dots 0,3) \cdot m_r$
- buitenste steekcirkeldiameter $d_e$ 
  $z\cdot m_{e}=d_{m}+b\star\sin\left(\phi\right)$
- gemiddelde steekcirkeldiameter $d_m$
  $z\cdot m_{m}=z\cdot m_{e}\cdot\frac{R_{m}}{R_{e}}=d_{e}-b\cdot\sin\left(\phi\right)$
- steekkegelhoek van het drijvende wiel  $\phi_1$ 
  de steekkegelhoek is de hoek die de buitenste vertanding maakt in relatie tot de as
- steekkegelhoek van het gedreven wiel  $\phi_2$ 
  de steekkegelhoek is de hoek die de buitenste vertanding maakt in relatie tot de as
- ashoek $\sum$ 
  is de hoek tussen de assen van twee kegeltandwielen. 
  $\sum=\phi_1+\phi_2$ (houd dus ook rekening met de steekhoeken als je een unieke ashoek nodig hebt)
- rugkegel
  punt $O_1$ en $O_2$ zijn deel van 2 kegelvormen die elk bestaan uit het wiel als boden en twee stippellijnen die loodrecht op de steekkegel liggen. Dit is de rugkegel en word gebruikt om afmetingen van de tanden (steek, tandhoogte, enz.) 
- buitenste steekkegellengte $R_e$
  $\frac{d_{e}}{2\cdot\sin\left(\phi\right)}\ge3\cdot b$
- gemiddelde steeklengte $R_m$
  $\frac{d_{m}}{2\cdot\sin\left(\phi\right)}=R_{e}-\frac{b}{2}$
- binnenste steekcirkellengte $R_i$
  $\frac{d_{i}}{2\cdot\sin\left(\phi\right)}=R_{e}-b$
- tandbreedte $b$
  $b\le\frac{R_3}{3}$
  $b\le10\cdot m_{e}$
  $b\sim0.15\cdot d_{el}\cdot\sqrt{u^2+1}$
## Ontwerp- en berekeningsaspecten
### grenswaardes
Voor kegeltandwielen geldt, net als bij [[tandwiel|cilindrische tandwielen]], een **minimum aantal tanden**. 
omdat voor rechte cilindrische tandwielen zonder profielverschuiving $z_{\min} = 17$ is, geldt voor kegeltandwielen:

$$
z_{v\min} \approx 17,\quad z_{\min} = z_{v\min}\cos\delta = 17\cos\delta
$$
👉 Dit betekent: hoe groter de **steekhoek** $\delta$, hoe kleiner het minimaal benodigde aantal tanden wordt.

Wanneer een tandwiel minder tanden heeft dan dit minimum ($z < z_{v\min}$), ontstaat er [[ondersnijding]].  
Om dat te voorkomen, moet er een [[profielverschuiving]] worden toegepast:

$$
x_{\mathrm{tot}} = \frac{14 - z_{v\min}}{17}\cdot\frac{z}{\cos\delta}
$$

Zelfs bij profielverschuiving geldt nog een absoluut **minimum aantal tanden**. 
Voor cilindrische tandwielen is dat $z_{\min} = 7$.
Voor kegeltandwielen hangt dit af van de steekhoek $\delta$ en te berekenen met voorheen genoemde formule:

|Steekhoek $\delta$|< 15°|20°|30°|38°|45°|
|---|---|---|---|---|---|
|**Minimaal aantal tanden $z_{\min}$**|7|7|7|6|6|
|**Virtueel aantal tanden $z_{v\min}$**|17|16|13|11|10|
### overbrengverhouding (alleen rechte vertanding gecheckt)
$$i=\frac{n_1}{n_2}=\frac{d_{e2}}{d_{e1}}=\frac{r_{e2}}{r_{e1}}=\frac{z_2}{z_1}=\frac{\sin\left(\phi_2\right)}{\sin\left(\phi_1\right)}$$
waarin:
- n = toerental
- d = buitenste diameter
- r = buitenste straal
- z = hoeveelheid tanden
- $\phi$ = steekkegelhoek
### tandverhouding (alleen rechte vertanding gecheckt)
$$u=\frac{z_{groot}}{z_{klein}}\leq1$$
waarin
- u = tandverhouding
- z = hoeveelheid tanden
### steekkegelhoek  (alleen rechte vertanding gecheckt)
voor ashoeken van $\sum\leq90$ 
$$\tan\left(\phi_1\right)=\frac{\sin\left(\sum\right)}{u+\cos\left(\sum\right)}$$
voor ashoek van $\sum>90$
$$\tan\left(\phi_1\right)=\frac{\sin\left(180-\sum\right)}{u-\cos\left(180-\sum\right)}$$
waarin:
- u = tandverhouding
- $\phi$ = steekkegelhoek
- $\sum$ = ashoek
### kegelwiel belasting
Bij het in elkaar grijpen van kegelwielen met een ashoek Σ = 90 graden, geldt dat de axiale kracht die op het aangedreven tandwiel werkt gelijk is aan de radiale kracht die op het aangedreven tandwiel werkt. Evenzo is de radiale kracht die op het aandrijvende tandwiel werkt gelijk aan de axiale kracht die op het aangedreven tandwiel werkt.

#### rechte kegelwieloverbrenging  
| Type tandwiel           | Tangentiële kracht $F_t$                              | Axiale kracht $F_x$                                                                                                                                                                                                       | Radiale kracht $F_r$                                                                                                                                                                                                     |
| ----------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Straight bevel gear** | $$F_t = \frac{2000T}{d_m}$$                           | $$F_x = F_t \tan \alpha \sin \delta$$                                                                                                                                                                                     | $$F_r = F_t \tan \alpha \cos \delta$$                                                                                                                                                                                    |
hieronder zie je hoe de krachten werken op een rechte kegelwieloverbrenging.

![Fig 12.3 Directions of Forces acting on a Straight Bevel Gear Mesh](https://khkgears.net/new/images/Gear-Forces/Fig-12.3-Directions-of-Forces-acting-on-a-Straight-Bevel-Gear-Mesh.jpg)
#### spiraalvormige kegelwieloverbrenging
| Tangentiële kracht $F_t$                              | Axiale kracht $F_x$                                                                                                                                                                                                       | Radiale kracht $F_r$                                                                                                                                                                                                     |
| ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| $$F_t = \frac{2000T}{d_m},\ d_m = d - b \sin \delta$$ | Convex werkend: $$F_x = \frac{F_t}{\cos \beta_m} (\tan \alpha_n \sin \delta - \sin \beta_m \cos \delta) $$<br> Concave werkend: $$F_x = \frac{F_t}{\cos \beta_m} (\tan \alpha_n \sin \delta + \sin \beta_m \cos \delta)$$ | Convex werkend: $$F_r = \frac{F_t}{\cos \beta_m} (\tan \alpha_n \cos \delta + \sin \beta_m \sin \delta)$$<br> Concave werkend: $$F_r = \frac{F_t}{\cos \beta_m} (\tan \alpha_n \cos \delta - \sin \beta_m \sin \delta)$$ |
De tanden van spiraalvormige kegelwielen hebben bolle en holle zijden. Afhankelijk van op welk oppervlak de kracht werkt, veranderen zowel de richting als de grootte van de kracht. Dit verschilt bovendien afhankelijk van welk tandwiel de aandrijver is en welk het aangedreven tandwiel.
![Fig.12.4 Convex surface and concave surface of a spiral bevel gear](https://khkgears.net/new/images/Gear-Forces/Fig.12.4-Convex-surface-and-concave-surface-of-a-spiral-bevel-gear.jpg)  
![Table 12.5 Meshing Tooth Face](https://khkgears.net/new/images/Gear-Forces/Table-12.5-Meshing-Tooth-Face.jpg)
- **Spiral-hand (L of R)**: Geeft de draairichting van de spiraal van de tand aan (Links- of Rechtsdraaiend).
- **Drive Gear Rotatierichting (CW/CCW)**: Richting waarin het aandrijvende tandwiel draait (Clockwise / Counterclockwise).
- **Mashing tooth face**: Het contactvlak van de tanden dat met het andere tandwiel in aanraking komt. Voor het aandrijvende tandwiel kan dit bol (convex) of hol (concave) zijn, afhankelijk van draairichting en spiraalhand.
- **Driven Gear**: Het aangedreven tandwiel; het contactvlak en draairichting zijn afhankelijk van het aandrijvende tandwiel.
- De laatste kolom geeft de spiral-hand van het aangedreven tandwiel weer, die tegengesteld is aan het aandrijvende tandwiel.
![Fig.12.5 The Directions of Forces Carried by Spiral Bevel Gears 1](https://khkgears.net/new/images/Gear-Forces/Fig.12.5-The-Directions-of-Forces-Carried-by-Spiral-Bevel-Gears-1.jpg)  
![Fig.12.5 The Directions of Forces Carried by Spiral Bevel Gears 2](https://khkgears.net/new/images/Gear-Forces/Fig.12.5-The-Directions-of-Forces-Carried-by-Spiral-Bevel-Gears-2.jpg)  
![Fig.12.5 The Directions of Forces Carried by Spiral Bevel Gears 3](https://khkgears.net/new/images/Gear-Forces/Fig.12.5-The-Directions-of-Forces-Carried-by-Spiral-Bevel-Gears-3.jpg)  
![Fig.12.5 The Directions of Forces Carried by Spiral Bevel Gears 4](https://khkgears.net/new/images/Gear-Forces/e8b037d64e9fe5587615fddc3b86cddf.jpg)
#### voorbeelden
Table 12.3 Calculation Examples (Spiral Gear)  
![Table 12.3 Calculation Examples （Spiral Gear）](https://khkgears.net/new/images/Gear-Forces/c46b2d5fd444941d3d5e92b069e2484b.jpg)

Table 12.4 Calculation Examples (Straight Bevel Gear)  
![Table 12.4 Calculation Examples（Straight Bevel Gear）](https://khkgears.net/new/images/Gear-Forces/01d3f0d8b43a80b3c40e6f235d12ec72.jpg)


![Table 12.6 Calculation Examples (Spiral Bevel Gears)](https://khkgears.net/new/images/Gear-Forces/Table-12.6-Calculation-Examples-Spiral-Bevel-Gears.jpg)
erhouding
De verhouding volgt uit het aantal tanden:
$i = \dfrac{z_2}{z_1}$  
waarbij:
- $i$ = overbrengingsverhouding  
- $z_1$ = aantal tanden op het kleinste wiel (pignon)  
- $z_2$ = aantal tanden op het grootste wiel  
### Draaisnelheden
verschillende soorten kegeltandwielen hebben verschillende maximale snelheden:
- rechte ongeslepen vertanding ongeveer 6m/s
- rechte geslepen vertanding ongeveer 20m/s
### Modul en tandgrootte
- De keuze van **modul** ($m$) bepaalt de tandgrootte en daarmee de belastbaarheid.  
- Voor kegelwielen geldt: $d = m \cdot z$, waarbij $d$ de deelcirkel diameter is.  
- De conische vorm vraagt extra correctiefactoren bij berekeningen (bijvoorbeeld voor tandbreedte en drukhoek).  

### Koppeloverdracht
Het uitgangskoppel volgt uit:
$M_2 = M_1 \cdot i \cdot \eta$  
waarbij:
- $M_1$ = ingangs-koppel  
- $M_2$ = uitgangs-koppel  
- $\eta$ = rendement (afhankelijk van wrijving, meestal 0,95–0,98 voor goed ontworpen tandwielen)  
## leveranciers
- [[chiaravalli]]
  ![[Chiaravalli_Bevel_Gears_catologus.pdf]]