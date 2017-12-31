## Alimentacion USB: {#nota-con-la-alimentacion-USB}

El Echidna **normalmente se alimenta a través de la alimentación USB **del Arduino, ya sea cuando está conectado con el ordenador, o cuando se utiliza un PowerBank por ejemplo, o cargador de móvil (esto ocurre cuando Arduino tiene el programa grabado en él y puede vivir sin el ordenador).

![](/images/image43.jpg)

Lo que hay que hacer es que el jumper que tiene arriba a la izquierda tenerlo conectado a 5V:

![](/assets/2017-12-24 17_09_04-Documento1 - Microsoft Word.png)

**No utilizar la alimentación 5V cuando los [servos o dispositivos](/5_extensiones/README.md) a controlar consuman más de 300mA**, para no sobrepasar el regulador del Arduino, en este caso utilizar la alimentación externa:

## Alimentacion externa: {#nota-con-la almentacion-externa}

Arduino se puede alimentar con un portapilas o fuente de alimentación, sin ningún problema, con un rango desde 9V hasta 12V.

![](/images/image5.png)

Pero hay que decirle al Echidna que la alimentación no es por 5V sino por **Vin**, pues el Arduino también se alimenta por Vin, esto se hace cambiando el jumper:

![](/images/image69.png)

**Nota**:

Es posible que en ocasiones nos interese utilizar **las dos alimentaciones a la vez**, por ejemplo queremos usar el Arduino dependiendo del ordenador, porque queremos por ejemplo que interactue con el _Sprite oso panda del mBlock_ (por lo tanto está conectado al cable USB) pero _las extensiones que queremos conectar necesitan potencia _(más de 300mA) por lo tanto conectamos también un portapilas o fuente de alimentación, así pues estamos obligados de decirle al Echidna que alimente las extensiones por Vin cambiando el jumper a Vin.



