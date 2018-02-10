## 5.1 MONTAJE 13 ENCENDER CON EL MÓVIL Bluetooth {#5-1-bluetooth} 

# ATENCION: MUY DIFICIL

### 5.1.1 Módulo HC-06 {#5-1-1-m-dulo-hc-06}

Echidna tiene un conector preparado para conectar un módulo de Bluetooth

![](/images/image72.png)

Nosotros utilizaremos un JY-MCU o [HC-06](https://www.google.com/url?q=https://www.electronicaembajadores.com/es/Productos/Detalle/LCBTHT6/modulos-electronicos/modulos-bluetooth/modulo-bluetooth-hc-06&sa=D&ust=1513946282913000&usg=AFQjCNGVPwbqIaSl83g1qkQu3Eyu5mgYsg) muy común y barato. .

![](/images/image71.png)

Te recomendamos estas páginas:

*   [Teoría de Bluetooth](https://www.google.com/url?q=https://catedu.gitbooks.io/programa-arduino-mediante-codigo/content/teora_bluetooth.html&sa=D&ust=1513946282913000&usg=AFQjCNExwoGDz-eIrGCuuYS3eRiIGm-fhw)
*   [Cómo se comunica con un Arduino](https://www.google.com/url?q=https://catedu.gitbooks.io/programa-arduino-mediante-codigo/content/mdulo_bluetooth.html&sa=D&ust=1513946282914000&usg=AFQjCNF-hMv5pjD9KSrm30OwufLsCImCxg)

Para conectar el HC-06 lo hacemos hacia abajo de modo que coincida los pines:

| Pines del HC-06 | Pines del Echidna | Pines del Arduino |
| --- | --- | --- |
| Vcc | 5V | 5V |
| GND | GND | GND |
| RX | TX | D1 |
| TX | RX | D0 |

![](/images/image39.png)

Nosotros vamos a utilizar la APP BlueControl:

*   [ver cómo funciona](https://www.google.com/url?q=https://catedu.gitbooks.io/programa-arduino-mediante-codigo/content/la_app.html&sa=D&ust=1513946282917000&usg=AFQjCNHHg9urZiFpzriTYLu8m3bOPNT7-g)
*   [ver cómo se vincula con el móvil](https://www.google.com/url?q=https://catedu.gitbooks.io/programa-arduino-mediante-codigo/content/vincular_mvil.html&sa=D&ust=1513946282917000&usg=AFQjCNHpsmCx_UeWor-4NHetd1qEQXH25A)

![](/assets/2018-02-10 20_47_35-¿Cómo emparejar el Bluetooth del Arduino con el móvil y la APP Bluecontrol - Pre.png)

### 5.1.2 Problema número 1: ocupamos el puerto serie {#5-1-2-problema-n-mero-1-ocupamos-el-puerto-serie}

Si has leído [Cómo se comunica con un Arduino](https://www.google.com/url?q=https://catedu.gitbooks.io/programa-arduino-mediante-codigo/content/mdulo_bluetooth.html&sa=D&ust=1513946282918000&usg=AFQjCNE5YcVVUpUsPb1bHvlMTgS6ZQBUuw) habrás visto que ocupamos LOS MISMOS PINES D0 Y D1 QUE UTILIZA EL ARDUINO PARA COMUNICARSE POR EL PUERTO SERIE CON EL ORDENADOR.

Esto crea un problema: No se puede tener conectado el HC-06 mientras nos comunicamos el ordenador con el Arduino.

Solución: **Pues quítalo,** y luego cuando acabes de descargar el programa en el Arduino,** pues lo pones**.

Bah!! ¿sólo era eso? pues no, que nos ocupe el puerto serie nos fastidia: ¿puedes interaccionar con el Sprite? por ejemplo ¿puedes hacer que el oso panda de mBlock se mueva según el mando de BlueControl?...**NO**

### 5.1.3 Problema 2 la velocidad del puerto es elevada {#5-1-3-problema-2-la-velocidad-del-puerto-es-elevada}

Al programar con mBlock fija la velocidad del puerto serie a 115200 baudios, y nuestro HC-06 soporta 9600

Solución: Bajarlo manualmente, **un rollo**, tenemos que salir de mBlock, editarlo en Arduino IDE .... esto se ve mejor en el ejemplo siguiente.

### 5.1.4 Reto: Encendido y apagado de LEDs con el móvil {#5-1-4-reto-encendido-y-apagado-de-leds-con-el-m-vil}

Vamos a ejecutar este pequeño programa, que al apretar el botón de arriba se encienden los leds y al apretar el de abajo se apagan:

{% youtube %}https://www.youtube.com/watch?v=XFPGEuX7uTs&feature=youtu.be{% endyoutube %}

%accordion%Solución%accordion%

![](/images/image49.png)

#### Primero hay que vincular el móvil con la APP

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vT0vG1z61MuZXKmdiw4ga7z15FlQfeussqDNYzMauJSZUU2G2NlL7M-JjXb4PFT4YTigj9Yal8PzHmR/embed?start=false&loop=false&delayms=3000" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>


#### Segundo hay que subir el programa solucionando los problemas anteriores

Mejor verlo con[ esta presentación:](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vTu_PBSd5olMZaMepTlp_kIVO67NDKiGwi6WCS9I_ECSQlq5SRAPQ5_P1vNMq_zrj6NujU0jTQzLsP8/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282920000&usg=AFQjCNGr6QOtYAEir7ENZwslE6wXKGZaeQ)

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vTu_PBSd5olMZaMepTlp_kIVO67NDKiGwi6WCS9I_ECSQlq5SRAPQ5_P1vNMq_zrj6NujU0jTQzLsP8/embed?start=false&;loop=false&;delayms=3000" frameborder="0" width="100%" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

%/accordion%

O sea, ya podemos jugar con el móvil y con nuestro Echidna !!!
<iframe src="https://giphy.com/embed/4K0kLjAFNgzao" width="425" height="480" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/phone-the-big-bang-theory-4K0kLjAFNgzao">via GIPHY</a></p>

Por ejemplo.. se podría hacer un coche teledirigido, el programa lo tienes en el repositorio: [https://github.com/JavierQuintana/Echidna](https://github.com/JavierQuintana/Echidna) 
y el vídeo en el [muro](/muro.md)



