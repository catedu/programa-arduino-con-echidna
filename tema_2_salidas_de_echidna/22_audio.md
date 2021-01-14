## 2.2 MONTAJE 3 TIMBRE {#2-2-audio}

**RETO**
Queremos que hagas un programa en el Echidna que:
* Cuando se pulsa D2 suene una onda cuadrada de 282Hz o sea una duración 0.035 segundos (0.0175seg el bajo y 0.0175seg el alto).
* Si se pulsa el botón D3 que suene el tono C4 que es aproximadamente esa frecuenca.

**SOLUCIÓN**

%accordion%Solución%accordion%

La solución seguro que te sonará [pues lo hemos visto en el Tema 1](/tema_1_como_utilizar_echidna/12_como_se_programa_echidna_shield/124-mblock-vs-snap4arduino-cual-es-el-mejor/1247-importante-subir-a-arduino.md).

![](/assets/TnoC4.png)

%/accordion%

Si lo ejecutamos desde el ordenador, y pulsamos el botón D2 se oye un tut, tut, tut por los auriculares, ya dijimos en [este apartado](../tema_1_como_utilizar_echidna/12_como_se_programa_echidna_shield.md#1-2-4-7-subir-a-arduino) que la culpa lo tiene tu ordenador: No es capaz de enviar mBlock órdenes al Arduino a la velocidad de 0.00175 segundos. Si pulsamos el botón D3 se oye el tono C4 sin problemas.

La solución consiste en subir al arduino, ya lo hemos visto en el Tema 1 ¿no te acuerdas? vuelve a ver esta [presentación](https://docs.google.com/presentation/d/e/2PACX-1vTkh8pwo-b7LACnD7_ZAfWzYCchZI9H1_uR-tZqgfBRtOPFOaVDH8ognsCNEXA8khLI7UX6ziUQXZsx/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000):

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vTkh8pwo-b7LACnD7_ZAfWzYCchZI9H1_uR-tZqgfBRtOPFOaVDH8ognsCNEXA8khLI7UX6ziUQXZsx/embed?start=false&;loop=false&;delayms=3000" frameborder="0" width="100%" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>




El resultado es este vídeo:

{% youtube %} https://www.youtube.com/watch?v=WbA8p_yC-90 {% endyoutube %}

Si pulsamos D2 el sonido es más agudo que pulsando D3 que corresponde a la nota C4 ¿por qué? porque la señal es cuadrada.

%accordion%Más explicación%accordion%

Los cálculos del tiempo de subida y bajada tiempo=0.00175s calculados [anteriormente](../tema_1_como_utilizar_echidna/12_como_se_programa_echidna_shield.md#1-2-4-1-instrucciones-espec-ficas-para-arduino) están bien hechos ¿por qué no reproduce bien el tono de la nota C4? por esto:

![](/images/image76.png)

No es lo mismo una onda analógica sinusoidal de 282 Hz que una onda digital cuadrada que es lo que se reproduce en la salida digital D10

¿Y por qué se oye más agudo? Vamos a fijarnos en una transición por ejemplo la de bajada de 5V a 0V ¿A qué se parece más esa transición?

![](/images/image15.png)

Evidentemente a la segunda, y esa pendiente tan vertical corresponde más a ondas agudas:

![](/images/image48.png)

Por lo tanto se oye más agudo, por eso es

Ya sé que el anterior razonamiento, si lo lee algún físico, le producirá un rechinar de dientes 

![](/images/image63.png)
[via GIPHY](https://giphy.com)

pues para los frikis: … la transformada Fourier de una onda cuadrada produce armónicos de orden superior, incluso infinitos si fuese perfecta..., ja!, pero es mejor ser simple que ser incomprensible.

%/accordion%

