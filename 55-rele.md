### 5.5 Servo

El servo es un motor que podemos controlar el ángulo, hay diferentes clases, pero nos vamos a centrar en este que tiene un precio/calidad aceptable.

![](/assets/2018-01-08 13_40_36-Controlar un servo con Arduino.png)

Este servo se controlan con una salida digital, y se les indica el ángulo de giro, que puede ir desde 0º hasta 180ª (no permite otro márgen)

Aprende más sobre servos en esta página de [Luis Llamas](https://www.luisllamas.es/controlar-un-servo-con-arduino/)

La instrucción para los servos en mBlock es muy fácil, simplemente le indicamos en qué pin digital está conectado y el ángulo que deseamos:

![](/assets/servo2.png)

El resultado lo puedes ver en este vídeo, donde puedes observar que para valores límites 0º y 180º hace un poco de vibración pues trabaja forzado:

{% youtube%} https://www.youtube.com/watch?v=xZl9bXtVzto {% endyoutube%}