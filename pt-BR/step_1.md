Para acender um LED, você precisa construir um circuito com estes componentes:

| Protoboard                           | Fios jumper macho-fêmea          | LED                    | Resistor                         | Componente de energia                  |
| ------------------------------------ | -------------------------------- | ---------------------- | -------------------------------- | -------------------------------------- |
| ![protoboard](images/breadboard.png) | ![jumpermf](images/mfjumper.png) | ![LED](images/led.png) | ![resistor](images/resistor.png) | ![raspberrypi](images/raspberrypi.png) |

Dê uma olhada no seu LED. Você deve reparar que uma perna é mais longa que a outra. A perna longa é a perna do **positivo**, e também chamado de **ânodo**. Deve sempre ser conectada no lado positivo de um circuito. A perna curta é a perna do **negativo**, chamada de **cátodo**. Ela precisa estar conectada no lado negativo. Uma maneira de lembrar isso é imaginar a perna longa como tendo algo acrescentado (+) e a perna curta como tendo algo retirado (-).

Você verá que existem LEDs com pernas do mesmo comprimento. Nesse caso, a perna do positivo é a perna em que a borda plástica do LED é redonda. Onde a perna do negativo está, a borda tem um chanfro (achatada), como na imagem abaixo.

![Close do LED](images/LEDcloseup.png)

+ Empurre a perna do positivo do LED para a linha 1 da sua protoboard, perto do lado esquerdo da fenda. Coloque a perna do negativo na linha 1 do outro lado da fenda.

+ Agora encontre seu resistor. Um resistor é um componente não polarizado, portanto, não importa em que sentido você o coloca na protoboard. Empurre uma perna na mesma linha em que a perna do negativo do LED está, para que ela se conecte ao LED. Empurre a outra perna do resistor para qualquer outra linha livre no lado direito da fenda.

+ Agora pegue um fio jumper macho-fêmea e empurre a extremidade macho na mesma linha do LED, no lado esquerdo da fenda, próximo à perna do positivo do LED. Empurre a extremidade fêmea para o pino GPIO **3V3**.

Seu circuito deve ficar assim:

![Circuito sem o terra](images/ground-missing.png)

Agora, conecte seus componentes ao pino GPIO terra (**GND**):

+ Verifique se o seu Raspberry Pi está ligado. Pegue outro fio jumper macho-fêmea e empurre a extremidade macho na mesma linha da segunda perna do resistor, no mesmo lado da fenda. Em seguida, empurre a extremidade fêmea para o pino **GND**. Seu LED deve acender!

![Fluxo da corrente no circuito](images/circuit-current-flow.gif)

Se o seu LED não acender, tente o seguinte: 1) Verifique se o Raspberry Pi está ligado 2) Verifique se todos os seus componentes estão firmemente pressionados na protoboard 3) Verifique se o LED está na orientação certa 4) Verifique se as pernas dos seus componentes estão do lado direito da fenda 5) Tente outro LED
