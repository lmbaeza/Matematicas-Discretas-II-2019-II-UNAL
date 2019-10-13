# Algebra Booleana

### Minitermino
Para una función booleana de `n` variables ![miniterminos](http://latex.codecogs.com/gif.latex?x_1%2C%5C%3A...%5C%3A%2C%5C%3Ax_n) un producto booleano en el que cada una de la `n` variables aparece una sola vez (negada o sin negar) es llamado minitérmino.

**Ejemplo:**

* ![ejemplo](http://latex.codecogs.com/gif.latex?xyz)
* ![ejemplo](http://latex.codecogs.com/gif.latex?x%5Coverline%7By%7Dz)
* ![ejemplo](http://latex.codecogs.com/gif.latex?x%5Coverline%7By%7D%5Coverline%7Bz%7D)
* ![ejemplo](http://latex.codecogs.com/gif.latex?%5Coverline%7Bx%7D%5Coverline%7By%7Dz)
* `...`
* ![ejemplo](http://latex.codecogs.com/gif.latex?%5Coverline%7Bxyz%7D)

### Maxitermino
Para una función booleana de `n` variables ![miniterminos](http://latex.codecogs.com/gif.latex?x_1%2C%5C%3A...%5C%3A%2C%5C%3Ax_n) un maxitermino es la es una suma booleana en la que cada una de las n variables solo aparece una vez.

**Ejemplo:**

* ![ejemplo](http://latex.codecogs.com/gif.latex?x%5C%3A&plus;%5C%3Ay%5C%3A&plus;%5C%3Az)
* ![ejemplo](http://latex.codecogs.com/gif.latex?x%5C%3A&plus;%5C%3A%5Coverline%7By%7D%5C%3A&plus;%5C%3Az)
* ![ejemplo](http://latex.codecogs.com/gif.latex?x%5C%3A&plus;%5C%3A%5Coverline%7By%7D%5C%3A&plus;%5C%3A%5Coverline%7Bz%7D)
* ![ejemplo](http://latex.codecogs.com/gif.latex?%5Coverline%7Bx%7D%5C%3A&plus;%5C%3A%5Coverline%7By%7D%5C%3A&plus;%5C%3Az)
* `...`
* ![ejemplo](http://latex.codecogs.com/gif.latex?%5Coverline%7Bx%7D%5C%3A&plus;%5C%3A%5Coverline%7By%7D%5C%3A&plus;%5C%3A%5Coverline%7Bz%7D)

### Forma Normal Disyuntiva (FND)
En lógica booleana, una forma normal disyuntiva (FND) es una estandarización (o normalización) de una fórmula lógica que es una disyunción de cláusulas conjuntivas. 

*Suma de Miniterminos*

**Ejemplo:**

![FND](http://latex.codecogs.com/gif.latex?xyz%5C%3A&plus;%5C%3Axy%5Coverline%7Bz%7D%5C%3A&plus;%5C%3Ax%5Coverline%7By%7D%5Coverline%7Bz%7D%5C%3A&plus;%5C%3A%5Coverline%7Bxyz%7D)

### Forma Normal Conjuntiva (FNC)
En lógica booleana, una fórmula está en forma normal conjuntiva (FNC) si corresponde a una conjunción de cláusulas, donde una cláusula es una disyunción de literales, donde un literal y su complemento no pueden aparecer en la misma cláusula.

*Producto de Maxiterminos*

**Ejemplo:**

![FNC](http://latex.codecogs.com/gif.latex?%5Cleft%28x&plus;y&plus;z%5Cright%29%5Ccdot%20%5Cleft%28x&plus;y&plus;%5Coverline%7Bz%7D%5Cright%29%5Ccdot%20%5Cleft%28x&plus;%5Coverline%7By%7D&plus;%5Coverline%7Bz%7D%5Cright%29%5Ccdot%20%5Cleft%28%5Coverline%7Bx%7D&plus;%5Coverline%7By%7D&plus;%5Coverline%7Bz%7D%5Cright%29)

### Ejercicios:

#### 1) Pasar una función a Forma Normal Disyuntiva
![funtion](http://latex.codecogs.com/gif.latex?f%5Cleft%28x%2C%5C%3Ay%2C%5C%3Az%5Cright%29%5C%3A%3D%5C%3A%5Cleft%28x%5C%3A&plus;%5C%3Ay%5Cright%29%5Ccdot%20%5Coverline%7Bz%7D)

![function](http://latex.codecogs.com/gif.latex?x%5Coverline%7Bz%7D%5C%3A&plus;%5C%3Ay%5Coverline%7Bz%7D%5C%3A%3D%5C%3Ax1%5Coverline%7Bz%7D%5C%3A&plus;%5C%3A1y%5Coverline%7Bz%7D)

![function](http://latex.codecogs.com/gif.latex?%5C%3Ax%5Cleft%28y&plus;%5Coverline%7By%7D%5Cright%29%5Coverline%7Bz%7D%5C%3A&plus;%5C%3A%5Cleft%28x&plus;%5Coverline%7Bx%7D%5Cright%29y%5Coverline%7Bz%7D)

![function](http://latex.codecogs.com/gif.latex?xy%5Coverline%7Bz%7D%5C%3A&plus;%5C%3Ax%5Coverline%7By%7D%5Coverline%7Bz%7D%5C%3A&plus;%5C%3Axy%5Coverline%7Bz%7D%5C%3A&plus;%5C%3A%5Coverline%7Bx%7Dy%5Coverline%7Bz%7D%5C%3A)

![funtion](http://latex.codecogs.com/gif.latex?%3D%5C%3Axy%5Coverline%7Bz%7D%5C%3A&plus;%5C%3Ax%5Coverline%7By%7D%5Coverline%7Bz%7D%5C%3A&plus;%5C%3A%5Coverline%7Bx%7Dy%5Coverline%7Bz%7D%5C%3A)

### Bibliografia

[[1] Algebra de Boolean - Wikipedia](https://es.wikipedia.org/wiki/Formas_canónicas_(álgebra_de_Boole))

[[2] Forma normal disyuntiva - Wikipedia](https://es.wikipedia.org/wiki/Forma_normal_disyuntiva)

[[3] Forma normal conjuntiva - Wikipedia](https://es.wikipedia.org/wiki/Forma_normal_conjuntiva)