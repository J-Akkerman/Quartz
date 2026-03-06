# tandwiel belasting
[Gear Forces \| KHK G...](https://khkgears.net/new/gear_knowledge/gear_technical_reference/gear_forces.html)
## overvieuw
![Fig. 12.1 Direction of Forces Acting on a Gear](https://khkgears.net/new/images/Gear-Forces/Fig.-12.1-Direction-of-Forces-Acting-on-a-Gear.jpg)
Wanneer het tandwielkoppel vermogen overbrengt, werken er krachten op de tandwielen. Zoals hierboven weergegeven, geldt het volgende als de Z-as de as van het tandwiel aangeeft:

- De kracht die in de X-richting werkt, wordt gedefinieerd als de **tangentiële kracht Ft (N)**
- De kracht die in de Y-richting werkt, wordt gedefinieerd als de **radiale kracht Fr (N)**
- De kracht die in de Z-richting werkt, wordt gedefinieerd als de **axiale kracht Fx (N)**

Bij het ontwerpen van een tandwiel is het essentieel om deze krachten op de tandwielen, assen, lagers, enz. te analyseren.

| Type tandwiel               | Tangentiële kracht $F_t$                                                                                            | Axiale kracht $F_x$                                                                                                                                                                                                       | Radiale kracht $F_r$                                                                                                                                                                                                     |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Spur gear**               | $$F_t = \frac{2000T}{d}$$                                                                                           | –                                                                                                                                                                                                                         | $$F_{r}=F_{t}\cdot\tan\left(\alpha\right)$$                                                                                                                                                                              |
| **Helical gear**            | $$F_t = \frac{2000T}{d}$A$                                                                                          | $$F_x = F_t \tan \beta$$                                                                                                                                                                                                  | $$F_r = F_t \frac{\tan \alpha_n}{\cos \beta}$$                                                                                                                                                                           |
| **Straight bevel gear**     | $$F_t = \frac{2000T}{d_m}$$                                                                                         | $$F_x = F_t \tan \alpha \sin \delta$$                                                                                                                                                                                     | $$F_r = F_t \tan \alpha \cos \delta$$                                                                                                                                                                                    |
| **Spiral bevel gear**       | $$F_t = \frac{2000T}{d_m},\ d_m = d - b \sin \delta$$                                                               | Convex werkend: $$F_x = \frac{F_t}{\cos \beta_m} (\tan \alpha_n \sin \delta - \sin \beta_m \cos \delta) $$<br> Concave werkend: $$F_x = \frac{F_t}{\cos \beta_m} (\tan \alpha_n \sin \delta + \sin \beta_m \cos \delta)$$ | Convex werkend: $$F_r = \frac{F_t}{\cos \beta_m} (\tan \alpha_n \cos \delta + \sin \beta_m \sin \delta)$$<br> Concave werkend: $$F_r = \frac{F_t}{\cos \beta_m} (\tan \alpha_n \cos \delta - \sin \beta_m \sin \delta)$$ |
| **Worm gear pair (Driver)** | $$F_{t1} = \frac{2000T_1}{d_1}$$                                                                                    | $$F_x = \frac{F_{t1} \cos \alpha_n \cos \gamma - \mu \sin \gamma}{\cos \alpha_n \sin \gamma + \mu \cos \gamma}$$                                                                                                          | $$F_r = \frac{F_{t1} \sin \alpha_n}{\cos \alpha_n \sin \gamma + \mu \cos \gamma}$$                                                                                                                                       |
| **Worm gear pair (Driven)** | $$F_{t2} = F_{t1} \frac{\cos \alpha_n \cos \gamma - \mu \sin \gamma}{\cos \alpha_n \sin \gamma + \mu \cos \gamma}$$ | $$F_x = F_{t1}$$                                                                                                                                                                                                          | $$F_r = \frac{F_{t1} \sin \alpha_n}{\cos \alpha_n \sin \gamma + \mu \cos \gamma}$$                                                                                                                                       |
| **Screw gear (Driver)**     | $$F_{t1} = \frac{2000T_1}{d_1}$$                                                                                    | $$F_x = \frac{F_{t1} \cos \alpha_n \sin \beta - \mu \cos \beta}{\cos \alpha_n \cos \beta + \mu \sin \beta}$$                                                                                                              | $$F_r = \frac{F_{t1} \sin \alpha_n}{\cos \alpha_n \cos \beta + \mu \sin \beta}$$                                                                                                                                         |
| **Screw gear (Driven)**     | $$F_{t2} = F_{t1} \frac{\cos \alpha_n \sin \beta - \mu \cos \beta}{\cos \alpha_n \cos \beta + \mu \sin \beta}$$     | $$F_x = F_{t1}$$                                                                                                                                                                                                          | $$F_r = \frac{F_{t1} \sin \alpha_n}{\cos \alpha_n \cos \beta + \mu \sin \beta}$$                                                                                                                                         |
- $d_m$​ = centrale referentiediameter bij bevel tandwielen.
- $β_m​$ = gemiddelde helixhoek bij conische tandwielen.
- $α_n$​ = drukhoek normaal.
- γ = wormspoedhoek.
- μ = wrijvingscoëfficiënt.
## belasting op een [[tandwiel]]
de krachten die werken op de tanden van een spiraalvormig tandwiel en grotere spoelhoek van de tanden resulteert in een grotere axiale kracht (druk). In het geval van rechte tandwielen werkt er geen axiale kracht op de tanden.

![Fig.12.2 Direction of Forces acting on a Helical Gear Mesh 1](https://khkgears.net/new/images/Gear-Forces/Fig.12.2-Direction-of-Forces-acting-on-a-Helical-Gear-Mesh-1.jpg)  
![Fig.12.2 Direction of Forces acting on a Helical Gear Mesh 2](https://khkgears.net/new/images/Gear-Forces/Fig.12.2-Direction-of-Forces-acting-on-a-Helical-Gear-Mesh-2.jpg)

Table 12.2 Calculation Examples (Spur Gear)  
![Table 12.2 Calculation Examples (Spur Gear)](https://khkgears.net/new/images/Gear-Forces/Table-12.2-Calculation-Examples-Spur-Gear.jpg)

## belasting op een [[kegelwiel]]

Bij het in elkaar grijpen van kegelwielen met een ashoek Σ = 90 graden, geldt dat de axiale kracht die op het aangedreven tandwiel werkt gelijk is aan de radiale kracht die op het aangedreven tandwiel werkt. Evenzo is de radiale kracht die op het aandrijvende tandwiel werkt gelijk aan de axiale kracht die op het aangedreven tandwiel werkt.

### rechte kegelwieloverbrenging  
| Type tandwiel           | Tangentiële kracht $F_t$                              | Axiale kracht $F_x$                                                                                                                                                                                                       | Radiale kracht $F_r$                                                                                                                                                                                                     |
| ----------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Straight bevel gear** | $$F_t = \frac{2000T}{d_m}$$                           | $$F_x = F_t \tan \alpha \sin \delta$$                                                                                                                                                                                     | $$F_r = F_t \tan \alpha \cos \delta$$                                                                                                                                                                                    |
hieronder zie je hoe de krachten werken op een rechte kegelwieloverbrenging.

![Fig 12.3 Directions of Forces acting on a Straight Bevel Gear Mesh](https://khkgears.net/new/images/Gear-Forces/Fig-12.3-Directions-of-Forces-acting-on-a-Straight-Bevel-Gear-Mesh.jpg)
### spiraalvormige kegelwieloverbrenging
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
### voorbeelden
Table 12.3 Calculation Examples (Spiral Gear)  
![Table 12.3 Calculation Examples （Spiral Gear）](https://khkgears.net/new/images/Gear-Forces/c46b2d5fd444941d3d5e92b069e2484b.jpg)

Table 12.4 Calculation Examples (Straight Bevel Gear)  
![Table 12.4 Calculation Examples（Straight Bevel Gear）](https://khkgears.net/new/images/Gear-Forces/01d3f0d8b43a80b3c40e6f235d12ec72.jpg)


![Table 12.6 Calculation Examples (Spiral Bevel Gears)](https://khkgears.net/new/images/Gear-Forces/Table-12.6-Calculation-Examples-Spiral-Bevel-Gears.jpg)

## belasting op een [[wormwieloverbrenging]] 
Figuur 12.6 toont hoe de krachten werken op de tanden van een wormwieloverbrenging met een ashoek Σ = 90 graden.  
Omdat de krachtoverbrenging in een wormwieloverbrenging voornamelijk gebaseerd is op **glijdend contact** (in plaats van rollend contact zoals bij gewone tandwielen), heeft de **wrijvingscoëfficiënt** van het tandoppervlak een grote invloed op de **overbrengingsrendement (ηR)** en de grootte van de krachten die op het tandcontact werken.

een hogere wrijving leidt tot meer energieverlies (lager rendement) en grotere krachten op de tanden, wat de belasting op de lagers en de slijtage kan verhogen.
![formula 12.2](https://khkgears.net/new/images/Gear-Forces/formula-12.2.jpg)

![Fig. 12.6 Direction of Forces in a Worm Gear Pair Mesh 1](https://khkgears.net/new/images/Gear-Forces/Fig.-12.6-Direction-of-Forces-in-a-Worm-Gear-Pair-Mesh-1.jpg)  
![Fig. 12.6 Direction of Forces in a Worm Gear Pair Mesh 2](https://khkgears.net/new/images/Gear-Forces/Fig.-12.6-Direction-of-Forces-in-a-Worm-Gear-Pair-Mesh-2.jpg)

| Type tandwiel               | Tangentiële kracht $F_t$                                                                                            | Axiale kracht $F_x$                                                                                              | Radiale kracht $F_r$                                                               |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
| **Worm gear pair (Driver)** | $$F_{t1} = \frac{2000T_1}{d_1}$$                                                                                    | $$F_x = \frac{F_{t1} \cos \alpha_n \cos \gamma - \mu \sin \gamma}{\cos \alpha_n \sin \gamma + \mu \cos \gamma}$$ | $$F_r = \frac{F_{t1} \sin \alpha_n}{\cos \alpha_n \sin \gamma + \mu \cos \gamma}$$ |
| **Worm gear pair (Driven)** | $$F_{t2} = F_{t1} \frac{\cos \alpha_n \cos \gamma - \mu \sin \gamma}{\cos \alpha_n \sin \gamma + \mu \cos \gamma}$$ | $$F_x = F_{t1}$$                                                                                                 | $$F_r = \frac{F_{t1} \sin \alpha_n}{\cos \alpha_n \sin \gamma + \mu \cos \gamma}$$ |
### reken voorbeeld
![Table 12.7 Calculation Examples (Worm Gear Pair)](https://khkgears.net/new/images/Gear-Forces/Table-12.7-Calculation-Examples-Worm-Gear-Pair.jpg)

## belasting op een [[Schroef tandwiel]] 
de krachten in een schroef tandwiel zijn bijna gelijk aan die in een wormwieloverbrenging. 
![Fig 12.7 Direction of Forces in a Screw Gear Mesh 1](https://khkgears.net/new/images/Gear-Forces/Fig-12.7-Direction-of-Forces-in-a-Screw-Gear-Mesh-1.jpg)  
![Fig 12.7 Direction of Forces in a Screw Gear Mesh 2](https://khkgears.net/new/images/Gear-Forces/Fig-12.7-Direction-of-Forces-in-a-Screw-Gear-Mesh-2.jpg)

Table 12.8 Calculation Examples (Screw Gear)  
![Table 12.8 Calculation Examples (Screw Gear)](https://khkgears.net/new/images/Gear-Forces/Table-12.8-Calculation-Examples-Screw-Gear.jpg)