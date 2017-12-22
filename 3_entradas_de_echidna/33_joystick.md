## 3.3 Joystick {#3-3-joystick}

El Joystick está conectado a los pines A0 y A1 y su valor varía desde 100 hasta 1024. El pin A0 controla el eje X y el pin A1 el eje Y.

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

#### 3.3.2 Come bichos {#3-3-2-come-bichos}

No podemos dejar el Joystick sin hacer un videojuego !!

![](/images/image61.png)La siguiente RETO es mover un Sprite “Bat” con el Joystick para atrapar un Beetle

![](/images/image9.png) ![](/images/image60.png)

El bicho lo haremos mover bastante rápido y al azar en el eje Y para que lo tenga difícil Bat:

![](/images/image13.png)

Y bat tiene que moverse con el joystick

![](/images/image81.png)

Los valores de m y n lo hemos calculado con la [HOJA DE CÁLCULO](https://www.google.com/url?q=https://docs.google.com/spreadsheets/d/e/2PACX-1vTyASTvUIs_xsZ8c4RZOJ1sEstk4Cc6d--_Drne_U0o1_CXhgzxQkvZ4ZNYGLdKa2lrhLHDKmAwsKnK/pub?output%3Dxlsx&sa=D&ust=1513946282881000&usg=AFQjCNHOP0NNKMiqEjmSGaucO7Mi5EKLoQ) que comentamos anteriormente, los valores límites que hemos puesto son:

Para el eje X:

![](/images/image84.png)

Para el eje Y:

![](/images/image40.png)

Además hemos añadido la puntuación y el cambio de disfraz para que parezca que aletea:

![](/images/image10.png)

El resultado es:

[https://www.youtube.com/watch?v=VERfepEkNv8](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DVERfepEkNv8&sa=D&ust=1513946282883000&usg=AFQjCNH0OIDQrns2VTKR8FmqfVzW1miGqA)

Lo sé …. soy bastante malo !!

![](/images/image87.gif)