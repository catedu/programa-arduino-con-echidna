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