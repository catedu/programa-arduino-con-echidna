## 5.4 Ultrasonidos

Queremos poner un ejemplo de un sensor que tenga 4 pines, barato y que puede darnos mucho juego pues nos da información de la distancia en la que se encuentra un objeto.

![](/assets/ultrasonidos.png)

Funciona por eco entre la señal que se emite por Trg y la que se recibe por Echo y para su utilización requiere utilizar la fórmula de conversión de tiempo a espacio con la fórmula de la velocidad del sonido... tranqui !! no lo vamos a hacer, pues ya mBlock tiene una función especial para ello sin utilizar fórmulas y **nos da diréctamente la distancia en cm**, pero si quieres saber más sobre este sensor, te recomendamos la página de [Luis Llamas](https://www.luisllamas.es/medir-distancia-con-arduino-y-sensor-de-ultrasonidos-hc-sr04/):

![](/assets/ultrasonidosmblock.png)

Como se necesitan 4 pines, y las extensiones tienen 3 utilizaremos alguno libre.

**RETO RADAR LUMINOSO**
Realizar un programa que a medida que se acerque un objeto, se enciendan más luces, reutilizar el sprite del semáforo para visualizarlo.

%accordion%Solución%accordion%

El programa es simplemente recoger la distancia con la instrucción que hemos señalado antes.
La conexión que vamos a realizar entre los pines I/O de Echidna y el sensor ultrasonidos HC-SR04 va a ser:

* el D4 en Trig
* el D7 en Echo
* el '+' en Vcc
* el G en GND

Por lo tanto el programa es (sólo se visualiza una parte, el resto es continuar con las condiciones, hemos puesto de límites 50cm, 40cm, 30cm, 20cm y 10cm para ir encendiendo luces)

![](/assets/radarluminoso.png)

%/accordion%

El resultado es :
{% youtube %}https://www.youtube.com/watch?v=7s1LDSDaA_A&feature=youtu.be{% endyoutube%}

Los siguientes retos, aunque las imágenes se ve que no están hechos con Echidna, da igual, es simplemente conectar el trig y echo en los pines D4 y D7 del Echidna y utilizar la instrucción de _"lee el sensor ultrasónico trig pin 4 echo pin 7"_ (o utilizar otro orden o el D8 si te pones revelde y cambiar los números anteriores) **¿Te atreves a hacerlos todos ?**

<iframe src="https://giphy.com/embed/aCrRttmzK1jKo" width="480" height="394" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/yes-the-big-bang-theory-sheldon-cooper-aCrRttmzK1jKo">via GIPHY</a></p>

** RETO HINCAR UNA PELOTA **
Pon de sprite una pelota y que se hinche a medida que acercas un objeto al ultrasonidos.
[Solución](https://catedu.gitbooks.io/ensena-pensamiento-computacional-con-arduino/content/ultrasonidos.html)

**RETO PIANO INVISIBLE**

Que suene una nota según la distancia del objeto.
[Solución](https://catedu.gitbooks.io/ensena-pensamiento-computacional-con-arduino/content/piano_invisible_con_ultrasonidos.html)

**RETO RADAR CON INTERMITENCIA DE UN LED**

Cuanto más cerca está un objeto, más rápido un led se enciende y apaga.
[Solución](https://catedu.gitbooks.io/ensena-pensamiento-computacional-con-arduino/content/con_un_led.html)

**RETO SENSOR PARKING**

Cuanto más cerca está un objeto, más rápido suena un pitido intermitente
[Solución](https://catedu.gitbooks.io/ensena-pensamiento-computacional-con-arduino/content/con_altavoz_del_pc.html)



 
