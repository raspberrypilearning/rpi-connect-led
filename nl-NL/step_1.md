Om een LED op te laten lichten, moet je met deze componenten een circuit bouwen:

| Experimenteerbord                           | Mannetje-vrouwtje aansluitdraden         | LED                    | Weerstand                         | Voeding                                |
| ------------------------------------------- | ---------------------------------------- | ---------------------- | --------------------------------- | -------------------------------------- |
| ![experimenteerbord](images/breadboard.png) | ![mv-aansluitdraad](images/mfjumper.png) | ![LED](images/led.png) | ![weerstand](images/resistor.png) | ![raspberrypi](images/raspberrypi.png) |

Kijk eens naar je LED. Je zou moeten zien dat het ene pootje langer is dan het andere. Het lange pootje is de **positieve** aansluiting, ook wel de **anode** genoemd. Het moet altijd worden aangesloten op de positieve kant van een circuit. Het korte pootje is de **negatieve** aansluiting, de **kathode** genoemd. Het moet worden aangesloten op de negatieve kant. Een manier om dit te onthouden is om je voor te stellen dat er aan de lange poot iets is toegevoegd en dat aan de korte poot iets is weggehaald.

Je zult merken dat er LED's zijn met poten van dezelfde lengte. In dat geval is het positieve pootje het pootje waar de plastic rand van de LED rond is. Bij de negatieve poot, is de rand afgeplat, zoals in de onderstaande afbeelding.

![LED van dichtbij](images/LEDcloseup.png)

+ Duw de positieve poot van de LED in rij 1 van je experimenteerbord, dichtbij de linkerkant van de sleuf. Plaats de negatieve poot in rij 1 aan de andere kant van de sleuf.

+ Zoek nu je weerstand. Een weerstand heeft geen positieve of negatieve zijde, dus het maakt niet uit hoe je hem in het experimenteerbord plaatst. Duw één poot in dezelfde rij waarin de negatieve LED-poot zit, zodat deze wordt aangesloten op de LED. Duw de andere weerstandspoot in een andere vrije rij aan de rechterkant van het sleuf.

+ Neem nu een man-naar-vrouw-aansluitdraad en duw het mannelijke uiteinde in dezelfde rij als de LED, aan de linkerkant van de sleuf bij de positieve poot van de LED. Duw het vrouwelijke uiteinde op de **3V3** GPIO-pin.

Je circuit zou er ongeveer zo uit moeten zien:

![Circuit zonder aarde](images/ground-missing.png)

Verbind nu je componenten met de aarde (**GND**) GPIO-pin:

+ Zorg ervoor dat er spanning op je Raspberry Pi staat. Neem nog een man-naar-vrouw-aansluitdraad en duw het mannelijke uiteinde in dezelfde rij als de tweede poot van de weerstand, aan dezelfde kant van de sleuf. Duw vervolgens het vrouwelijke uiteinde op je **GND** pin. Je LED zou moeten oplichten!

![Circuit stroom loop](images/circuit-current-flow.gif)

Als jouw LED niet oplicht, probeer dan het volgende: 1) Controleer of jouw Raspberry Pi aan staat 2) Controleer of al je componenten stevig in het experimenteerbord zijn gedrukt 3) Controleer of je LED op de juiste manier is aangesloten 4) Zorg ervoor de poten van je componenten zich aan de juiste kant van de sleuf bevinden 5) Probeer een andere LED
