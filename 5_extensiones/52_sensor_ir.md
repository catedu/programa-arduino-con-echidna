## 5.2 Sensor IR {#5-2-sensor-ir}

Vamos a provechar las conexiones digitales que tiene Echidna preparado para conectar módulos exteriores, si te fijas está preparado para conectar fácilmente estos módulos pues facilita la alimentación, GND y el pin digital

![](/images/image33.png)

Hay muchos módulos para conectar, y todos tienen la misma configuración en sus pines : GND, + , I/O, donde I/O es el pin digital o analógico de entrada o salida, dependiendo del sensor, y como puedes ver en la figura, hay mucha variedad (busca en Internet sensores para Arduino)

![](/images/image8.png)

hay para  a empezar con uno sencillo de entrada digital que es muy útil: el sensor Infrarrojos

![](/images/image28.png)

Para ver más información de este sensor te recomendamos[ esta página.](https://www.google.com/url?q=https://www.luisllamas.es/detectar-obstaculos-con-sensor-infrarrojo-y-arduino/&sa=D&ust=1513946282923000&usg=AFQjCNEtRW_FHKpsxaNaGxRTg8LrhdXQUQ)

En el Echidna arriba a la izquierda tienes 3 conectores digitales a elegir, nosotros elegimos el primero D4 luego el pin OUT del sensor se conecta al D4, el resto en el mismo orden

![](/images/image45.png)

Nota: El potenciometro es para ajustar la sensibilidad

Nota: Hay sensores con 4 pines, que permiten alimentar el diodo IR de forma independiente, pero tienen un jumper que inutiliza el 4 para sólo utilizar los 3 pines.

Realizamos un pequeño programa muy fácil que detecta si hay un obstáculo o no:

![](/images/image26.png)

El resultado es

[https://www.youtube.com/watch?v=eSpKITeSonA&;feature=youtu.be](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DeSpKITeSonA%26feature%3Dyoutu.be&sa=D&ust=1513946282925000&usg=AFQjCNHjlWbMFvlr62AVWGNybIKFy9X8RQ)

.