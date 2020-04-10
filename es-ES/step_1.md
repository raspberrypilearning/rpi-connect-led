Para encender un LED, necesitas construir un circuito con estos componentes:

| Placa de pruebas                           | Cable puente macho a hembra      | LED                    | Resistencia                         | Fuente de alimentación                 |
| ------------------------------------------ | -------------------------------- | ---------------------- | ----------------------------------- | -------------------------------------- |
| ![placa de pruebas](images/breadboard.png) | ![mfjumper](images/mfjumper.png) | ![LED](images/led.png) | ![resistencia](images/resistor.png) | ![raspberrypi](images/raspberrypi.png) |

Echa un vistazo a tu LED. Deberías ver que una patilla es más larga que la otra. La patilla más larga es el terminal **positivo**, también llamado **ánodo**. Siempre debe estar conectado al lado positivo de un circuito. La patilla más corta es el terminal **negativo**, también llamado **cátodo**. Necesita estar conectada al lado negativo. Una forma de recordar esto es imaginar que la patilla larga tiene algo añadido y a la patilla corta se le quitó algo.

Encontrarás que hay LEDs que tienen patillas de la misma longitud. En ese caso, la patilla positiva es donde el borde de plástico del LED es redondo. Donde está la patilla negativa, el borde estará plano, como en la imagen siguiente.

![LED de cerca](images/LEDcloseup.png)

+ Empuja la patilla positiva del LED en la fila 1 de tu placa de pruebas, en la parte izquierda de la hendidura cerca de ella. Coloca la patilla negativa en la fila 1 al otro lado de la hendidura del tablero.

+ Ahora busca tu resistencia. Una resistencia es un componente no polarizado, por lo que no importa en qué dirección lo coloques en la placa de pruebas. Empuja una patilla en la misma fila en la que se encuentra el terminal negativo del LED, para que se conecte al él. Empuja la otra patilla de la resistencia en cualquier otra fila libre en el lado derecho a la hendidura de la placa.

+ Ahora toma un cable de puente de macho a hembra y empuja el extremo macho en la misma fila que el LED, en el lado izquierdo de la hendidura de la placa, cerca de la patilla positiva del LED. Empuja el extremo hembra sobre el **3V3** Pin GPIO.

Tu circuito debería verse mas o menos así:

![Circuito sin Tierra](images/ground-missing.png)

Ahora, conecta tus componentes al pin de tierra (**GND**) GPIO:

+ Asegúrate de que tu Raspberry Pi esté encendida. Coge otro cable de puente de macho a hembra y empuja el extremo macho en la misma fila que el segundo terminal de la resistencia, en el mismo lado de la hendidura de la placa. Ahora empuja el extremo hembra sobre el pin **GND**. ¡Tu LED debería encenderse!

![Flujo de corriente del circuito](images/circuit-current-flow.gif)

Si tu LED no se enciende, intenta lo siguiente: 1) Verifica que tu Raspberry Pi esté encendida 2) Verifica que todos tus componentes estén firmemente insertados en el tablero 3) Verifica que tu LED esté en la posición correcta 4) Verifica que los terminales de tus componentes estén en el lado derecho de la hendidura del tablero 5) Prueba con otro LED
