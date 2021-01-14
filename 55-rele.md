### 5.5 Servo

El servo es un motor que podemos controlar el ángulo de giro, hay diferentes clases, pero nos vamos a centrar en este que tiene un precio/calidad aceptable, **el MG90S**.

![](/assets/2018-01-08 13_40_36-Controlar un servo con Arduino.png)

Este servo se controla con una salida digital, y se les indica el ángulo de giro, que puede ir desde 0º hasta 180ª (no permite otro márgen). Si elegimos otro más barato, puede tener deriva en los extremos ([ver vídeo con HD-144A](https://catedu.github.io/programa-arduino-mediante-codigo/montaje_1_testea_tu_servo.html))

Aprende más sobre servos en esta página de [Luis Llamas](https://www.luisllamas.es/controlar-un-servo-con-arduino/).

La instrucción para los servos en mBlock es muy fácil, simplemente le indicamos en qué pin digital está conectado y el ángulo que deseamos:

![](/assets/servo2.png)

y ponlo bien, el marrón indica la masa:

![](/assets/2018-02-10 09_22_49-Documento1 - Microsoft Word.png)

El resultado lo puedes ver en este vídeo, donde puedes observar que para valores límites 0º y 180º hace un poco de vibración pues trabaja forzado:

{% youtube%} https://www.youtube.com/watch?v=xZl9bXtVzto {% endyoutube%}

Mira la diferencia con un **servo de rotación continúa**, fíjate como:
- Los extremos 0º y 180º es a máxima velocidad, pero un sentido u otro.
- 90º es parado.
- Un valor intermedio es menos velocidad (se ve el ejemplo 80º y 100º)
- Si tiene deriva, (cosa frecuente) hay un potenciómetro para ajustar.

{% youtube %}https://www.youtube.com/watch?v=Z-5SerXmRY0&feature=youtu.be{% endyoutube %}



