## 1.2 Cómo se programa Echidna Shield {#1-2-c-mo-se-programa-echidna-shield}

Tenemos dos opciones:

*   Programación **mediante lenguajes gráficos**: símbolos, gráficos… tipo [Scratch](https://scratch.mit.edu)
    *   **Ventajas**: Mucho más sencillo e intuitivo, ideal para principiantes, primaria y secundaria.
    *   **Inconvenientes**: No se llega a aprovechar todas las posibilidades del Arduino. 
    ***Programas**: [Snap4Arduino](http://snap4arduino.rocks), [mBlock](http://www.mblock.cc), [ArduinoBlocks,](http://www.arduinoblocks.com) [Bitbloq](http://bitbloq.bq.com), [S4A](http://s4a.cat) 
*   Programación mediante **código**:
    *  ** Ventaja**: Se aprovecha todo el potencial de programación, puesto que se controla todas las variables
    *   **Inconvenientes**: Como toda programación en código, tiene su dificultad pues requiere una abstracción.
    *   **Programas**: [ArduinoIDE](https://www.google.com/url?q=https://www.arduino.cc/en/Main/Software&sa=D&ust=1513946282806000&usg=AFQjCNExOvtkBbrZbOR3YVDNnp8QfwtQIQ).

Cómo este curso trata del Echidna, que es una shield sencilla, nos decantamos por la programación mediante lenguajes gráficos, no obstante vas a ver las diferencias en el siguiente apartado.

Vamos a enseñarte tres formas de hacer el mismo programa: Un semáforo

Nota: Acuerdate en toda esta sección de poner la Echidna en modo Sensor

![](/images/image4.png)



### 1.2.3 Programación mediante código {#1-2-3-programaci-n-mediante-c-digo}

PRIMERO QUÉ ES

Es la forma de trabajar de forma profesional el Arduino: con su lenguaje código, en realidad, los otros lenguajes traducen el programa gráfico en lenguaje código Arduino, es decir son meros intermediarios.![](/images/image20.png)

El programa se puede descargar de su web oficial, aunque también hay una versión online [https://www.arduino.cc/](https://www.google.com/url?q=https://www.arduino.cc/&sa=D&ust=1513946282816000&usg=AFQjCNHa3tcU0VmaAnThGmZXHCiV-qpDug)

SEGUNDO LA CONFIGURACIÓN

Aquí no hay que instalar ningún Firmware, pues el código, o sea tú programa, es el mismo “firmware”. Digamos que no necesitas intermediarios si tratas con el agricultor ;)

TERCERO EL EJEMPLO SEMÁFORO CON CÓDIGO

Aquí es donde vemos que la programación no es apropiada para Primaria, y la explicación de cada línea necesitaría un curso entero. ([Como el que hay en Aularagón !](https://www.google.com/url?q=http://moodle.catedu.es/course/view.php?id%3D111&sa=D&ust=1513946282817000&usg=AFQjCNERjSWHukwxmzhifvfPZT29ynCGJw) ).

/* Semáforo Arduino  Leds conectados a pines 11,12,13 = EchidnaShield */int verde = 11;int amarillo = 12;int rojo = 13;void setup(){  pinMode(verde, OUTPUT);  pinMode(amarillo, OUTPUT);  pinMode(rojo, OUTPUT);  Serial.begin(9600); //inicializa la comunicación Serial}void loop(){  Serial.println("Semaforo - Inicio"); //Escribe el texto digitalWrite(verde, HIGH);  Serial.println("Semaforo - Verde"); //Escribe el texto  delay(2000);  digitalWrite(verde, LOW);  digitalWrite(amarillo, HIGH);  Serial.println("Semaforo - Amarillo"); //Escribe texto  delay(1000);  digitalWrite(amarillo, LOW);  digitalWrite(rojo, HIGH);  Serial.println("Semaforo - Rojo"); //Escribe el texto  delay(2000);  digitalWrite(rojo, LOW);}

Este programa se escribe (o copia y pega ¡es un texto !!) en el software del Arduino y se carga en la placa, en[ el vídeo](https://www.google.com/url?q=https://youtu.be/S8dQdCqOtto&sa=D&ust=1513946282823000&usg=AFQjCNHMu_skH6o86eJWChPi0zjmOX5ymw) se ve muy bien:

[https://www.youtube.com/watch?v=S8dQdCqOtto&;feature=youtu.be](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DS8dQdCqOtto%26feature%3Dyoutu.be&sa=D&ust=1513946282823000&usg=AFQjCNH1vbkAMxxBIb6hP4KZY9w_2Qdwag)

En este programa queremos que te fijes en una desventaja: La interacción con el ordenador se pierde frente a mBlock y Snap4Arduino:

*   En los lenguajes gráficos, tenemos a interacción con el ordenador igual que en Scratch: si te fijas en la pantalla el dibujo del semáforo va cambiando de disfraz para representar los colores de la luz que se enciende a la vez que en el Arduino.
*   En un programa grabado en el Arduino perdemos esa interacción, lo máximo que podemos visualizar es una ventana donde se representa en formato texto qué es lo que le está pasando al Arduino (en el ejemplo del semáforo sale "Semáforo - Verde, Semáforo- Rojo ….")(en realidad, con programación muy muy avanzada sí que se podría pero no vamos a entrar en estos jaleos).

Esto lo vemos como una desventaja desde el punto de vista de la enseñanza de la programación pues perdemos el potencial de interactuar con los elementos del ordenador crear personajes, disfraces, sonidos, teclado….

Pero… (siempre hay un “pero” para estropear la fiesta) la programación en código tiene una ventaja: Se graba en el Arduino, no utiliza de intermediario entre nuestro programa y el Arduino el ordenador, quien manda en el Arduino es nuestro programa, no nuestro ordenador, esto se traduce en: rapidez !, esto se soluciona en mBlock como lo veremos [más adelante](#1-2-4-7-subir-a-arduino).

Conclusión: Profesionalmente es mejor utilizar lenguaje con código pero en la enseñanza es mejor el lenguaje gráfico, además lo hemos dicho en el [apartado ¿Cómo se programa Echidna?](#1-2-c-mo-se-programa-echidna-shield) es una Shield Educativa que lo lógico es utilizar un lenguaje adaptado al nivel educativo: Gráfico. Pero … ¿cual?

###  {#-3}

###  {#-4}

### 1.2.4 mBlock vs Snap4Arduino ¿cuál es el mejor? {#1-2-4-mblock-vs-snap4arduino-cu-l-es-el-mejor}

Siempre es mejor moverse en estándares, actualmente está claro: el lenguaje basado en Scratch, y vamos a centrarnos en dos programas ¿Snap4Arduino o mBock?

![](/images/image73.png)

#### 1.2.4.1 Instrucciones específicas para Arduino {#1-2-4-1-instrucciones-espec-ficas-para-arduino}

Si entramos en la sección de instrucciones específicas para Arduino, en Snap4Arduino sólo tenemos las instrucciones básicas simples, a partir de estas piezas tienes que hacer el puzzle. Mientras que en mBlock tenemos más instrucciones que nos simplifican los programas pues la misma instrucción implican varias de las simples básicas:![](/images/image18.png)

![](/images/image58.png) 

Esto parece una tontería pero no lo es: por ejemplo, supongamos que queremos reproducir el tono C4 es más o menos 282Hz:

![](/images/image85.png)

Luego tiempo que dura la onda es =1/282 = 0.0035 segundos es decir el tiempo de “encendido HIGH” es 0.0035/2= 0.00175seg y el tiempo de “apagado LOW” es  0.0035/2= 0.00175seg.

o sea… que para hacer esta instrucción en mBlock

![](/images/image51.png)

necesitas hacer todo esto en Snap4Arduino :

![](/images/image16.png)

#### 1.2.4.2 Importación de librerías![](/images/image19.png) {#1-2-4-2-importaci-n-de-librer-as}

Snap4Arduino puede importar instrucciones o librerías que pueden aumentar el repertorio de instrucciones.

mBlock también tiene en Extensiones-Administrar extensiones pero no son tan específicas para el Arduino.

![](/images/image50.png)

#### 1.2.4.3 Formas de conexión con Arduino![](/images/image18.png) {#1-2-4-3-formas-de-conexi-n-con-arduino}

Vamos a fijarnos las diferentes posibilidades que tiene de conectarse el programa con el Arduino

![](/images/image47.png)

En Snap4Arduino hay que dar con el botón derecho en el sprite y sólo permite conexiones puerto serie.

Mientras que en mBlock hay un menú con la opción de Conexiones y diferentes caminos para conectarse: Puerto serie, Bluetooth, 2.4G ..

![](/images/image74.png)

#### 1.2.4.4 Reutilizar proyectos desde Scratch {#1-2-4-4-reutilizar-proyectos-desde-scratch}

![](/images/image55.png)

Si vemos un proyecto en Scratch que nos gusta y lo queremos reutilizar lo descargamos, y en mBlock lo podemos abrir, pero no siempre va bien.

Snap4Arduino no acepta ficheros Scratch, pero hay conversores online como [Snapin8r](https://www.google.com/url?q=http://hardmath123.github.io/Snapin8r/&sa=D&ust=1513946282830000&usg=AFQjCNGjVbyRXorjfBpa4SGIpnt1hODCIQ) más explicación en [esta página](https://www.google.com/url?q=http://codigo21.educacion.navarra.es/autoaprendizaje/snap4arduino-ventajas-instalacion-e-importacion-de-proyectos-de-scratch/&sa=D&ust=1513946282831000&usg=AFQjCNE3n062cljvcrnl3qqrTZAHkemzag), y también da problemas. Así que tortazo a los dos !!

Lo veremos mejor más adelante en[ esta sección](../3_entradas_de_echidna/34_acelerometro.md#3-4-2-reutilizamos-del-todo-copiamos-el-proyecto-de-otra-persona).

#### 1.2.4.5 Entorno amigable![](/images/image18.png) {#1-2-4-5-entorno-amigable}

En Snap4Arduino no existe un menú arriba, las opciones no se encuentran tan inmediatamente

![](/images/image62.png)

Mientras que en mBlock es más intuitivo:

![](/images/image70.png)

#### 1.2.4.6 Guardar en la nube y compartir![](/images/image19.png) {#1-2-4-6-guardar-en-la-nube-y-compartir}

Snap4Arduino permite grabar tus programas en la nube, esto es una gran ventaja, pues permite al alumnado estar en cualquier ordenador, y seguir trabajando con sus programas que están en su repositorio en Internet.

![](/images/image32.png)

Incluso puede grabar y compartir con otra persona el proyecto, (la otra persona recibe una copia del programa, no el original), esto permite publicar en un blog por ejemplo los programas.[Ver como.](https://www.google.com/url?q=https://youtu.be/rcnGCMbYJBY&sa=D&ust=1513946282833000&usg=AFQjCNGXgV9jzZl4seU-0Xb5F_OfSFdG8A)

mBlock sólo trabaja en modo local.

#### 1.2.4.7 Subir a Arduino {#1-2-4-7-subir-a-arduino}

En mBlock podemos poner la vista de Modo Arduino Y NOS MUESTRA NUESTRO PROGRAMA ESCRITO EN LENGUAJE GRAFICO CONVERTIDO A LENGUAJE CÓDIGO![](/images/image18.png)

Esto nos permite SUBIR AL ARDUINO es decir, nuestro programa grabarlo en el Arduino como si fuera un Firmware y ganar velocidad aquí tienes una captura y puedes observar cómo traduce el programa gráfico en código:

![](/images/image41.png)

El anterior programa funciona bien si lo hacemos subir al Arduino, pero si lo hacemos de forma normal (cambiamos el evento “Programa Arduino” por evento bandera):![](/images/image38.png)

NO FUNCIONA BIEN

¿por qué?: por la lentitud.

Si apretamos el pulsador 2 le pedimos al ordenador que encienda y apague D10 a una velocidad de 0.00175 segundos esto lo tiene que procesar el ordenador, pasa por el cuello de botella del puerto serie y al final se ejecuta en el Arduino a una velocidad mucho más baja, más o menos 0.5 segundos, en vez de oirse un tono, se oye tut,tut,tut,tut….

Si apretamos el pulsador 3 sí que se oye bien, porque mBlock manda el código del bucle de golpe para que se oiga bien.

Volveremos a este programa varias veces, no te preocupes si no lo has entendido del todo bien.

Desventajas de subir un programa al Arduino:

1.  NO PODEMOS INTERACTUAR CON EL ORDENADOR es decir, no podemos hacer que el sprite (el oso por defecto) se mueva o que al pulsar una tecla del ordenador… porque EL ARDUINO ES INDEPENDIENTE DEL ORDENADOR, incluso podemos desconectarlo y sigue funcionando !!!
2.  Nos hemos cargado el Firmware que tenía antes !! luego al finalizar tu programa, tenemos que volver a configurar el Arduino para que haga caso al programa mBlock visto en [esta presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vRLqEoJCT355xMCeCXsd0Wc7JcJRk9JkwLCyzEPb_h1S2IbYKK7OdUf33yWRIXq216Zgh9Da7-gIOq1/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282836000&usg=AFQjCNHZIx2i9Q4U-O15shd8SJobHkWsQA).

Ventajas de subir un programa al Arduino:

1.  Rapidez, tenemos la ventaja del lenguaje con código, el programa se ejecuta a la velocidad del Arduino sin tener el ordenador como intermediario.
2.  Independencia: Alimentamos el arduino con una batería ¡¡ y funciona !! esto es esencial para proyectos que impliquen movimiento y no queramos tener el ordenador encendido para que funcione.

#### 1.2.4.8 Rapidez en la simulación {#1-2-4-8-rapidez-en-la-simulaci-n}

Aunque Snap4Arduino no sube el programa, sólo simula es mucho más rápido en la simulación que mBlock![](/images/image19.png)

En[ este apartado](../3_entradas_de_echidna/33_joystick.md#3-3-1-telesketch) veremos las diferencias.

#### 1.2.4.8 And winner is … {#1-2-4-8-and-winner-is}

Nosotros le vamos a dar el premio a mBlock

![](/images/image79.png)

Todo es cuestión de gustos, las capturas y descargas de programas de este curso serán en mBlock, pero si te gusta Snap4Arduino puedes hacer este curso pero que tendrás que currarte [las instrucciones más elaboradas que tiene mBlock](#1-2-4-1-instrucciones-espec-ficas-para-arduino) y no podrás descargar tu programa al Arduino para que sea independiente [tal y como hace mBlock](#1-2-4-7-subir-a-arduino).

####  {#-5}

####  {#-6}

#### 1.2.4.9 Otros {#1-2-4-9-otros}

Existen otros programas gráficos, el ArduinoBlocks, Bitblock… pero no tienen la posibilidad de iteraccionar con Sprites del ordenador, ni tienen el mismo entorno del referente Scratch, por lo que no se utilizarán en este curso, pero son posibilidades interesantes, os mostramos dos capturas de pantalla del mismo programa semáforo visto anteriormente, fíjate que aquí no hay Sprite:

Con ArduinoBlocks:

![](/images/image91.png)

Con Bitblock:

![](/images/image12.png)