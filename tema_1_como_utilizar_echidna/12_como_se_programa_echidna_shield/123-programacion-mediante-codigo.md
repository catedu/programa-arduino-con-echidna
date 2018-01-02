**PRIMERO QUÉ ES "MEDIANTE CODIGO" **

Es la forma de trabajar de forma profesional el Arduino: con su lenguaje código, en realidad, los otros lenguajes traducen el programa gráfico en lenguaje código Arduino, es decir son meros intermediarios.
![](/images/image20.png)

El programa se puede descargar de su web oficial, aunque también hay una versión online [https://www.arduino.cc/](https://www.google.com/url?q=https://www.arduino.cc/&sa=D&ust=1513946282816000&usg=AFQjCNHa3tcU0VmaAnThGmZXHCiV-qpDug)

**SEGUNDO LA CONFIGURACIÓN**

Aquí no hay que instalar ningún Firmware, pues el código, o sea tú programa, es el mismo “firmware”. Digamos que no necesitas intermediarios si tratas con el agricultor ;)

**TERCERO EL EJEMPLO SEMÁFORO CON CÓDIGO**

Aquí es donde vemos que la programación no es apropiada para Primaria, y la explicación de cada línea necesitaría un curso entero. ([Como el que hay en Aularagón !](https://www.google.com/url?q=http://moodle.catedu.es/course/view.php?id%3D111&sa=D&ust=1513946282817000&usg=AFQjCNERjSWHukwxmzhifvfPZT29ynCGJw) ) pero si eres un poco _pito_ seguro que eres capaz de leerlo intuitivamente sin problemas.

```cpp

/* Semáforo Arduino
  Leds conectados a pines 11,12,13 = EchidnaShield */
int verde = 11;
int amarillo = 12;
int rojo = 13;

void setup()
{
 pinMode(verde, OUTPUT);
 pinMode(amarillo, OUTPUT);
 pinMode(rojo, OUTPUT);
 Serial.begin(9600); //inicializa la comunicación Serial
}

void loop()
{
 Serial.println("Semaforo - Inicio"); //Escribe el texto 
 digitalWrite(verde, HIGH);
 Serial.println("Semaforo - Verde"); //Escribe el texto
 delay(2000);
 digitalWrite(verde, LOW);
 digitalWrite(amarillo, HIGH);
 Serial.println("Semaforo - Amarillo"); //Escribe texto
 delay(1000);
 digitalWrite(amarillo, LOW);
 digitalWrite(rojo, HIGH);
 Serial.println("Semaforo - Rojo"); //Escribe el texto
 delay(2000);
 digitalWrite(rojo, LOW);
}

```

Este programa se escribe (o copia y pega ¡es un texto !!) en el software del Arduino y se carga en la placa, en[ el vídeo](https://www.google.com/url?q=https://youtu.be/S8dQdCqOtto&sa=D&ust=1513946282823000&usg=AFQjCNHMu_skH6o86eJWChPi0zjmOX5ymw) se ve muy bien:

{% youtube %}https://www.youtube.com/watch?v=S8dQdCqOtto&;feature=youtu.be{% endyoutube %}

En este programa queremos que te fijes en una **desventaja**: La interacción con el ordenador se pierde frente a mBlock y Snap4Arduino:

*   En los lenguajes gráficos, tenemos a **interacción con el ordenador** igual que en Scratch: si te fijas en la pantalla el dibujo del semáforo va cambiando de disfraz para representar los colores de la luz que se enciende a la vez que en el Arduino.
*   En un programa grabado en el Arduino **perdemos esa interacción**, lo máximo que podemos visualizar es una ventana donde se representa en formato texto qué es lo que le está pasando al Arduino (en el ejemplo del semáforo sale "Semáforo - Verde, Semáforo- Rojo ….")(en realidad, con programación muy muy avanzada sí que se podría pero no vamos a entrar en estos jaleos).

Esto lo vemos como una **desventaja** desde el punto de vista de la enseñanza de la programación pues perdemos el potencial de interactuar con los elementos del ordenador crear personajes, disfraces, sonidos, teclado….

Pero… (siempre hay un “pero” para estropear la fiesta) la programación en código tiene una **ventaja**: Se graba en el Arduino, no hay ningún intermediario entre nuestro programa y el Arduino (en mBlock y Snap está el ordenador), quien manda en el Arduino es nuestro programa, no nuestro ordenador, esto se traduce en: **rapidez !**, esto se soluciona en mBlock como lo veremos [más adelante.](https://catedu.gitbooks.io/programa-arduino-con-echidna/content/tema_1_como_utilizar_echidna/12_como_se_programa_echidna_shield/124-mblock-vs-snap4arduino-cual-es-el-mejor/1247-importante-subir-a-arduino.html)

**Conclusión**: Profesionalmente es mejor utilizar lenguaje con código pero en la enseñanza es mejor el lenguaje gráfico, además lo hemos dicho en el [apartado ¿Cómo se programa Echidna?](#1-2-c-mo-se-programa-echidna-shield) es una Shield Educativa que lo lógico es utilizar un lenguaje adaptado al nivel educativo: Gráfico. Pero … ¿cual?

