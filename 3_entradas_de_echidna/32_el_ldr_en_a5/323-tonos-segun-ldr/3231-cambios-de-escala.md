#### 3.2.3.1 Cambios de escala {#3-2-3-1-cambios-de-escala}

Nos encontramos que:

*   Los valores de entrada, es decir, el LDR trabaja con unos límites, que según hemos visto en [el apartado comprobar los límites](#3-2-1-comprobar-los-l-mites), el nuestro va de 108 a 982, llamaremos a esta variable de entrada X
*   Los valores de salida son los tonos,que mBlock trabaja con la norma americana (la europea es el típico DoReMiFaSol) y los americanos, son valores numéricos que van desde 48 hasta 72 (lo puedes comprobar con la instrucción “tocar nota” que está en Programas-Sonido). Llamaremos a la variable salida de notas Y:

![](/images/image67.png)

Problema: ¿cómo convertimos X en Y?

Matemáticamente es una recta con una pendiente m y una ordenada n :

Y = m*X + n

Para calcular m y n tenemos que utilizar un sistema de ecuaciones dadas las condiciones límites de X e Y:

*   Cuando X = 108 quiero que Y valga 48: 48=m*108 + n
*   Cuando X = 982 quiero que Y valga 72: 72=m*982 + n

Ala! calcula m y n

![](/images/image11.png)

Buen ejercicio para los alumnos para que vean matemáticas aplicadas

No obstante, como esto lo repetiremos muchas veces los cambios de escala, hemos confeccionado [ESTA HOJA DE CÁLCULO](https://www.google.com/url?q=https://docs.google.com/spreadsheets/d/e/2PACX-1vTyASTvUIs_xsZ8c4RZOJ1sEstk4Cc6d--_Drne_U0o1_CXhgzxQkvZ4ZNYGLdKa2lrhLHDKmAwsKnK/pub?output%3Dxlsx&sa=D&ust=1513946282873000&usg=AFQjCNG67xpZIAuP9snBWW1bar7eOxSF9g) que te lo puedes descargar y facilita las cosas: Ponemos en las celdas amarillas los valores límites :

*   X1= 108 X2=982
*   Y1=48    Y2=72

Y nos da los valores m y n automáticamente:

![](/images/image46.png)

Luego la fórmula para el cálculo de la Y (las notas) en función de la luminosidad X es:

Y = 0.027 * X + 45

