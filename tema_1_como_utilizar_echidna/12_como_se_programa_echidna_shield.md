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