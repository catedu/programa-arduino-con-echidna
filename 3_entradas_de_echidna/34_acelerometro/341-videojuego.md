### MONTAJE 9 HELICOPTERO

**RETO**

Vamos a realizar un sencillo videojuego: Mover un helicóptero, el movimiento de un sprite con el acelerómetro y esquivando edificios que se mueven de derecha a izquierda dando la sensación de que el helicóptero vuela.

El reto te lo complicamos con dos premisas:
* Reutiliza el "sprite" edificio copiándotelo desde [Scratch](https://scratch.mit.edu/)
* El helicóptero explota si choca con un edificio

%accordion%Solución sprite helicóptero moviéndose según acelerómetro%accordion%

El sprite lo vamos a seleccionar de la biblioteca: Helicopter y le vamos a añadir otro disfraz que sea una explosión:

![](/images/image82.png)

, la manera más sencilla es elegir otro disfraz de la biblioteca, por ejemplo sol, y borrar la cara feliz que tiene:

![](/images/image6.png)

Vamos a hacer que se mueva según el acelerómetro:

Posición X: La pantalla de mBlock tiene desde -240 hasta 240 y hemos visto que los márgenes de A2 del acelerómetro va desde 250 hasta 500 luego hacemos el cambio de escala con la [HOJA DE CÁLCULO](https://docs.google.com/spreadsheets/d/e/2PACX-1vTyASTvUIs_xsZ8c4RZOJ1sEstk4Cc6d--_Drne_U0o1_CXhgzxQkvZ4ZNYGLdKa2lrhLHDKmAwsKnK/pub?output%3Dxlsx) que comentamos anteriormente:

![](/images/image22.png)

luego la fórmula para la posición X es (creando una variable que se llame POSX) :

![](/images/image24.png)

E igualmente para la posición Y pero en este caso los márgenes de la pantalla van desde -180 a 180 luego:

![](/images/image7.png)

luego la fórmula para la posición Y es (creando una variable que se llame POSY):

![](/images/image42.png)

El programa para el helicóptero es:

![](/images/image65.png)

%/accordion%

%accordion%Solución edificio, cómo se reutiliza un sprite%accordion%

Reutilizamos un poco: Nos copiamos un Sprite.

Vamos a copiar un poco el código de otra persona: Vamos a [scratch](https://scratch.mit.edu/)

Y seguimos [estos pasos](https://docs.google.com/presentation/d/e/2PACX-1vQU1KCgFxkeWMPgMhi9AhXU6MXlHNc5nO9yrjd2qIOzcNMpWsW_zDiunPCmH-kRl8D3T3iFTKXysuPl/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000)

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQU1KCgFxkeWMPgMhi9AhXU6MXlHNc5nO9yrjd2qIOzcNMpWsW_zDiunPCmH-kRl8D3T3iFTKXysuPl/embed?start=false&;loop=false&;delayms=3000" frameborder="0" width="100%" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

%/accordion%

%accordion%Solución a la muerte del helicóptero%accordion%


Vamos a poner que si toca un edificio, “explota” (o sea, cambia el disfraz a explosión), además envía el mensaje “you died” que vemos que el script del edificio lo necesita para esconderse una vez terminado el juego:

![](/images/image25.png)

%/accordion%

El resultado se puede ver en este vídeo:

{% youtube %} https://www.youtube.com/watch?v=aMY6qiib-Bc&;feature=youtu.be{% endyoutube %} 


**MEJORAS**

Ya sé que colocando el helicóptero siempre arriba, siempre ganas!!

<iframe src="https://giphy.com/embed/f79OYWh5uwIfK" width="100%" height="270" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/cbs-f79OYWh5uwIfK">via GIPHY</a></p>

Te propongo que añadas además de los edificios, unos pájaros que tengan el mismo comportamiento pero que aleatoriamente aparezcan a diferente altura, para complicar un poco la vida del helicóptero.

