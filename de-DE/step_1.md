Um eine LED leuchten zu lassen, musst du eine Schaltung aus folgenden Komponenten erstellen:

| Steckbrett                           | Überbrückungsdrähte männlich - weiblich | LED                    | Widerstand                         | Stromquelle                            |
| ------------------------------------ | --------------------------------------- | ---------------------- | ---------------------------------- | -------------------------------------- |
| ![Steckbrett](images/breadboard.png) | ![m-w Drähte](images/mfjumper.png)      | ![LED](images/led.png) | ![Widerstand](images/resistor.png) | ![RaspberryPi](images/raspberrypi.png) |

Schau dir deine LED an. Du solltest sehen, dass ein Bein länger ist als das andere. Das lange Bein ist das **positive** Bein und wird auch ** Anode** genannt. Es sollte immer an die positive Seite eines Stromkreises angeschlossen werden. Das kurze Bein ist das ** negative ** Bein, genannt ** Kathode **. Es muss mit der negativen Seite verbunden werden. Eine Möglichkeit, sich daran zu erinnern, besteht darin, sich vorzustellen, dass dem langen Bein etwas hinzugefügt wurde und dem kurzen Bein etwas weggenommen wurde.

Du wirst feststellen, dass es LEDs mit gleich langen Beinen gibt. In diesem Fall ist das positive Bein das Bein, an dem die Kunststoffkante der LED rund ist. Wo sich das negative Bein befindet, wird der Rand abgeflacht, wie im Bild unten.

![LED-Details](images/LEDcloseup.png)

+ Stecke das positive Bein der LED in die Reihe 1 deines Steckbretts nahe der linken Seite der Mittellinie. Stecke das negative Bein in Reihe 1 auf der anderen Seite der Mittellinie.

+ Nimm jetzt deinen Widerstand. Ein Widerstand ist eine nicht polarisierte Komponente, daher spielt es keine Rolle, in welche Richtung du ihn in das Steckbrett steckst. Stecke ein Bein in dieselbe Reihe, in der sich das negative LED-Bein befindet, damit es mit der LED verbunden ist. Stecke das andere Widerstandsbein in eine andere freie Reihe auf der rechten Seite der Mittellinie.

+ Nimm nun ein männlich zu weiblich Überbrückungskabel und stecke das männliche Ende in die gleiche Reihe wie das positive Bein der LED auf der linken Seite der Mittellinie. Schiebe das weibliche Ende auf den **3V3** GPIO-Pin.

Deine Schaltung sollte ungefähr so aussehen:

![Stromkreis ohne Masseverbindung](images/ground-missing.png)

Verbinde nun deine Komponenten mit einem Masse-Anschluß (** GND **):

+ Stelle sicher, dass dein Raspberry Pi eingeschaltet ist. Nimm ein weiteres Stecker-zu-Buchse-Kabel und schiebe das männliche Ende in dieselbe Reihe wie das zweite Bein des Widerstands auf derselben Seite der Mittellinie. Schiebe das weibliche Ende auf den Masse-Anschluß ** GND **. Deine LED sollte aufleuchten!

![Stromfluss](images/circuit-current-flow.gif)

Wenn deine LED nicht leuchtet, versuche Folgendes: 1) Überprüfe, ob dein Raspberry Pi eingeschaltet ist. 2) Überprüfe, ob alle deine Komponenten fest in das Steckbrett eingedrückt sind. 3) Überprüfe, ob deine LED richtig herum eingesteckt ist. 4) Vergewissere dich, dass die Beine deiner Komponenten sich auf der richtigen Seite der Mittellinie befinden. 5) Versuche es mit einer anderen LED
