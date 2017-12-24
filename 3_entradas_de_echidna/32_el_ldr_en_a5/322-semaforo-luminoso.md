RETO Vamos a reutilizar esfuerzos: reutilizar el semáforo visto en [esta sección](../tema_1_como_utilizar_echidna/12_como_se_programa_echidna_shield.md#1-2-1-programaci-n-gr-fica-con-mblock) pero vamos a hacer que se iluminen los colores según la luz:

| Semáforo | Luz |
| --- | --- |
| Todo apagado | Mucha oscuridad |
| Rojo | Oscuridad |
| Amarillo | Luz normal |
| Verde | Mucha luz |

SOLUCIÓN

Según nuestros límites medidos en el anterior programa fijamos nuestras propias fronteras para cumplir el enunciado (puedes poner otros valores parecidos):

| Semáforo | Luz | Límite inferior | Límite superior |
| --- | --- | --- | --- |
| Todo apagado | Mucha oscuridad | --- | 199 |
| Rojo | Oscuridad | 200 | 499 |
| Amarillo | Luz normal | 500 | 799 |
| Verde | Mucha luz | 800 | --- |

El programa sería el siguiente, donde hemos capturado los semáforos en los tres estados utilizando una linterna y nuestra mano para oscurecer el LDR:

![](/images/image68.png)

El resultado lo puedes ver en [este vídeo](https://www.google.com/url?q=https://www.youtube.com/watch?v%3DMX558VKV_pE&sa=D&ust=1513946282868000&usg=AFQjCNGfVxyWAIq0qEDJW3N48RafvkjefQ):

https://www.youtube.com/watch?v=MX558VKV_pE

