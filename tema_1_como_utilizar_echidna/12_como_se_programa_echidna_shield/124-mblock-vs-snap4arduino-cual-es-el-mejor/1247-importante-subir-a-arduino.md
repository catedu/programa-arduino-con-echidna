#### 1.2.4.7 Subir a Arduino {#1-2-4-7-subir-a-arduino}

En mBlock podemos poner la vista de Modo Arduino Y NOS MUESTRA NUESTRO PROGRAMA ESCRITO EN LENGUAJE GRAFICO CONVERTIDO A LENGUAJE CÓDIGO![](/images/image18.png)

Esto nos permite SUBIR AL ARDUINO es decir, nuestro programa grabarlo en el Arduino como si fuera un Firmware y ganar velocidad aquí tienes una captura y puedes observar cómo traduce el programa gráfico en código:

![](/images/image41.png)

El anterior programa funciona bien si lo hacemos subir al Arduino, pero si lo hacemos de forma normal (cambiamos el evento “Programa Arduino” por evento bandera):![](/images/image38.png)

NO FUNCIONA BIEN

¿por qué?: por la lentitud.

Si apretamos el pulsador 2 le pedimos al ordenador que encienda y apague D10 a una velocidad de 0.00175 segundos esto lo tiene que procesar el ordenador, pasa por el cuello de botella del puerto serie y al final se ejecuta en el Arduino a una velocidad mucho más baja, más o menos 0.5 segundos, en vez de oirse un tono, se oye tut,tut,tut,tut….

Si apretamos el pulsador 3 sí que se oye bien, porque mBlock manda el código del bucle de golpe para que se oiga bien.

Volveremos a este programa varias veces, no te preocupes si no lo has entendido del todo bien.

Desventajas de subir un programa al Arduino:

1.  NO PODEMOS INTERACTUAR CON EL ORDENADOR es decir, no podemos hacer que el sprite (el oso por defecto) se mueva o que al pulsar una tecla del ordenador… porque EL ARDUINO ES INDEPENDIENTE DEL ORDENADOR, incluso podemos desconectarlo y sigue funcionando !!!
2.  Nos hemos cargado el Firmware que tenía antes !! luego al finalizar tu programa, tenemos que volver a configurar el Arduino para que haga caso al programa mBlock visto en [esta presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vRLqEoJCT355xMCeCXsd0Wc7JcJRk9JkwLCyzEPb_h1S2IbYKK7OdUf33yWRIXq216Zgh9Da7-gIOq1/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282836000&usg=AFQjCNHZIx2i9Q4U-O15shd8SJobHkWsQA).

Ventajas de subir un programa al Arduino:

1.  Rapidez, tenemos la ventaja del lenguaje con código, el programa se ejecuta a la velocidad del Arduino sin tener el ordenador como intermediario.
2.  Independencia: Alimentamos el arduino con una batería ¡¡ y funciona !! esto es esencial para proyectos que impliquen movimiento y no queramos tener el ordenador encendido para que funcione.

