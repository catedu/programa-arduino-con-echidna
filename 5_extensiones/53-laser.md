## 5.3. MONTAJE 15 ALARMA LASER {#5-3-laser}

Hemos visto anteriormente una entrada digital sencilla con el sensor IR, ahora vamos a ver una salida digital muy simple, buscando siempre la motivación en nuestros proyectos: El diodo Laser.

![](/assets/2017-12-25 07_35_11-Encender un diodo láser con Arduino.png)

Si quieres saber más de este componente, te recomendamos la página de [Luis Llamas](https://www.luisllamas.es/diodo-laser-arduino/).
Si tienes que comprar uno, te recomendamos que no sea superior a 5mW, pues puede dañar permanentemente la retina del ojo [[+info](https://cuidatuvista.com/punteros-laser-juguetes-ojos/)]. El modelo que te proponemos es de **1mW**, no obstante, prevendremos a los alumnos **a no enfocar a los ojos**.

**RETO**
Te proponemos que realices un programa para desactivar una **ALARMA LASER**.
* La alarma está protegida por un haz laser (que enfoca a nuestro querido [LDR del Echidna](/3_entradas_de_echidna/32_el_ldr_en_a5.md)), si se corta el haz la alarma suena.
* El disparo va a ser simulada en el ordenador, no queremos queremos que alertar a los vecinos, un sonido en el ordenador y en la pantalla una imagen en el ordenador.
* Para desactivar la alarma, pulsamos la tecla espacio, y nos pide introducir el código (tienes 10 segundos para darle más entusiasmo, sino se dispara), si has acertado, el laser se apaga y ya puedes entrar a tu lindo hogar.

 Luego vamos a no ponernos nerviosos para desactivar la alarma y mantener la serenidad.
 
  <iframe src="https://giphy.com/embed/29SqSyXlyO6WI" width="480" height="271" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/big-bang-theory-nervous-anxiety-29SqSyXlyO6WI">via GIPHY</a></p>
  
%accordion%SOLUCION%accordion%

**Conexiones** son sencillas, el laser al D4 por ejemplo y hay que tener maña para que apunte al LDR:

![](/assets/2017-12-25 08_23_01-Documento1 - Microsoft Word.png)

**El script que controla si se corta el haz laser que se dispare** es un condicional que lee el LDR en A5, mientras sea mayor que 900 es que tiene una intensidad de luz muy grande, es decir, le está enfocando el laser, la variable _PARACRONO _es en el caso de que se desactive la alarma, el laser se apagará luego que no se crea que se corta el haz. Si se corta el haz envía un mensaje _Booom _que lo leeran los demás scripts. Se aprovecha este script para ENCENDER EL LASER pin digital 4 alto:

![](/assets/laser1.png)

**El script que controla la desactivación de la alarma mediante código** es el siguiente. Si se acierta con el código secreto 666, se envía el mensaje _Ufff _al resto de scripts:

![](/assets/laser3.png)


**El script que desactiva la alarma** es cuando reciba el mensaje _Ufff _por lo tanto para el cronómetro y apaga el laser:

![](/assets/laser5.png)

**El script del tiempo** cuenta de forma descendente, y si finaliza envía el mensaje Boom al resto de scripts, sólo se para si PARACRONO=1

![](/assets/laser2.png)

El resto: esconder y mostrar scripts y disfraces se omiten por simplicidad, el programa lo puedes descargar desde el repositorio.

%/accordion%

El resultado es 

{% youtube %}https://www.youtube.com/watch?v=i282JU35m2k{% endyoutube %}

## OTRO RETO
Si se corta el haz, hay 10 segundos para desactivarlo con código, sino, se dispara.
No ponemos la solución ¡¡ponlo tú en [el muro](/muro.md) !!

Seguro que se te ocurren muchas ideas...

![](/assets/2018-02-08 14_08_51-Documento2 - Microsoft Word.png)










