
Doel: Het vertalen van multidimensionale chaos en dynamische ruimtetijd naar een leesbare, cyclische en interactieve data-interface door middel van complexe analyse, topologie en ruimtelijke projecties.
1. Introductie

De VORTEX-architectuur is gebouwd op het snijvlak van discrete wiskunde, complexe analyse en topologie. Om een onafgebroken, oneindige datastroom (zoals de iteraties van de 64 hexagrammen) en 4D-ruimtetijd te kunnen visualiseren zonder randen of vastlopers, maakt het systeem gebruik van specifieke wiskundige transformaties. Geïnspireerd door de geometrische illusies van M.C. Escher, "vouwt" VORTEX de data op tot gesloten, navigeerbare constructies.
2. Het Domein van Complexe Getallen en de Riemannbol

Om de beperkingen van standaard lineaire waarden te overstijgen, opereert de kern van de datatransformatie binnen het complexe domein (C).

    Complexe Basis: De wiskunde vereist het gebruik van imaginaire getallen voor operaties met negatieve wortels: −1​=i. Complexe getallen nemen de vorm aan van a+bi.

    De Stereografische Projectie (σN​): Om te voorkomen dat functies met meerdere uitkomsten (multi-valente functies) onoverzichtelijk worden, wordt het oneindige platte vlak geprojecteerd op een 3D-sfeer (de Riemannbol, of S2).

        Formule voor projectie op het equatoriale 2D-vlak (R2)
    

        Toepassing in VORTEX: Deze logica vormt de basis van de project4Dto2D-functies in de shaders (GLSL). Het reduceert oneindigheid tot één gedefinieerd referentiepunt (de 'noordpool' van de bol), waardoor we 4D-hyperruimtes via een 3D-perspectief op een 2D-scherm kunnen weergeven.

3. Quaternionen ter Voorkoming van Gimbal Lock

Wanneer het complexe 2D-vlak onvoldoende is voor 3D- en 4D-rotaties (zoals bij de geanimeerde tesseract), wordt het domein uitgebreid.

    Wiskundige Definitie: Quaternionen vormen een vierdimensionale uitbreiding van de complexe getallen


    Toepassing in VORTEX: Door rotaties in de VORTEX-ruimte als quaternionen te berekenen, vermijdt de architectuur gimbal lock (het verlies van een rotatiegraad wanneer assen parallel komen te staan). Dit garandeert een vloeiende, ononderbroken navigatie door de multidimensionale data.

4. Minkowski-Ruimtetijd en Möbius-transformaties

Het VORTEX-dashboard verwerkt niet alleen ruimtelijke, maar ook temporele data (dynamische ruimtetijd).

    Isomorfisme met de Lorentz-groep: De wiskundige operaties die we op de Riemannbol uitvoeren (uitrekken, roteren, transleren) behoren tot de groep PSL(2,C). Deze is wiskundig identiek aan de Lorentz-groep SO+(1,3).

    De Minkowski-Zandloper: De transformaties op de Riemannbol modelleren direct de manier waarop objecten bewegen door de Minkowski-ruimtetijd (de lichtkegel die verleden en toekomst scheidt).

    Toepassing in VORTEX: Hierdoor kan tijd als een ruimtelijke coördinaat op het raster worden geprojecteerd.

5. Torus-Topologie (S1×S1) en Cyclische Iteratie

Terwijl de Riemannbol ideaal is voor ruimtelijke projectie en het vangen van de uitersten (oneindig), vereist het cyclische karakter van de data (zoals de I Tjing hexagrammen) een structuur zonder einde of top.

    Van Vlak naar Lus: Binnen de complexe analyse kan een vlak via een periodiek rooster (Λ) worden 'opgerold' tot een Torus.

    Twee Dimensies van Iteratie: De Torus vertegenwoordigt het product van twee cirkels (S1×S1).

    Toepassing in VORTEX: De Torus fungeert als de logische 'drager' van de datalussen.

        Cirkel 1 (Tijd): Zorgt voor de oneindige iteratielus, waarbij data cyclisch doorstroomt zonder ooit de rand van het systeem te bereiken.

        Cirkel 2 (Inhoud): Vertegenwoordigt de overlappende waarden, zoals de 64 hexagrammen.

        De naadloze inbedding van de datastromen op deze torus-topologie resulteert in het stabiel en synchroon draaien van het hele dashboard-ecosysteem.

Samenvatting van de Pijpleiding

    Data Invoer: Inkomende hexagram-cycli en temporele coördinaten.

    Transformatie (Quaternionen): 4D-berekeningen voeren naadloze rotaties uit op de datastructuur.

    Cyclische Binding (Torus): De datapunten worden in een oneindige topologische lus (S1×S1) geplaatst.

    Projectie (Riemannbol/Stereografisch): De N-dimensionale staat wordt met de functie σN​ vanuit de projectiepool teruggebracht naar een observeerbaar 2D/3D-vlak voor de interface.
