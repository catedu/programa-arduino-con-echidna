## 2.1 Luces {#2-1-luces}

Ya hemos visto las luces LED con el [semáforo](../tema_1_como_utilizar_echidna/12_como_se_programa_echidna_shield.md#1-2-1-programaci-n-gr-fica-con-mblock), ahora vamos a ver el **LED RGB**  
![](/assets/2017-12-22 13_45_04-EchidnaShield.png)  
Está conectado a las salidas digitales D5, D6 y D9 y si te fijas, en el Arduino tienen el símbolo ~ ¿Qué significa esto? Que son señales PWM. Si has leído [¿Qué es un Arduino?](../tema_1_como_utilizar_echidna/11_que_es_echidnashield.md#1-1-1-primero-qu-es-arduino-qu-es-una-shield) habrás leído que es una señal digital pero los pulsos pueden variar su ancho de tal manera que la media puede ser una tensión entre 0 y 5V, que se gobiernan con esta instrucción:

![](/images/image36.png)

Donde 0 sería 0V y el valor 255 sería el valor máximo de tensión que en nuestro caso es 5V aunque puede ser otra tensión si se alimenta Arduino con una alimentación externa Vin.

**RETO**

Vamos a realizar un programa con mBlock que se iluminen todas las luces de colores de forma aleatoria, además vamos a poner un fondo, un personaje y música para que parezca una discoteca.

%accordion%Solución%accordion%



Vamos a utilizar un sprite de la biblioteca que tiene mBlock “cassy” que tiene ya los disfraces apropiados de baile:

![](/images/image77.png)

De fondo, utilizaremos el escenario de la biblioteca también “Spootlight” pero añadiremos otro pintando el mismo pero modificándolo de forma que parezca que salgan luces \(aquí te ponemos el reto de copiar el escenario en un editor de imágenes, aunque sea el Paint y poner los haces de luces\):

![](/images/image27.png)

Y ya nos queda programar en el Sprite cassy para cumplir el enunciado:

![](/images/image54.png)

El programa lo puedes descargar de este [repositorio](https://www.google.com/url?q=https://drive.google.com/drive/folders/1pXcRUqMM7q_UK0QhILd9QwLe8KtPCM5m?usp%3Dsharing&sa=D&ust=1513946282845000&usg=AFQjCNFQB4Zf3zyqNCr_9ynL06x8skFTKg).

%/accordion%

El resultado es el siguiente [vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Ds2yQwG53sGg%26feature%3Dyoutu.be&sa=D&ust=1513946282845000&usg=AFQjCNHE7oXLQVNlgArzKmpprdUN85NpOw):

[https://www.youtube.com/watch?v=s2yQwG53sGg&;feature=youtu.be](https://www.google.com/url?q=https://www.youtube.com/watch?v%3Ds2yQwG53sGg%26feature%3Dyoutu.be&sa=D&ust=1513946282846000&usg=AFQjCNEgkcJwuMtyh4Ci2Ts5Wzw6jlXejw)

