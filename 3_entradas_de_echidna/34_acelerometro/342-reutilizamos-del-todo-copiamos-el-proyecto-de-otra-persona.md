#### 3.4.2 Reutilizamos del todo: Copiamos el proyecto de otra persona {#3-4-2-reutilizamos-del-todo-copiamos-el-proyecto-de-otra-persona}

Esta vez no vamos a ser originales, vamos a ser un poco vagos y nos vamos a copiar el programa de otra persona

![](/images/image78.png)

Vamos a buscar un programa de un videojuego y hacerlo que funcione con nuestro acelerómetro de la Echidna.

La [web de Scratch](https://www.google.com/url?q=https://scratch.mit.edu/&sa=D&ust=1513946282889000&usg=AFQjCNGygwtyuNaEEsxDNvVSFxX9GBVf1A) tiene un repositorio de millones de proyectos, podemos seleccionar uno, y adaptarlo a nuestra simpática Echidna. Vamos a ver un ejemplo con este proyecto [https://scratch.mit.edu/projects/29744/](https://www.google.com/url?q=https://scratch.mit.edu/projects/29744/&sa=D&ust=1513946282890000&usg=AFQjCNEWwHBWiXjFJuaLk0mMV7oYIQlLdQ)

##### 3.4.2.1 Reutilizando un proyecto con mBlock {#3-4-2-1-reutilizando-un-proyecto-con-mblock}

En [esta presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vSCDGNYTkUuXsIOtMJDozS3jijvI8ZgYk9cy50vpgvlCAUVZOZbLtTjynKjkZ_CHhq9nvJQzIefO9V2/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282890000&usg=AFQjCNHlGqrxqDlrGjo3EAQlihyYh5JcXw) se muestra cómo se importa un proyecto a mBlock:

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vSCDGNYTkUuXsIOtMJDozS3jijvI8ZgYk9cy50vpgvlCAUVZOZbLtTjynKjkZ_CHhq9nvJQzIefO9V2/embed?start=false&;loop=false&;delayms=3000" frameborder="0" width="100%" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

Una vez importando nos fijamos en el código que hay que modificar, está claro que lo que hay que tocar es el Sprite “Ship” que es el que queremos mover con el acelerómetro y modificar el “posicionX que se realiza con el ratón y cambiarlo por el acelerómetro:

![](/images/image44.png)

Perooo como siempre: la posición del ratón es la misma que las coordenadas de la pantalla de mBloc y la x va desde -240 hasta 240 y nuestro acelerómetro de A2 va desde 250 hasta 500 luego hacemos el cambio de escala con la [HOJA DE CÁLCULO](https://www.google.com/url?q=https://docs.google.com/spreadsheets/d/e/2PACX-1vTyASTvUIs_xsZ8c4RZOJ1sEstk4Cc6d--_Drne_U0o1_CXhgzxQkvZ4ZNYGLdKa2lrhLHDKmAwsKnK/pub?output%3Dxlsx&sa=D&ust=1513946282891000&usg=AFQjCNG-30BZx1eA-t1QqrwaNZvW04wknA) que ya lo hemos hecho con el [helicóptero](#3-4-1-1-helic-ptero) anteriormente:

![](/images/image24.png)

Y cambiamos el código:

![](/images/image37.png)

También vamos a cambiar el disparador “espacio” por pin digital 2 para disparar con el botón D2 del Echidna:

![](/images/image3.png)

El resultado en[ este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DPs3jB89KIg8%26feature%3Dyoutu.be&sa=D&ust=1513946282892000&usg=AFQjCNFBi0uZVxoLx2azVBPFTGbAaJ8gFw):

[https://www.youtube.com/watch?v=Ps3jB89KIg8&;feature=youtu.be](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DPs3jB89KIg8%26feature%3Dyoutu.be&sa=D&ust=1513946282892000&usg=AFQjCNFBi0uZVxoLx2azVBPFTGbAaJ8gFw)

##### 3.4.2.2 Reutilizando un proyecto con Snap4Arduino {#3-4-2-2-reutilizando-un-proyecto-con-snap4arduino}

Este programa para la simulación de proyectos grandes va más rápido por lo que vamos a ver como alternativa:

Para importar un proyecto desde Scratch es un poco más complicado, ver [esta presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vQ7PutZ1rJdylUGdaQ6qgkoofiQu1-t0inaBN5JN0idYOlvlK84qa1THTBzNUx4SW3kslXdjUdEs9NF/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282893000&usg=AFQjCNEVlBh7kkM1aLorDX-QmbsH9hplKw):

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vQ7PutZ1rJdylUGdaQ6qgkoofiQu1-t0inaBN5JN0idYOlvlK84qa1THTBzNUx4SW3kslXdjUdEs9NF/embed?start=false&;loop=false&;delayms=3000" frameborder="0" width="100%" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

Los cambios en el código son los mismos que los anteriores. ![](/images/image89.png)

Recuerda que e[n esta presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vQ7tr9aNDDuzFcEMFOepVVao5eCKWBBQh3U5emsy5oaN4a-Q8tNkYMWxKyma6xz-gBVL6nLLlmlWuPw/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282894000&usg=AFQjCNH_vEQY0Dj3hZ-FhPh4qoUqn2RKkw) se enseña cómo configurar Snap4Arduino para que se comunique con nuestro Arduino y la Echidna.

El programa lo puedes abrir en Snap4Arduino en esta [URL](https://www.google.com/url?q=http://snap4arduino.org/run%23present:Username%3Djavierquintana%26ProjectName%3DAlien%2520Invasion-MODIFICADO&sa=D&ust=1513946282894000&usg=AFQjCNF-EVqjqnW1UNgn7LgENVXRNCHhIg)

El Sprite que tienes que conectar con Arduino es la nave esa con cuernos.

El resultado lo puedes ver en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Dec4q_5bbBQQ%26feature%3Dyoutu.be&sa=D&ust=1513946282895000&usg=AFQjCNH6g4-3XuX_dmITOzJaesmWmq3CPA):

[https://www.youtube.com/watch?v=ec4q_5bbBQQ&;feature=youtu.be](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Dec4q_5bbBQQ%26feature%3Dyoutu.be&sa=D&ust=1513946282895000&usg=AFQjCNH6g4-3XuX_dmITOzJaesmWmq3CPA)