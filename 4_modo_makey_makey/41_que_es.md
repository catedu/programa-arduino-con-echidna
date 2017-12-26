## 4.1 ¿Qué es? {#4-1-qu-es}

Es una placa que se inventó en 2010 que permite conectar cualquier cosa que conduzca mínimamente la electricidad en entrada por el puerto USB. Para que lo entiendas bien, mira este vídeo:

{% youtube %}https://www.youtube.com/watch?v=rfQqh7iCcOU{% endyoutube %}

Nuestra placa tiene esta función, pero en vez de ser una entrada por el puerto USB es una entrada por Arduino que podemos leer, luego en esta sección cambia nuestra placa Echidna el modo sensor a modo makey makey

![](/images/image4.png)

Tiene las siguientes entradas:

![](/images/image59.png)

*   ANALOGICAS

    *   Desde A0 hasta A5 que tenemos que detectarlas si superan un cierto “umbral” que dependerá de lo que conectemos.

*   DIGITALES

    *   D2 y D3 aquí es fácil, 0 o 1
    
*   GND o sea el conector que tiene que conectarse a una parte de tu cuerpo y realizarás el puente eléctrico.

_Nota_:

En [Aularagón](https://www.google.com/url?q=http://moodle.catedu.es/&sa=D&ust=1513946282898000&usg=AFQjCNFbbdhoQZIogmh59s6_ZIDyenPqFA) tienes un curso de manejo de la Makey Makey original Scractch avanzado y Makey Makey ¿entonces?¿qué ventajas tiene esta placa con respecto a la original?:

*   Más **barata **(importante)
*   **2x1** sí, sí, piénsalo: Tienes en la misma placa una Shield educativa con sensores y a le vez una Makey makey,
*   **Autonomía**: Makey necesita un ordenador y nuestra Echidna necesita Arduino ¿quien gana en simplicidad? si hacemos que nuestro programa se graba al Arduino: _¡¡La portabilidad es total!!_

.