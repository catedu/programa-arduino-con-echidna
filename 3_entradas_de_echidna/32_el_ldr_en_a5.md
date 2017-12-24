## 3.2 El LDR en A5 {#3-2-el-ldr-en-a5}

Primero de todo ¿Qué es un LDR? Vamos a la Wikipedia:
![](/images/image90.png)

[Fotorresistor](https://www.google.com/url?q=https://es.wikipedia.org/wiki/Fotorresistor&sa=D&ust=1513946282856000&usg=AFQjCNFvI1f7-bBAKWj9CTQacixEY8dZBQ)

_Una fotorresistencia es un componente electrónico cuya resistencia disminuye con el aumento de intensidad de luz incidente. Puede también ser llamado fotorresistor, fotoconductor, célula fotoeléctrica o resistor dependiente de la luz, cuyas siglas, LDR, se originan de su nombre en inglés light-dependent resistor. Su cuerpo está formado por una célula fotorreceptora y dos patillas._

![](/images/image31.png)[More at Wikipedia (ES)](https://www.google.com/url?q=https://es.wikipedia.org/wiki/Fotorresistor&sa=D&ust=1513946282857000&usg=AFQjCNHqQ70Mh0qFolRehlc1CT1rUagwJQ)

Lo verás en el Echidna arriba un poco a la derecha, y está conectado a la entrada analógica del Arduino A5 y según [http://echidna.es/](https://www.google.com/url?q=http://echidna.es/&sa=D&ust=1513946282857000&usg=AFQjCNHYPnLWO872xrJi9_N6tiFHvLZv6Q) los valores van desde 20 en ausencia de luz, hasta 1.000 con mucha luz.



### 3.2.2 Semáforo luminoso {#3-2-2-sem-foro-luminoso}

RETO Vamos a reutilizar esfuerzos: reutilizar el semáforo visto en [esta sección](../tema_1_como_utilizar_echidna/12_como_se_programa_echidna_shield.md#1-2-1-programaci-n-gr-fica-con-mblock) pero vamos a hacer que se iluminen los colores según la luz:

| Semáforo | Luz |
| --- | --- |
| Todo apagado | Mucha oscuridad |
| Rojo | Oscuridad |
| Amarillo | Luz normal |
| Verde | Mucha luz |

SOLUCIÓN

Según nuestros límites medidos en el anterior programa fijamos nuestras propias fronteras para cumplir el enunciado (puedes poner otros valores parecidos):

| Semáforo | Luz | Límite inferior | Límite superior |
| --- | --- | --- | --- |
| Todo apagado | Mucha oscuridad | --- | 199 |
| Rojo | Oscuridad | 200 | 499 |
| Amarillo | Luz normal | 500 | 799 |
| Verde | Mucha luz | 800 | --- |

El programa sería el siguiente, donde hemos capturado los semáforos en los tres estados utilizando una linterna y nuestra mano para oscurecer el LDR:

![](/images/image68.png)

El resultado lo puedes ver en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DMX558VKV_pE&sa=D&ust=1513946282868000&usg=AFQjCNGfVxyWAIq0qEDJW3N48RafvkjefQ):

https://www.youtube.com/watch?v=MX558VKV_pE

### 

###  {#-0}

### 3.2.3 Tonos según LDR {#3-2-3-tonos-seg-n-ldr}

La RETO es la siguiente:

Realizar un programa que suene una nota diferente según la luz

Parece sencillo pero no lo es ¿por qué? Porque hay cambios de escala, el LDR nuestro trabaja con valores distintos al de las notas, por lo tanto hay que hacer UN CAMBIO DE ESCALA, y esto necesita un apartado diferente:

#### 3.2.3.1 Cambios de escala {#3-2-3-1-cambios-de-escala}

Nos encontramos que:

*   Los valores de entrada, es decir, el LDR trabaja con unos límites, que según hemos visto en [el apartado comprobar los límites](#3-2-1-comprobar-los-l-mites), el nuestro va de 108 a 982, llamaremos a esta variable de entrada X
*   Los valores de salida son los tonos,que mBlock trabaja con la norma americana (la europea es el típico DoReMiFaSol) y los americanos, son valores numéricos que van desde 48 hasta 72 (lo puedes comprobar con la instrucción “tocar nota” que está en Programas-Sonido). Llamaremos a la variable salida de notas Y:

![](/images/image67.png)

Problema: ¿cómo convertimos X en Y?

Matemáticamente es una recta con una pendiente m y una ordenada n :

Y = m*X + n

Para calcular m y n tenemos que utilizar un sistema de ecuaciones dadas las condiciones límites de X e Y:

*   Cuando X = 108 quiero que Y valga 48: 48=m*108 + n
*   Cuando X = 982 quiero que Y valga 72: 72=m*982 + n

Ala! calcula m y n

![](/images/image11.png)

Buen ejercicio para los alumnos para que vean matemáticas aplicadas

No obstante, como esto lo repetiremos muchas veces los cambios de escala, hemos confeccionado [ESTA HOJA DE CÁLCULO](https://www.google.com/url?q=https://docs.google.com/spreadsheets/d/e/2PACX-1vTyASTvUIs_xsZ8c4RZOJ1sEstk4Cc6d--_Drne_U0o1_CXhgzxQkvZ4ZNYGLdKa2lrhLHDKmAwsKnK/pub?output%3Dxlsx&sa=D&ust=1513946282873000&usg=AFQjCNG67xpZIAuP9snBWW1bar7eOxSF9g) que te lo puedes descargar y facilita las cosas: Ponemos en las celdas amarillas los valores límites :

*   X1= 108 X2=982
*   Y1=48    Y2=72

Y nos da los valores m y n automáticamente:

![](/images/image46.png)

Luego la fórmula para el cálculo de la Y (las notas) en función de la luminosidad X es:

Y = 0.027 * X + 45

#### 3.2.3.2 Solución {#3-2-3-2-soluci-n}

El programa es pues el siguiente

![](/images/image30.png)

¿por qué lo hacemos con la opción de subir a Arduino? Ya l[o tendrías que saber.](../tema_1_como_utilizar_echidna/12_como_se_programa_echidna_shield.md#1-2-4-7-subir-a-arduino)

El resultado lo puedes ver en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Db7SSXn4q8WM&sa=D&ust=1513946282874000&usg=AFQjCNEfV2QXm1N1OLCI8H4wj6eCu5ejVg):

[https://www.youtube.com/watch?v=b7SSXn4q8WM](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Db7SSXn4q8WM&sa=D&ust=1513946282875000&usg=AFQjCNEFIbUNPNDhSBEVwesaa_IgLbR0Cw)