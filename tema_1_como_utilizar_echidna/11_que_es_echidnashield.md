## 1.1 ¿Qué es EchidnaShield? {#1-1-qu-es-echidnashield}

### 1.1.1 Primero ¿qué es Arduino? ¿qué es una Shield? {#1-1-1-primero-qu-es-arduino-qu-es-una-shield}

¿Qué es Arduino? Pues no podemos explicarlo en este curso, suponemos que lo conoces, sino te recomendamos [que visites esta página](https://www.google.com/url?q=http://aularagon.catedu.es/materialesaularagon2013/Arduino-codigo/1_Fundamentos_arduino_y_Edubasica/informacin_bsica_sobre_arduino.html&sa=D&ust=1513946282789000&usg=AFQjCNGOWM7sjaDcyBYG5PsZwEX378yvsQ), si la lees verás que tiene un inconveniente: Arduino es una placa microcontroladora orientado para las entradas y las salidas tanto analógicas como digitales, pero…. tienes que ponerlas, y eso implica cableado y electrónica.

Una solución es utilizar una Shield, está adaptado para ponerlo encima e incluso hay posibilidad utilizar varias a la vez.

![](images/image14.png)

 [Enrique Crespo](https://www.google.com/url?q=https://aprendiendoarduino.wordpress.com/&sa=D&ust=1513946282790000&usg=AFQjCNEn2pVo2t4pzYe5QHIJgDSzRi7hYQ) CC-BY-SA

Hay muchas en el mercado:

*   Para las comunicaciones:

*   [EthernetShield](https://www.google.com/url?q=http://arduino.cc/en/Main/ArduinoEthernetShield&sa=D&ust=1513946282791000&usg=AFQjCNED8XbujvH0W3_mV4nOHMkrN9fPMw).
*   [WifiShield](https://www.google.com/url?q=http://arduino.cc/en/Main/ArduinoWiFiShield&sa=D&ust=1513946282791000&usg=AFQjCNEbVO-c3cy8lyTdVxatS2ZBlw0oIQ)
*   [GSMShield móvil GPRS](https://www.google.com/url?q=http://arduino.cc/en/Main/ArduinoGSMShield&sa=D&ust=1513946282791000&usg=AFQjCNElNdodMK7E3F9XrKloBNv91NDAtA)

*   Para salidas concretas

*   [Motores](https://www.google.com/url?q=http://arduino.cc/en/Main/ArduinoMotorShieldR3&sa=D&ust=1513946282792000&usg=AFQjCNFycDm4oPRcP6pIAGo_vQMCn_nz0g)
*   [Relés RelayShield](https://www.google.com/url?q=http://wordpress.redirectingat.com/?id%3D725X1342%26site%3Daprendiendoarduino.wordpress.com%26xs%3D1%26isjs%3D1%26url%3Dhttp%253A%252F%252Fwww.seeedstudio.com%252Fdepot%252Frelay-shield-v20-p-1376.html%253FcPath%253D132_134%26xguid%3Dc96fc6b2e8b6e2cd4d30927fb5b4f760%26xuuid%3D943237e103c06b377b37d9b84237ccac%26xsessid%3Dd6ceb3761df5c0a048e8d27e4cb9982d%26xcreo%3D0%26xed%3D0%26sref%3Dhttps%253A%252F%252Faprendiendoarduino.wordpress.com%252F2015%252F03%252F23%252Fshields-para-arduino%252F%26pref%3Dhttps%253A%252F%252Fduckduckgo.com%252F%26xtz%3D-60&sa=D&ust=1513946282793000&usg=AFQjCNEHlYtEd6ZwKNIv6U68yJ0O4OQ7bA)

*   Para entradas concretas

*   [OpenEnergy Medidor Medidor de magnitudes eléctricas](https://www.google.com/url?q=http://openenergymonitor.org/emon/emontxshield/smt&sa=D&ust=1513946282793000&usg=AFQjCNFpC1mQ-cFhu6O9SQSh4RqTr1y6GA)

*   Para facilitar la conexión de sensores y actuadores

*   [Grove Shield](https://www.google.com/url?q=http://wordpress.redirectingat.com/?id%3D725X1342%26site%3Daprendiendoarduino.wordpress.com%26xs%3D1%26isjs%3D1%26url%3Dhttp%253A%252F%252Fwww.seeedstudio.com%252Fdepot%252FGrove-Base-Shield-p-754.html%26xguid%3Dc96fc6b2e8b6e2cd4d30927fb5b4f760%26xuuid%3D943237e103c06b377b37d9b84237ccac%26xsessid%3Dd6ceb3761df5c0a048e8d27e4cb9982d%26xcreo%3D0%26xed%3D0%26sref%3Dhttps%253A%252F%252Faprendiendoarduino.wordpress.com%252F2015%252F03%252F23%252Fshields-para-arduino%252F%26pref%3Dhttps%253A%252F%252Fduckduckgo.com%252F%26xtz%3D-60&sa=D&ust=1513946282794000&usg=AFQjCNG-R-W5rKO7B1nhMLypq0BtPiin_A) donde hay una familia sensores y actuadores de conectar y listo asociados.

Hay tantos que la lista es interminable…

Y otras están orientadas para el uso educativo:

*   [Edubásica](https://www.google.com/url?q=http://www.practicasconarduino.com/edubasica/&sa=D&ust=1513946282795000&usg=AFQjCNEF47F_X281uom93Kn-ywSbmYHT3A)[ ](https://www.google.com/url?q=http://www.practicasconarduino.com/edubasica/&sa=D&ust=1513946282795000&usg=AFQjCNEF47F_X281uom93Kn-ywSbmYHT3A)que en Aularagón tenemos [un curso dedicado](https://www.google.com/url?q=http://moodle.catedu.es/course/view.php?id%3D111&sa=D&ust=1513946282796000&usg=AFQjCNGsspGI01oVS4PP1SwjztLu5vP2aA) a esta Shield creada por docentes y para docentes.
*   ¿Y cómo no?: nuestra estrella en este curso [Echinda](https://www.google.com/url?q=http://echidna.es/&sa=D&ust=1513946282796000&usg=AFQjCNFunTuOFCt9IZOkGTWzogcQ0OD3EQ)

Hay muchas más Shields …. prueba poner las palabras Shield Arduino en tu buscador. Sólo hemos representado las que hemos elegido en nuestra

HOJA DE RUTA

.

También hay que nombrar “entrenadores” educativos para Arduino, “Kits de principiantes”, etc.. los hay con muchos sensores y otros muy compactos como [Evive](https://www.google.com/url?q=https://www.hackster.io/evive/products/evive&sa=D&ust=1513946282797000&usg=AFQjCNEnLOuE4TLgJ1DtEtGw-X1YRKdBtA): en el [vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?time_continue%3D35%26v%3D3F0_JspobN0&sa=D&ust=1513946282798000&usg=AFQjCNGSPO-_LZPb4pH3iPYWYPi3_JXU1g) explican muy bien las ventajas de utilizar una Shield/entrenador frente a usar la electrónica pura.

### 

###  {#-0}

### 1.1.2 Ahora sí: ¿Qué es Echidna? {#1-1-2-ahora-s-qu-es-echidna}

Es una Shield de Arduino diseñada para facilitar la programación del Arduino en los últimos cursos de primaria y primeros de secundaria, pensado en minimizar el cableado de la electrónica (ya lo sabemos pues es una Shield) y enfocado a nivel educativo y al lenguaje por símbolos

¿Por qué hemos elegido esta Shield?

Por varias razones:

*   Es OpenHardware, por lo tanto es un proyecto con garantías de estabilidad, libre, colaborativo y vivo, con la misma filosofía que la placa Arduino.
*   Salidas acertadas:

*   Diodos Red D13, Orange D12 y Green D11\.
*   Diodo de 3 colores RGB gobernados por D9, D5 y D6 respectivamente.
*   Audio en D10.

*   Entradas o sensores acertados:

*   Joystick (estupendo para hacer proyectos atractivos) xy con A0 y A1
*   Acelerómetro (idem) xy en A2 y A3
*   Luz LDR en A5
*   Botones digitales D2 y D3

*   Conexión Bluetooth que da más potencial a nuestros proyectos.
*   Es MakeyMakey: Dos Shields en una: Sensores y [MakeyMakey](https://www.google.com/url?q=https://www.makeymakey.com/&sa=D&ust=1513946282801000&usg=AFQjCNGmwfca8WNbhk924by4KaIzS1HjuQ) por lo tanto da más potencial a nuestros proyectos.(Tenemos [un curso en Aularagon de MakeyMakey)](https://www.google.com/url?q=http://moodle.catedu.es/course/view.php?id%3D56&sa=D&ust=1513946282802000&usg=AFQjCNGrr19QzlN8_sn-qEpfskXqkvI28w)
*   Es barato y asequible para la mayoría de los centros.
*   Tiene pines para conexión de otros elementos como relés pero no pueden pasar de 300mA para más potencia es mejor utilizar Shield adaptados para ello como Edubásica.