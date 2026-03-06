voor het frame word er gebruik gemaakt van aluminium extrusies omdat deze makkelijk in elkaar te zetten zijn, en niet vervormen wanneer deze aan elkaar vast gemonteerd worden.

RK Rose+Krieger word als leverancier gebruikt, Math heeft in het verleden ook gebruik gemaakt van dit bedrijf.

het frame moet een aantal functies uitvoeren
- geleiding ondersteunen
- borstel verbinden
  hoogte instelbaar houden
- afbramer ondersteunen
  verticaal instelbaar
  ruimte voor aandrijving
  positie instellen
- alles aan elkaar verbinden

in\#geleiding_frame is gekozen dat er gebruik word gemaakt van F30 profielen en in en in borstel-frame is er gekozen voor een \#slot_geom van 40. [Aluminium profiles / size 30 - RK Rose+Krieger](https://rose-krieger.partcommunity.com/3d-cad-models/sso/aluminium-profiles-size-30-rk-rose-krieger?info=rose_krieger%2Falu_profilsysteme%2Fprofilsystem_blocan%2Fkonstruktionsprofile%2Fprofile_30&cwid=7912) de profielen lijken niet te kloppen

**wil ik nog end plates en caps?** ik maak er een advies van
# geleiding-frame
## profielen keuzes
![[f30x30 profiel]]
## borstel problemen
### staal borstel problemen
De staalborstel motor zit in de weg van het frame.
![[Pasted image 20251127093310.png]]
Om hieromheen te werken word er een deel van het frame weg gehaald. ![[Pasted image 20251127093808.png]]
### kunststof borstel problemen
op het moment komt er een klein stukje van de kunststof motor in contact met het geleiding frame:(rechtsboven)![[Pasted image 20251201133341.png]]
dit is simpel op te lossen door het frame in relatie tot de rest van het systeem een stukje naar rechts te bewegen \#onderdeel_positie. Het \#borstel_frame kan direct op het geleiding frame geplaatst als het systeem 8.7mm opgeschoven word.


verder zal het geleiding frame net de kunststof motor raken aan de voorkant:
![[Pasted image 20251202123459.png]]![[Pasted image 20251202123517.png]]
dit is maar een klein gebied, dus dit gedeelte uitsnijden zal geen problemen veroorzaken. 
![[Pasted image 20251202124256.png]]
## geleiding verbinding
~~vanuit PLM zijn er 3 verbind opties tussen de \#geleiding en het profiel die een steek van 120 hebben (net zoals de geleiding) en een \#slot_geom van 40: 4083214, 4083221 en 4082110. het grote verschil is de hoeveelheid gaten per T-nut. De geleiding heeft 9 gaten, dit kan perfect verbonden worden met 3x 4082110~~ er is slot geo f30 nodig

om deze te verbinden word er gebruik gemaakt van de stock [[bar material]] van rose+kruger [[bl_aluprofilsystem_en.pdf#page=94|4006200 3010]].
De geleiding heeft een speciale bout waar math meer van weet, deze moeten hier nog gemonteerd worden. #WIP
## extrusie hoekverbindingen
alle verbindingen aan andere gedeeltes van het frame is gedocumenteerd in de definitie van dat sub frame. in dit gedeelte word er alleen gesproken over de onderstaande situatie:
![[Pasted image 20251202113114.png]]
Er zijn 4 soortgelijke situaties in het frame waar waarschijnlijk dezelfde oplossing toegepast kan worden.

Rose+krieger levert meerdere [[bl_aluprofilsystem_en.pdf#page=46|right-ange connerction]] oplossingen. uit de volgende opties kan gekozen worden:
- Flange bracket connection
  ![[Pasted image 20251127101724.png]]
- Hidden screw -B-
  ![[Pasted image 20251127101814.png]]
- Bracing plates 
  ![[Pasted image 20251127101913.png]]
- connection plate 
  ![[Pasted image 20251127102354.png]]
- Angle brackets
  ![[Pasted image 20251127102421.png]]![[Pasted image 20251127102429.png]]![[Pasted image 20251127102441.png]]
~~Ik wil deze verbindingen zo stijf mogelijk hebben, een connection plate lijkt dit mogelijk te maken. Ik denk alleen dat hier te weinig ruimte voor is, het eerste gat laat maar een ruimte over van 10mm. een connenction plate is 15 mm~~

flange connections ([[bl_aluprofilsystem_en.pdf#page=50|4306709]]) zijn hier de beste optie
# Borstel frame 

![[Screenshot 2025-11-24 155205.png]]
![[Pasted image 20251124155230.png]]
## profiel keuze
In [[- definitie borstel]] zijn er al profielen gekozen om te zorgen dat de scharniern hier goed op gemonteerd kunnen worden. deze keuze is hieronder te zien
![[bovenste scharnier]]
## profielen verbinden
![[faceplate]]
## borstel-geleiding-verbinding
### staalborstel
op het moment van ontwerpen ziet de situate er als volgt uit:
![[Pasted image 20251127095738.png]]
~~De profielen zitten gelukkig wel op hoogte omdat het frame van het \#motor_boven_scharnier hierop is aangepast. hierdoor kan er een enkel **30x100** profiel over de bovenkant van de motor worden gemonteerd.~~ Om te zorgen dat de [[- definitie afbramer#axiale aandrijving]] goed gemonteerd word moet deze connectie bestaan uit 2 [[f30x60 profiel]] ([[bl_aluprofilsystem_en.pdf#page=28|4305000]]). Dit profiel word vervolgens met een custom connect stuk aan het geleiding frame verbonden. Dit versterkt ook het gedeelte van het frame wat verdund is
![[Pasted image 20251201141617.png]]
#### geleiding frame verbinding
![[Pasted image 20251201143426.png]]
De bovenstaande profielen moeten aan elkaar verbonden worden met een custom onderdeel. Dit onderdeel is niet heel complex maar moet aan de volgende eisen voldoen:
- goed stijf zijn
- minimaal 2 connectie punten per profiel verbinding
[[bl_aluprofilsystem_en.pdf|RK rose+krieger]] levert geen onderdelen die dit zouden kunnen. Het onderdeel wat het meeste in de buurt komt is een angeled bracket. Maar er bestaat geen profiel wat in deze excacte situatie past
dus is er gekozen voor volgende ontwerp:
![[Pasted image 20251201143454.png]]

Natuurlijk moet dit nog steeds verbonden worden aan het aluminium profiel, hiervoor word gekozen uit opties die in PLM staan. een T nut met 2 verbindingen en een steek van 30
####  **OUD** ~~motor frame verbinding~~
![[Pasted image 20251201145134.png]]
De bovenstaande profielen moeten aan elkaar verbonden worden. deze zullen veel moment moeten opvangen over de lengte vand e verbinding en moet dit dus ook goed aankunnen. 
dit moet gedaan worden met een [[bl_aluprofilsystem_en.pdf#page=68|cross connection]] van rose+krieger. 
![[Pasted image 20251127101244.png]]

aan de frame kant moet er gekozen worden uit een [[bl_aluprofilsystem_en.pdf#page=46|right-ange connerction]]. uit de volgende opties kan gekozen worden:
- Flange bracket connection
  ![[Pasted image 20251127101724.png]]
- Hidden screw -B-
  ![[Pasted image 20251127101814.png]]
- Bracing plates (waarschijnlijk te weinig ruimte voor)
  ![[Pasted image 20251127101913.png]]
- connection plate (Lijkt niet te bestaan)
  ![[Pasted image 20251127102354.png]]
- Angle brackets
  ![[Pasted image 20251127102421.png]]![[Pasted image 20251127102429.png]]![[Pasted image 20251127102441.png]]
Een angel bracket lijkt hier perfect alle krachten op te kunnen vangen. Er zijn 3 soorten angele brachtes:
- profile angle
  ![[Pasted image 20251201145652.png]]
- cast
  ![[Pasted image 20251201145610.png]]
- sheet steel
  ![[Pasted image 20251201145628.png]]
profile types passen niet
~~de profile type is de enige waarvan een klein stuk gekocht kan worden, hierdoor is het waarschijnlijk goedkoper. Er word gekozen voor een 100mm lange 4010102 profiel, omdat de grotere versie niet past.~~

~~de cast types maken gebruik van een centering rib die in deze situatie handig kan zijn voor uitlijnen.~~ ~~4695100 zou met een stuk beide groeven kunnen ondersteunen~~. ~~omdat alle opties die beide groeven met een profiel verbinden te groot zijn moet er worden gekozen voor 2 aparte profielen.~~ Deze moeten maximaal 50mm breed zijn, anders passen deze niet in de groeven

alle profielen lijken een stuk te groot te zijn voor de situatie die ik heb. In PLM lijken ook geen stevige profielen aanwezig te zijn. Dus moet ik mijn eigen profiel ontwerpen wat met een van de T-nuts uit PLM (4191347) te verbinden is aan de extrusie:
![[Pasted image 20251201155411.png]]
Ik wil dit onderdeel verder ondersteunen door ook twee Flange bracket connections (4176705)op de kop van het borstel frame te plaatsen. Deze moet wel aangedraaid worden voordat het hoekprofiel word geplaatst ![[Pasted image 20251201161318.png]]
### kunststof borstel
De situatie is als volgt:
![[Pasted image 20251201162930.png]]
rose+krieger levert hiervoor geen standaard oplossing waarvan ik vertrouw dat deze het volledige moment op kan vangen wat er op dit punt komt te staan. Tijdens ontwerp zie ik 2 opties om dit op te lossen:
- hoekprofiel eronder
- de 2 profielen aan de bovenkant verbinden
Ik wil gaan proberen om de 2 profielen aan de bovenkant te verbinden met een plaat waar deze beide ingeschroefd kunnen worden:![[Pasted image 20251201163743.png]]

De plaat mag maximaal 3mm dik zijn zodat de \#spindel van het systeem verwijderd kan worden

De plaat word aan het borstel frame verbinden met bouten direct in en frame. terwijl bij het frame gebruik wordt gemaakt van de stock bar materiaal van rose+kruger [[bl_aluprofilsystem_en.pdf#page=94|4006200 3010]] met M6 gatenm

Is ondertussen weer geupdate zodat deze de [[spindel lager]] kan ondersteurnen en een deel van het frame af te schermen #docu 

# afscherming-frame
Om het frame te ontwerpen is er niet voor elk onderdeel een morfologisch overzicht gemaakt. Er is een vooronderzoek rond extrusie profielen opties gedaan een er zijn [[frame concept|frame concepten]] gemaakt. Met dit begin is er begonnen met ontwerpen vanaf de overdekking aan de meeloopcenter kant.
#docu
## generale vormgeving
![[frame concept]]
## deuren
![[Klep scharnier]]
### dicht houden
![[ball catch]] 
### scharnier
![[deur scharnier]]
## kap
#WIP de kap is een keer verbeterd, maar deze veranderingen blijken niet doorgekomen te zijjn. Deze kap moet nu nog:
verbonden worden met bouten en gaten
### onderste kap scharnier
![[onderste kap scharnier]]
### bovenste scharnier kap
![[bovenste scharnier kap]]

### kap hendel
![[kap hendel]]
## profiel connectie
4006221 voor rechts grote stukken
## platen connects
![[bar material]]

# kosten
  ![[profielen tellen]]

- [[- definitie frame#Borstel frame|30x100]] (29, 30 en 32) #rose_kruger 
  $(815+125*2)*2+2*360=2850mm$  -> 3m
- [[- definitie frame#profiel keuze|staal boven 30x60]] (31) #rose_kruger 
  $245*2=490mm$ -> .5 m
-  30x30 #rose_kruger 
    totaal 24241.804 mm -> 25m
	  1. 485.668 mm
	  2. 485.668 mm
	  3. 1305.00 mm
	  4. 1335.00 mm
	  5. 485.668 mm
	  6. 1000.00 mm
	  7. 1000.00 mm
	  8. 670.000 mm
	  9. 750.000 mm
	  10. 1030.00 mm
	  11. 930.000 mm
	  12. 1060.00 mm
	  13. 335.000 mm
	  14. 515.668 mm
	  15. 640.000 mm
	  16. 640.000 mm
	  17. 515.668 mm
	  18. 273.000 mm
	  19. 1060.00 mm
	  20. 358.000 mm
	  21. 1273.00 mm
	  22. 182.668 mm
	  23. 1305.00 mm
	  24. 640.000 mm
	  25. 1305.00 mm
	  26. 298.400 mm
	  27. 298.400 mm
	  28. 273.000 mm
  
- [[- definitie frame#profielen verbinden|faceplate]] #rose_kruger 42925351
  2 stuks
- [[bl_aluprofilsystem_en.pdf#page=92|Bar material]] #rose_kruger 4006200 3010
  7045mm -> 7.5m nodig voor:
  - [[- definitie frame#geleiding frame verbinding|2xM6-30]] (en bij profiel 18) 
    5 stuks van 50 mm = 250mm bar materiaal
  - [[- definitie frame#kunststof borstel|4xM6-50]] 
    1x 180 mm
  - 3xM6-100
    23x 225mm = 5175mm bar materiaal
  - 2xM6-100
    12x 120mm = 1440 mm bar materiaal
- [[bl_aluprofilsystem_en.pdf#page=88|Slot stone -R-]] #rose_kruger 4006221
  155 stuks nodig ->160 stuks
- [[bl_aluprofilsystem_en.pdf#page=48|Flange bracket connection]] #rose_kruger 4306709
  41 stuks lotsize van 5 ->45 stuks 

- 8083431 #materiaal
  - 8083431_04
  - 8083431_06
  - 8083431_19
  - 8083431_20
  - 8083431_05
  - 8083431_15
  - 8083431_21
  - 8083431_10
  - 8083431_22
  - 8083431_14
  - 8083431_24
  - 8083431_25
  - 8083431_26
  - 8083431_27
  - 8083431_28
  - 8083431_29
  - 8083431_34
  - 8083431_35
  - 8083431_34
  - 8083431_33
- 8095576 #materiaal
  - 8095576_01
  - 8095576_02
  - 8095576_03
  - 8095576_04
  - 8095576_05

- geleiding 4080945 #PLM 

- hendel kap 020010 2x #PLM
  5.86/s
  11.72 euro
- hendel deur 3215565 #PLM
  2.52 euro
- ball catch 2x #rose_kruger 4010606
  2x
- scharnier deur #rose_kruger 4005525
  4x
- scharnier kap onder 091400315 2x #PLM
  10.97 p/s
  21.94 euro
- scharnier kap boven 090500347 #PLM
  2.22 p/s
  4.44 euro
