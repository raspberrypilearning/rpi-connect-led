Για να ανάψεις μια λυχνία LED, πρέπει να δημιουργήσεις ένα κύκλωμα από αυτά τα εξαρτήματα:

| Πλακέτα δοκιμών                           | Καλώδια Αρσενικό-σε-Θηλυκό                         | Λυχνία LED                    | Αντίσταση                         | Παροχή ρεύματος                        |
| ----------------------------------------- | -------------------------------------------------- | ----------------------------- | --------------------------------- | -------------------------------------- |
| ![πλακέτα δοκιμών](images/breadboard.png) | ![καλώδιο αρσενικό-σε-θηλυκό](images/mfjumper.png) | ![Λυχνία LDE](images/led.png) | ![αντίσταση](images/resistor.png) | ![raspberrypi](images/raspberrypi.png) |

Ρίξε μια ματιά στη λυχνία LED σου. Θα πρέπει να δεις ότι ο ένας ακροδέκτης είναι μεγαλύτερος από τον άλλο. Ο μακρύς, είναι ο **θετικός** ακροδέκτης, και ονομάζεται επίσης και **άνοδος**. Πρέπει πάντα να συνδέεται με τη θετική άκρη ενός κυκλώματος. Ο κοντός, είναι ο **αρνητικός** ακροδέκτης, και ονομάζεται επίσης και **κάθοδος**. Πρέπει να συνδεθεί με την αρνητική άκρη. Ένας τρόπος να το θυμάσαι αυτό είναι να φανταστείς ότι ο μακρύς ακροδέκτης μοιάζει να του έχουν προσθέσει κάτι ενώ στον κοντό ακροδέκτη σαν να του έχουν αφαιρέσει κάτι.

You'll find that there are LEDs that have legs of the same length. In that case, the positive leg is the leg where the plastic edge of the LED is round. Where the negative leg is, the edge will be flattened, like in the image below.

![LED Closeup](images/LEDcloseup.png)

+ Push the positive leg of the LED into row 1 of your breadboard, close to the left side of the ravine. Place the negative leg into row 1 on the other side of the ravine.

+ Now find your resistor. A resistor is a non-polarised component, so it doesn’t matter which way around you put it into the breadboard. Push one leg into the same row that the negative LED leg is in, so it connects to the LED. Push the other resistor leg into any other free row on the right side of the ravine.

+ Now take a male-to-female jumper wire and push the male end into the same row as the LED, on the left side of the ravine near the LED's positive leg. Push the female end onto the **3V3** GPIO pin.

Your circuit should look a little like this:

![Circuit Missing Ground](images/ground-missing.png)

Now, connect your components to the ground (**GND**) GPIO pin:

+ Make sure that your Raspberry Pi is powered on. Take another male-to-female jumper wire and push the male end into the same row as the resistor’s second leg, on the same side of the ravine. Then push the female end onto your **GND** pin. Your LED should light up!

![Circuit Current Flow](images/circuit-current-flow.gif)

If your LED doesn’t light, try the following: 1) Check your Raspberry Pi is on 2) Check all your components are pushed firmly into the breadboard 3) Check your LED is the right way around 4) Make sure the legs of your components are on the right side of the ravine 5) Try another LED
