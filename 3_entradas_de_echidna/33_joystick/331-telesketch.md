#### 3.3.1 Telesketch {#3-3-1-telesketch}

Vamos a realizar el mismo ejemplo que [este vídeo de Jorge Lobo](https://www.google.com/url?q=https://www.youtube.com/watch?time_continue%3D8%26v%3DHx5DjQw7e_U&sa=D&ust=1513946282876000&usg=AFQjCNE8mVVKkIwRF0D-0kQn9ojW4gK_hQ) pero en vez de realizado en Snap4Arduino lo vamos a hacer en mBlock

[https://www.youtube.com/watch?time_continue=8&;v=Hx5DjQw7e_U](https://www.google.com/url?q=https://www.youtube.com/watch?time_continue%3D8%26v%3DHx5DjQw7e_U&sa=D&ust=1513946282876000&usg=AFQjCNE8mVVKkIwRF0D-0kQn9ojW4gK_hQ)

El programa lo puedes descargar de este [repositorio](https://www.google.com/url?q=https://drive.google.com/drive/folders/1pXcRUqMM7q_UK0QhILd9QwLe8KtPCM5m?usp%3Dsharing&sa=D&ust=1513946282877000&usg=AFQjCNHvBDu7av9p014L6b9oESHXcDnQlA) 

![](/images/image83.png)

simplemente vamos a comentar las condicionales principales:

*   Si A0 es menor que 300 es que estás inclinando el Joystick hacia la izquierda, luego el Sprite tiene que modificar su variable x hacia la derecha, es decir decrementando su valor

![](/images/image86.png)

*   Si A0 es mayor que 700 es seguro que estás inclinando el Joystick hacia la derecha luego hay que incrementar el valor de la ordenada X![](/images/image66.png)
*   Para los valores del eje Y es igual, cambiando A0 por A1

El resultado lo puedes ver en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DJzyd5cPb2-Y&sa=D&ust=1513946282878000&usg=AFQjCNELr1CkYreRS69YLd78fvl_qi0HUA):

[https://www.youtube.com/watch?v=Jzyd5cPb2-Y](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DJzyd5cPb2-Y&sa=D&ust=1513946282878000&usg=AFQjCNELr1CkYreRS69YLd78fvl_qi0HUA)

Por curiosidad puedes ver el mismo programa en Snap4Arduino en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Dj1lsYq6X5-U&sa=D&ust=1513946282879000&usg=AFQjCNFNlwlvU3OQ0ivLV0zw-yYGtRC7LA) y verás que es mucho más rápido que mBlock. El programa lo puedes abrir en Snap4Arduino desde [este enlace](https://www.google.com/url?q=http://snap4arduino.org/run%23present:Username%3Djavierquintana%26ProjectName%3Dtelesketch-bueno&sa=D&ust=1513946282879000&usg=AFQjCNFYQVyMwX5ojtqgA0dutS5-GDGQdw).

https://www.youtube.com/watch?v=j1lsYq6X5-U

