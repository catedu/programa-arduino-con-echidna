## 3.4 Acelerómetro {#3-4-aceler-metro}

El acelerómetro tiene el mismo efecto que el Joystick, nos da valores en el eje X o eje Y, en el caso del Joystick lo daba la inclinación de la palanca, en este caso lo da la inclinación del mismo Echidna.

Está conectado a los pines analógicos:

*   A2 nos da la inclinación en el eje X
*   A3 nos da la inclinación en el eje Y

Los valores van desde 250 hasta 500

#### 3.4.1 Videojuego {#3-4-1-videojuego}

Vamos a realizar un sencillo videojuego, el movimiento de un sprite con el acelerómetro y esquivando objetos.

##### 3.4.1.1 Helicóptero {#3-4-1-1-helic-ptero}

El sprite lo vamos a seleccionar de la biblioteca: Helicopter y le vamos a añadir otro disfraz que sea una explosión:

![](/images/image82.png)

, la manera más sencilla es elegir otro disfraz de la biblioteca, por ejemplo sol, y borrar la cara feliz que tiene:

![](/images/image6.png)

Vamos a hacer que se mueva según el acelerómetro:

Posición X: La pantalla de mBlock tiene desde -240 hasta 240 y hemos visto que los márgenes de A2 del acelerómetro va desde 250 hasta 500 luego hacemos el cambio de escala con la [HOJA DE CÁLCULO](https://www.google.com/url?q=https://docs.google.com/spreadsheets/d/e/2PACX-1vTyASTvUIs_xsZ8c4RZOJ1sEstk4Cc6d--_Drne_U0o1_CXhgzxQkvZ4ZNYGLdKa2lrhLHDKmAwsKnK/pub?output%3Dxlsx&sa=D&ust=1513946282885000&usg=AFQjCNFTLi5pX_fG-4CrveOTHPAb6tW1Ew) que comentamos anteriormente:

![](/images/image22.png)

luego la fórmula para la posición X es (creando una variable que se llame POSX) :

![](/images/image24.png)

E igualmente para la posición Y pero en este caso los márgenes de la pantalla van desde -180 a 180 luego:

![](/images/image7.png)

luego la fórmula para la posición Y es (creando una variable que se llame POSY):

![](/images/image42.png)

El programa para el helicóptero es:

![](/images/image65.png)

##### 3.4.1.2 Reutilizamos un poco: Nos copiamos un Sprite. {#3-4-1-2-reutilizamos-un-poco-nos-copiamos-un-sprite}

Vamos a copiar un poco el código de otra persona: Vamos a [scratch](https://www.google.com/url?q=https://scratch.mit.edu/&sa=D&ust=1513946282886000&usg=AFQjCNGamoaBekRsl8WkE6nz4l6rBODONg), elegimos un juego que tenga el sprite que nos interesa: por ejemplo éste (poniendo en su buscador ‘fly’) [https://scratch.mit.edu/projects/128227746/](https://www.google.com/url?q=https://scratch.mit.edu/projects/128227746/&sa=D&ust=1513946282886000&usg=AFQjCNFkit_qcC3-nq6jShgJOPQmkX-xBA)

Y seguimos [estos pasos](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vQU1KCgFxkeWMPgMhi9AhXU6MXlHNc5nO9yrjd2qIOzcNMpWsW_zDiunPCmH-kRl8D3T3iFTKXysuPl/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282887000&usg=AFQjCNERdSe7qnTWaGeNPvtdGL3Vz8aSGg)

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQU1KCgFxkeWMPgMhi9AhXU6MXlHNc5nO9yrjd2qIOzcNMpWsW_zDiunPCmH-kRl8D3T3iFTKXysuPl/embed?start=false&;loop=false&;delayms=3000" frameborder="0" width="100%" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

#### 3.4.1.3 Muerte del helicóptero {#3-4-1-3-muerte-del-helic-ptero}

Vamos a poner que si toca un edificio, “explota” (o sea, cambia el disfraz a explosión), además envía el mensaje “you died” que vemos que el script del edificio lo necesita para esconderse una vez terminado el juego:

![](/images/image25.png)

El resultado se puede ver en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DaMY6qiib-Bc%26feature%3Dyoutu.be&sa=D&ust=1513946282888000&usg=AFQjCNGCeX2xmm_K84bXIROob_sP_rBL0w)

[https://www.youtube.com/watch?v=aMY6qiib-Bc&;feature=youtu.be](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DaMY6qiib-Bc%26feature%3Dyoutu.be&sa=D&ust=1513946282888000&usg=AFQjCNGCeX2xmm_K84bXIROob_sP_rBL0w)

MEJORAS

Ya sé que colocando el helicóptero siempre arriba, siempre ganas!!

<iframe src="https://giphy.com/embed/f79OYWh5uwIfK" width="100%" height="270" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/cbs-f79OYWh5uwIfK">via GIPHY</a></p>

Te propongo que añadas además de los edificios, unos pájaros que tengan el mismo comportamiento pero que aleatoriamente aparezcan a diferente altura, para complicar un poco la vida del helicóptero.

#### 

####  {#-0}

#### 3.4.2 Reutilizamos del todo: Copiamos el proyecto de otra persona {#3-4-2-reutilizamos-del-todo-copiamos-el-proyecto-de-otra-persona}

Esta vez no vamos a ser originales, vamos a ser un poco vagos y nos vamos a copiar el programa de otra persona

![](/images/image78.png)

Vamos a buscar un programa de un videojuego y hacerlo que funcione con nuestro acelerómetro de la Echidna.

La [web de Scratch](https://www.google.com/url?q=https://scratch.mit.edu/&sa=D&ust=1513946282889000&usg=AFQjCNGygwtyuNaEEsxDNvVSFxX9GBVf1A) tiene un repositorio de millones de proyectos, podemos seleccionar uno, y adaptarlo a nuestra simpática Echidna. Vamos a ver un ejemplo con este proyecto [https://scratch.mit.edu/projects/29744/](https://www.google.com/url?q=https://scratch.mit.edu/projects/29744/&sa=D&ust=1513946282890000&usg=AFQjCNEWwHBWiXjFJuaLk0mMV7oYIQlLdQ)

##### 3.4.2.1 Reutilizando un proyecto con mBlock {#3-4-2-1-reutilizando-un-proyecto-con-mblock}

En [esta presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vSCDGNYTkUuXsIOtMJDozS3jijvI8ZgYk9cy50vpgvlCAUVZOZbLtTjynKjkZ_CHhq9nvJQzIefO9V2/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282890000&usg=AFQjCNHlGqrxqDlrGjo3EAQlihyYh5JcXw) se muestra cómo se importa un proyecto a mBlock:

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vSCDGNYTkUuXsIOtMJDozS3jijvI8ZgYk9cy50vpgvlCAUVZOZbLtTjynKjkZ_CHhq9nvJQzIefO9V2/embed?start=false&;loop=false&;delayms=3000" frameborder="0" width="100%" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

Una vez importando nos fijamos en el código que hay que modificar, está claro que lo que hay que tocar es el Sprite “Ship” que es el que queremos mover con el acelerómetro y modificar el “posicionX que se realiza con el ratón y cambiarlo por el acelerómetro:

![](/images/image44.png)

Perooo como siempre: la posición del ratón es la misma que las coordenadas de la pantalla de mBloc y la x va desde -240 hasta 240 y nuestro acelerómetro de A2 va desde 250 hasta 500 luego hacemos el cambio de escala con la [HOJA DE CÁLCULO](https://www.google.com/url?q=https://docs.google.com/spreadsheets/d/e/2PACX-1vTyASTvUIs_xsZ8c4RZOJ1sEstk4Cc6d--_Drne_U0o1_CXhgzxQkvZ4ZNYGLdKa2lrhLHDKmAwsKnK/pub?output%3Dxlsx&sa=D&ust=1513946282891000&usg=AFQjCNG-30BZx1eA-t1QqrwaNZvW04wknA) que ya lo hemos hecho con el [helicóptero](#3-4-1-1-helic-ptero) anteriormente:

![](/images/image24.png)

Y cambiamos el código:

![](/images/image37.png)

También vamos a cambiar el disparador “espacio” por pin digital 2 para disparar con el botón D2 del Echidna:

![](/images/image3.png)

El resultado en[ este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DPs3jB89KIg8%26feature%3Dyoutu.be&sa=D&ust=1513946282892000&usg=AFQjCNFBi0uZVxoLx2azVBPFTGbAaJ8gFw):

[https://www.youtube.com/watch?v=Ps3jB89KIg8&;feature=youtu.be](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DPs3jB89KIg8%26feature%3Dyoutu.be&sa=D&ust=1513946282892000&usg=AFQjCNFBi0uZVxoLx2azVBPFTGbAaJ8gFw)

##### 3.4.2.2 Reutilizando un proyecto con Snap4Arduino {#3-4-2-2-reutilizando-un-proyecto-con-snap4arduino}

Este programa para la simulación de proyectos grandes va más rápido por lo que vamos a ver como alternativa:

Para importar un proyecto desde Scratch es un poco más complicado, ver [esta presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vQ7PutZ1rJdylUGdaQ6qgkoofiQu1-t0inaBN5JN0idYOlvlK84qa1THTBzNUx4SW3kslXdjUdEs9NF/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282893000&usg=AFQjCNEVlBh7kkM1aLorDX-QmbsH9hplKw):

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQ7PutZ1rJdylUGdaQ6qgkoofiQu1-t0inaBN5JN0idYOlvlK84qa1THTBzNUx4SW3kslXdjUdEs9NF/embed?start=false&;loop=false&;delayms=3000" frameborder="0" width="100%" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

Los cambios en el código son los mismos que los anteriores. ![](/images/image89.png)

Recuerda que  e[n esta presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vQ7tr9aNDDuzFcEMFOepVVao5eCKWBBQh3U5emsy5oaN4a-Q8tNkYMWxKyma6xz-gBVL6nLLlmlWuPw/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282894000&usg=AFQjCNH_vEQY0Dj3hZ-FhPh4qoUqn2RKkw) se enseña cómo configurar Snap4Arduino para que se comunique con nuestro Arduino y la Echidna.

El programa lo puedes abrir en Snap4Arduino en esta [URL](https://www.google.com/url?q=http://snap4arduino.org/run%23present:Username%3Djavierquintana%26ProjectName%3DAlien%2520Invasion-MODIFICADO&sa=D&ust=1513946282894000&usg=AFQjCNF-EVqjqnW1UNgn7LgENVXRNCHhIg) 

El Sprite que tienes que conectar con Arduino es la nave esa con cuernos.

El resultado lo puedes ver en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Dec4q_5bbBQQ%26feature%3Dyoutu.be&sa=D&ust=1513946282895000&usg=AFQjCNH6g4-3XuX_dmITOzJaesmWmq3CPA):

[https://www.youtube.com/watch?v=ec4q_5bbBQQ&;feature=youtu.be](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Dec4q_5bbBQQ%26feature%3Dyoutu.be&sa=D&ust=1513946282895000&usg=AFQjCNH6g4-3XuX_dmITOzJaesmWmq3CPA)