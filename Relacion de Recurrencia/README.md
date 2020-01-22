# Relación de Recurrencia / Ecuaciones en Diferencias Lineales

## Contenido

* [Formulas Importantes](##formulas-importantes)
* [Relación de Recurrencia de 1er Orden](#relación-de-recurrencia-de-1er-orden)
* [Ecuación Caracteristica de 2do Orden](#ecuación-caracteristica-de-2do-orden)
* [Casos Posibles](##casos-posibles)
* [Bibliografia](#bibliografia)

## Formulas Importantes
* Esta ecuación solo se cumple si todas las soluciones de la ecuación caracteristica son diferentes.

    * ![Ecuacion 1](http://www.sciweavers.org/upload/Tex2Img_1579666667/render.png)

* Esta ecuación solo se cumple si se retire alguna solucion de la ecuación caracteristica.

    * ![Ecuación 2](http://www.sciweavers.org/upload/Tex2Img_1579666860/render.png)

## Relación de Recurrencia de 1er Orden
* Una Relación de Recurencia Lineal, Homogenea de orden `k` y con coeficiente constante es una relación de recurrencia de la forma:

![Relación de Recurrencia de 1er Orden](http://www.sciweavers.org/upload/Tex2Img_1579648677/render.png)

Donde  `C1, C2, C3, ..., Cn` Son numeros reales con `Ck ≠ 0`.

* La Ecuación es **Lineal** porque el termino de la derecha es una suma de multiplos del termino anterior de la sucesión.

* Es **Homogenea** porque no aparecen terminos que no sean multiplos de los ![A sub i](http://www.sciweavers.org/upload/Tex2Img_1579649072/render.png).

* `k` condiciones iniciales.
    ![K Condiciones Iniciales](http://www.sciweavers.org/upload/Tex2Img_1579649186/render.png)

**Nota:** Las relaciones de recurrencia Lineal y Homogeneas se estudian por dos motivos:

1. Aparecen con Frecuencia en problemas de Modelado
2. Pueden resolverse de forma sistematica.

## Teorema I

Sean `c1` y `c2` Números reales. Supongamos que ![Ejemplo 1](http://www.sciweavers.org/upload/Tex2Img_1579663621/render.png) tiene dos(2) raices reales distintas `r1` y `r2`. Entonces la sucesión ![A de n](http://www.sciweavers.org/upload/Tex2Img_1579662500/render.png) es una solución de la relación de recurrencia:

![Relación de Recurrencia](http://www.sciweavers.org/upload/Tex2Img_1579662630/render.png) 

Si, y solo si

![Ecuación 1](http://www.sciweavers.org/upload/Tex2Img_1579662740/render.png)

Para `n = 0, 1, 2, 3, ...`  donde `α1` y `α2` son constantes.

## Ecuación Caracteristica de 2do Orden

![Ecuación Caracteristica](http://www.sciweavers.org/upload/Tex2Img_1579662913/render.png)

![A n de p](http://www.sciweavers.org/upload/Tex2Img_1579662967/render.png) Solución Particular

![A de n](http://www.sciweavers.org/upload/Tex2Img_1579663040/render.png) Solución  General

* Si ![A n de p](http://www.sciweavers.org/upload/Tex2Img_1579662967/render.png) es una solución particular de:

![Ecuacion 2](http://www.sciweavers.org/upload/Tex2Img_1579665661/render.png)

y ![Ecuacion 3](http://www.sciweavers.org/upload/Tex2Img_1579665720/render.png) forman un sistema fundamental de soluciones `(h)`, entonces la **Solución General** es:

![Ecuación 4](http://www.sciweavers.org/upload/Tex2Img_1579665859/render.png)

## Casos Posibles

* Si ![Ecuacion 5](http://www.sciweavers.org/upload/Tex2Img_1579665959/render.png), para el ejemplo:

![Ecuacion 6](http://www.sciweavers.org/upload/Tex2Img_1579666024/render.png)

Probar con ![Ecuacion 7](http://www.sciweavers.org/upload/Tex2Img_1579666110/render.png) Excepto si `z` es la raiz de la ecuación caracteristica.

Si `z` es ka raiz de multiplicidad `m` entonces buscamos una solución de la forma.

![Ecuacion 8](http://www.sciweavers.org/upload/Tex2Img_1579666220/render.png)

* Si `q(n)` es un polinomio de grado `k`, buscamos soluciones en forma de polinomio del mismo grado. Si el 1 es raiz de la ecuación caracteristica, tomamos un polinomio de grado `k+1`, si ademas tiene grado de multiplicidad `c` probamos con un polinomio de grado `n+c`.

* Si `q(n)` es `sen(z*n)` o `cos(z*n)` entonces:

![Ecuacion 9](http://www.sciweavers.org/upload/Tex2Img_1579666466/render.png)

Y se debe determinan los valores de las constantes `β` y `x`.

# Bibliografia
[[1]](https://images-na.ssl-images-amazon.com/images/I/21dyiE2bogL._BO1,204,203,200_.jpg) Rosen, K. (n.d.). Discrete mathematics and its applications. McGraw Hill, pp.384-396.

[[2]](https://www.youtube.com/watch?v=GVQnbhqg2tU) YouTube. (2020). Matemática Discreta - Ecuaciones recurrentes lineales homogéneas. [online] Available at: https://www.youtube.com/watch?v=GVQnbhqg2tU.

[[3]](https://www.youtube.com/watch?v=Y6IFHKuSYzI) YouTube. (2020). Matemática Discreta - Ecuaciones recurrentes lineales homogéneas 2. [online] Available at: https://www.youtube.com/watch?v=Y6IFHKuSYzI.

[[4]](https://www.youtube.com/watch?v=JHeVpfXyaB4) YouTube. (2020). Método de la ecuación característica para recurrencias homogéneas lineales de segundo orden con coef. [online] Available at: https://www.youtube.com/watch?v=JHeVpfXyaB4.