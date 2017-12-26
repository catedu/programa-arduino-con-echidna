## 4.2 Piano con bananas {#4-2-piano-con-bananas}

Vamos a hacerlo !! Ten en cuenta que mBlock utiliza la notación americana de notas, y a cada nota la vamos a corresponder a una entrada Makey Makey (utilizando por ejemplo el acorde 4):

| Nota americana | C4 | D4 | E4 | F4 | G4 | A4 | B4 | C5 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Nota Europea | Do | Re | Mi | Fa | Sol | La | Si | Do |
| Makey | A0 | A1 | A2 | A3 | A4 | A5 | D2 | D3 |

Como las entradas analógicas pueden variar desde 0 a 1024 vamos a fijar como umbral en 500 (si es muy sensible lo subimos, si no nos hace caso lo bajamos, a nosotros nos ha funcionado bien 500).

El código lo subiremos al Arduino pues mBlock responde muy lentamente, si no te acuerdas cómo se hacía mira esta [presentación](https://www.google.com/url?q=https://docs.google.com/presentation/d/e/2PACX-1vTkh8pwo-b7LACnD7_ZAfWzYCchZI9H1_uR-tZqgfBRtOPFOaVDH8ognsCNEXA8khLI7UX6ziUQXZsx/pub?start%3Dfalse%26loop%3Dfalse%26delayms%3D3000&sa=D&ust=1513946282906000&usg=AFQjCNFKwGl4hNX0DvbuGHV6KWk4Um_4wg).

%accordion%Solución%accordion%

El programa es muy sencillo pero repetitivo:

![](/images/image21.png)

%/accordion%

Conectamos cada salida de Makey Makey a unos plátanos y la salida del auricular a unos altavoces de ordenador, en la foto puedes ver que se han utilizado unos cables con cocodrilos, y al subirlo al Arduino no hace falta tener el ordenador, alimentamos el Arduino con un PowerBank o incluso con pilas.

**ATENCIÓN VER [1.3 ALIMENTACION DEL ECHIDNA](/tema_1_como_utilizar_echidna/13-alimentacion-del-echidna.md)**

Y el [resultado](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DgyBRvFvs3Mk&sa=D&ust=1513946282908000&usg=AFQjCNHAm9mu3pM9P5Ng4GPBU_95yaO3mg) es …

{% youtube %} https://www.youtube.com/watch?v=gyBRvFvs3Mk{% endyoutube %} 

No somos buenos artistas, aún así en Catedu tenemos a uno que sabe tocar el piano y otro que es músico pero de guitarra!

![](/images/image35.png)