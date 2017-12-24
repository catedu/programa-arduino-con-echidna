**RETO**
Vamos a realizar el mismo ejemplo que [este vídeo de Jorge Lobo](https://www.google.com/url?q=https://www.youtube.com/watch?time_continue%3D8%26v%3DHx5DjQw7e_U&sa=D&ust=1513946282876000&usg=AFQjCNE8mVVKkIwRF0D-0kQn9ojW4gK_hQ) pero en vez de realizado en Snap4Arduino lo vamos a hacer en mBlock.

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

El resultado lo puedes ver en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DJzyd5cPb2-Y&sa=D&ust=1513946282878000&usg=AFQjCNELr1CkYreRS69YLd78fvl_qi0HUA):

{% youtube %} https://www.youtube.com/watch?v=Jzyd5cPb2-Y{% endyoutube %} 


Por curiosidad puedes ver el mismo programa en **Snap4Arduino **en este vídeo:

{% youtube %} https://www.youtube.com/watch?v=Jzyd5cPb2-Y{% endyoutube %} 

Puedes ver que es mucho más rápido que mBlock.

El programa lo puedes abrir en Snap4Arduino desde [este enlace](https://www.google.com/url?q=http://snap4arduino.org/run%23present:Username%3Djavierquintana%26ProjectName%3Dtelesketch-bueno&sa=D&ust=1513946282879000&usg=AFQjCNFYQVyMwX5ojtqgA0dutS5-GDGQdw).

{% youtube %} https://www.youtube.com/watch?v=j1lsYq6X5-U{% endyoutube %} 

