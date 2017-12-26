## Alimentacion USB: {#nota-con-la-alimentacion-USB}

El Echidna **normalmente se alimenta a través de la alimentación USB **del Arduino, ya sea cuando está conectado con el ordenador, o cuando se utiliza un PowerBank por ejemplo, o cargador de móvil (esto ocurre cuando Arduino tiene el programa grabado en él y puede vivir sin el ordenador).

![](/images/image43.jpg)

Lo que hay que hacer es que el jumper que tiene arriba a la izquierda tenerlo conectado a 5V:

![](/assets/2017-12-24 17_09_04-Documento1 - Microsoft Word.png)

## Alimantacion a pilas: {#nota-con-la almentacion-a-pilas}

Arduino se puede alimentar con un portapilas, sin ningún problema (también este caso es cuando está independiente del ordenador)

![](/images/image5.png)

Pero hay que cambiar en este caso el Echidna, hay que decirle que la alimentación no es por 5V sino por **Vin**, pues el Arduino también se alimenta por Vin, esto se hace cambiando el jumper, aunque realmente esto sólo es importante cuando se utilizan [las extensiones](/5_extensiones/README.md):

![](/images/image69.png)



