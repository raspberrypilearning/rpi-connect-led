Aby zaświecić diodę LED, musisz zbudować obwód z tych elementów:

| Breadboard                           | Male-to-female jumper wires                  | LED                    | Resistor                         | Power component                        |
| ------------------------------------ | -------------------------------------------- | ---------------------- | -------------------------------- | -------------------------------------- |
| ![breadboard](images/breadboard.png) | ![przewód gniazdo-wtyk](images/mfjumper.png) | ![LED](images/led.png) | ![resistor](images/resistor.png) | ![raspberrypi](images/raspberrypi.png) |

Have a look at your LED. You should see that one leg is longer than the other. Długa nóżka jest**dodatnią**, jest także nazywana **anodą**. It should always be connected to the positive side of a circuit. Krótka nóżka jest**ujemną**, nazywana jest **katodą**. It needs to be connected to the negative side. One way to remember this is to imagine the long leg as having had something added and the short leg as having had something taken away.

You'll find that there are LEDs that have legs of the same length. In that case, the positive leg is the leg where the plastic edge of the LED is round. Where the negative leg is, the edge will be flattened, like in the image below.

![Zbliżenie diody LED](images/LEDcloseup.png)

+ Wciśnij dodatnią nóżkę diody LED w 1 rzędzie płytki stykowej, blisko lewej strony rowka. Umieść nóżkę ujemną w rzędzie 1 po drugiej stronie rowku.

+ Now find your resistor. A resistor is a non-polarised component, so it doesn’t matter which way around you put it into the breadboard. Push one leg into the same row that the negative LED leg is in, so it connects to the LED. Wepchnij drugą nogę opornika do dowolnego wolnego rzędu po prawej stronie rowku.

+ Teraz weź przewód połączeniowy męsko-żeński i wepchnij męski koniec do tego samego rzędu co dioda LED, po lewej stronie rowku w pobliżu dodatniej nogi LED. Wciśnij żeński koniec na pin**3V3** GPIO.

Your circuit should look a little like this:

![Circuit Missing Ground](images/ground-missing.png)

Now, connect your components to the ground (**GND**) GPIO pin:

+ Make sure that your Raspberry Pi is powered on. Take another male-to-female jumper wire and push the male end into the same row as the resistor’s second leg, on the same side of the ravine. Then push the female end onto your **GND** pin. Your LED should light up!

![Circuit Current Flow](images/circuit-current-flow.gif)

If your LED doesn’t light, try the following: 1) Check your Raspberry Pi is on 2) Check all your components are pushed firmly into the breadboard 3) Check your LED is the right way around 4) Make sure the legs of your components are on the right side of the ravine 5) Try another LED
