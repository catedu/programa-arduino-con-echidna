### MONTAJE 7 TELESCKET

**RETO**
Vamos a realizar el mismo ejemplo que [este vídeo de Jorge Lobo](https://www.youtube.com/watch?time_continue%3D8%26v%3DHx5DjQw7e_U) pero en vez de realizado en Snap4Arduino lo vamos a hacer en mBlock.

{% youtube %}https://www.youtube.com/watch?time_continue=8&;v=Hx5DjQw7e_U{% endyoutube %}

%accordion%Solución%accordion%

El programa :

![](/images/image83.png)

simplemente vamos a comentar las condicionales principales:

*   Si A0 es menor que 300 es que estás inclinando el Joystick hacia la izquierda, luego el Sprite tiene que modificar su variable x hacia la derecha, es decir decrementando su valor

![](/images/image86.png)

*   Si A0 es mayor que 700 es seguro que estás inclinando el Joystick hacia la derecha luego hay que incrementar el valor de la ordenada X![](/images/image66.png)
*   Para los valores del eje Y es igual, cambiando A0 por A1

%/accordion%

**VA MUY LENTO**
El resultado lo puedes ver en [este vídeo](https://www.youtube.com/watch?v%3DJzyd5cPb2-Y):

{% youtube %} https://www.youtube.com/watch?v=Jzyd5cPb2-Y{% endyoutube %} 


Por curiosidad puedes ver el mismo programa en **Snap4Arduino **en este vídeo:

{% youtube %} https://www.youtube.com/watch?v=j1lsYq6X5-U{% endyoutube %} 

Puedes ver que es mucho **más rápido** que mBlock.

El programa lo puedes abrir en Snap4Arduino desde [este enlace](http://snap4arduino.org/run%23present:Username%3Djavierquintana%26ProjectName%3Dtelesketch-bueno).



