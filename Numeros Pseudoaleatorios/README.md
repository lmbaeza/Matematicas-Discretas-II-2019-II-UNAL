# Numeros Pseudoaleatorios

Un número Pseudo-aleatorio es un número generado mediante un proceso que usa una formula matematica para producir secuencias de numeros, estas secuencias se aproximan a las propiedades de los numeros aleatorios a pesar de que no los son ya que es un proceso netamente determinista definido por un valor inicial llamado `semilla`, cabe señalar que para la misma semilla se generaran dos numeros iguales.

La formula matematica de un generador congruencial lineal mencionada anteriormente es la siguiente:

![Numeros Pseudoaleatorios](https://i.ibb.co/qxb0vgb/Numeros-Pseudoaleatorios.png)

Donde:

`m` : Modulo, `a` : Multiplicador, `c` : Incremento, `x0` : Semilla

1. El modulo `m` es la cuota superior del numero de valores diferentes que puede tomar la semilla

2. Cuando `xi` vuelve a tomar el valor de la semilla inicial `x0`, la secuencia se repite ciclicamente

3. Todas las secuencias conocidas con este tipo de generador si se prolongan lo suficiente acaba en un ciclo que se repite infinitamente.

¿podemos elegir `a` y `c` de tal manera que logremos alcanzar el periodo máximo(`m`)?

Respuesta: Si, cumpliendo las Condiciones de Donald Knuth

## Condiciones de Donald Knuth
Existen 3 condiciones creadas por Donald Knuth para alcanzar el numero maximo de pseudoaleatorios posibles y estas son las Siguientes:

Un generador congruencial mixto (`c>0`) tendrá periodo completo para todas las semillas sí y sólo sí:

1. `m` y `c` son primos relativos.
2. `a − 1` es divisible por todos los factores primos de `m`.
3. `a − 1` es divisible por `4` siempre que `m` sea divisible por `4`.


## Algoritmo Iterativo en Python

```python
# Generador Congruencial de Numeros Pseudoaleatorios

class GeneradorCongruencial:

  def __init__(self, x0, a, c, m):
    self.xo = x0
    self.a = a
    self.c = c
    self.m = m

  def value(self, aXi):
    return (((self.a * aXi) + self.c) % self.m)

  def Xn(self):
    aXi = self.value(self.xo)

    print(aXi)

    while (aXi != self.xo):
      aXi = self.value(aXi)
      print(aXi)

gc = GeneradorCongruencial(3, 7, 4, 9)
gc.Xn()
```

# Bibliografia

[[1]](https://github.com/neoslink/gcm/blob/master/Python/gcm.py) A. Piña, "Generador Congruencial Mixto", GitHub, 2019. [Online]. Available: https://github.com/neoslink/gcm/blob/master/Python/gcm.py.

[2] Knuth, Donald E. 1997. The Art of Computer Programming, Volume 2: Seminumerical Algorithms. Third. Boston: Addison-Wesley.

[[3]](https://tereom.github.io/est-computacional-2018/numeros-pseudoaleatorios.html) M. Ortiz, "7.1 Números pseudoaleatorios | Estadística Computacional", Tereom.github.io, 2019. [Online]. Available: https://tereom.github.io/est-computacional-2018/numeros-pseudoaleatorios.html .