# Gebruiksaanwijzing

### opladen / vervangen batterijen
1. Gebruik
Controleer voor gebruik: Controleer de batterij op schade, opgezwollen cellen of lekkages. Gebruik nooit een beschadigde batterij.
Aansluiten: Zorg dat de connectoren correct zijn aangesloten (let op de polariteit).
Spanningsbereik: Gebruik de batterij alleen binnen het spanningsbereik van 6,0 V - 8,4 V om overladen of diep ontladen te voorkomen.
2. Opladen
Lader: Gebruik uitsluitend een LiPo-compatibele oplader.
Instellingen: Stel de oplader in op 2S (7,4 V) en de aanbevolen laadstroom (max. 1C).
Veiligheid: Laad de batterij op in een LiPo-safe zak en plaats deze op een niet-brandbare ondergrond.
3. Opslag
Opslagspanning: Bewaar de batterij op een opslagspanning van 3,7 - 3,85 V per cel.
Plaats: Bewaar op een koele, droge plek, weg van warmtebronnen en direct zonlicht.

### Draadloze Communicatie met de Auto
De auto is uitgerust met een Bluetooth-module om draadloos te communiceren. Let op: deze module werkt uitsluitend met Android-apparaten. Apple-apparaten worden niet ondersteund. Voor de bediening heb je de app "Serial Bluetooth Terminal" nodig, die je kunt downloaden via de Google Play Store. Volg de onderstaande stappen om de auto in gebruik te nemen.

### Verbinding maken

Ga naar de Bluetooth-instellingen op je Android-toestel en verbind met de Bluetooth-module van de auto.
Open vervolgens de "Serial Bluetooth Terminal"-app en selecteer de gekoppelde module. Hiermee is de verbinding tot stand gebracht en kun je commando’s naar de auto sturen.
Kalibratie
Voor een correcte werking moet de auto gekalibreerd worden voordat deze gaat rijden. Dit is nodig om zwart en wit op het oppervlak goed te herkennen. Plaats de auto eerst op een zwart oppervlak en voer het commando calibrate black in via de app. Zet de auto daarna op een wit oppervlak en voer het commando calibrate white in. Zorg ervoor dat je de kalibratie uitvoert op hetzelfde soort oppervlak als waar de auto zal rijden, met nauwkeurige kleuren. Na deze stap is de auto klaar om te rijden.

### Commando’s voor bediening
Je kunt de auto bedienen met de volgende commando’s:

debug [on/off]: Toont of verbergt de huidige instellingen van de auto.
run: Start de auto (de auto begint te rijden).
stop: Stopt de auto onmiddellijk.
set cycle [µs]: Stelt de duur van een cyclus in (aanbevolen waarde: tweemaal de calculation time, te zien via debug).
set power [0..255]: Regelt het motorvermogen. Zet dit niet direct op de maximale waarde, anders zal de auto wheelies maken.
set diff [0..1]: Regelt het snelheidsverschil tussen rechte stukken en bochten. Een hogere waarde zorgt voor minder vertraging in bochten.
set kp [0..]: Bepaalt hoe agressief de auto stuurt. Te hoge waarden kunnen schokkerig rijgedrag veroorzaken.
set ki [0..]: Zorgt ervoor dat de auto meer bijstuurt naarmate de bocht langer duurt.
set kd [0..]: Corrigeert fouten bij kp; hoe groter de fout, hoe sterker de correctie.

### Aanbevolen instellingen
Voor stabiele prestaties wordt aangeraden de volgende parameters in te stellen:

Cycle time: 3000
Power: 72
Diff: 0.74
Kp: 20
Ki: 0
Kd: 0.90

### start/stop button
Locatie: Geplaatst op de bovenkant van de auto.
Werking: Druk eenmaal om de auto in te schakelen, druk opnieuw om deze uit te schakelen.
