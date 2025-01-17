


# 100 ejercicios de numpy

Esta es una colección de ejercicios recogidos de distintas fuentes como: numpy mailing list, stackoverflow Y
documentación de numpy. El objetivo de esta colección es ofrecer material para el aprendizaje de numpy.

Este repositorio es una traducción del español del repositorio original en ingles 
[Respositorio de rougier](https://github.com/rougier/numpy-100).
Archivos generados de manera automática. Vea la documentación para cambiar preguntas/respuestas/ayudas (questions/answers/hints)

#### 1. Importa el paquete `numpy` como `np` (★☆☆)
`hint: import … as`
#### 2. Imprima por pantalla la versión y la configuración de numpy (★☆☆)
`hint: np.__version__, np.show_config)`
#### 3. Cree un vector null de tamaño 10 (vector de zeros)(★☆☆)
`hint: np.zeros`
#### 4. Como encuentra el tamaño en memoria de un array (★☆☆)
`hint: size, itemsize`
#### 5. ¿Cómo obtiene la documentación de numpy desde la terminal (comando de línea)? (★☆☆)
`hint: np.info`
#### 6. Crea un vector de ceros de tamaño 10 cuyo valor en la quinta posición sea 1 (★☆☆)
`hint: array[4]`
#### 7. Crea un vector con sus valores contegan los números del 10 a 49 (★☆☆)
`hint: arange`
#### 8. Obrenga un vector invertido (el primer elemento se convierte en el último) (★☆☆)
`hint: array[::-1]`
#### 9. Crea una matriz 3x3 cuyos valores contengan lo números del 0 al 8 (★☆☆)
`hint: reshape`
#### 10. Encuentre los elementos cuyos índice no son cero [1,2,0,0,4,0] (★☆☆)
`hint: np.nonzero`
#### 11. Crea una matriz identidad de 3x3 (★☆☆)
`hint: np.eye`
#### 12. Crea un vector 3x3x3 con valores aleatorios (★☆☆)
`hint: np.random.random`
#### 13. Crea una matriz 10x10 con valores random y encuentra el valor máximo yel mínimo (★☆☆)
`hint: min, max`
#### 14. Crea un vector de tamaño 30 con valores aleatorios y encuentre el valor promedio (★☆☆)
`hint: mean`
#### 15. Crea un vector 2D con los valores de 1 en el borde (es decir en la primera y última filas y columnas) con valores de 0 en el interior (★☆☆)
`hint: array[1:-1, 1:-1]`
#### 16. ¿Cómo añadir un borde (llenado con ceros) a una matriz existente? (★☆☆)
`hint: np.pad`
#### 17. ¿Cuál es el resultado de la siguiente expresión? (★☆☆)
```python
0 * np.nan
np.nan == np.nan
np.inf > np.nan
np.nan - np.nan
np.nan in set([np.nan])
0.3 == 3 * 0.1
```
`hint: NaN = not a number, inf = infinity`
#### 18. Crea una matriz 5x5 con valores 1,2,3,4 justo debajo de la diagonal (★☆☆)
`hint: np.diag`
#### 19. Crea una matriz 8x8 y llénelo con un patrón similar al del tablero de ajedrez (★☆☆)
`hint: array[::2]`
#### 20. Considere un array de dimensiones (6,7,8), ¿Cuáles son los índices (x,y,z) del 100vo elemento? (★☆☆)
`hint: np.unravel_index`
#### 21. Cree algo similar a un tablero de ajedez usando la función `tile` (★☆☆)
`hint: np.tile`
#### 22. Normalice una matriz de 5x5 que contiene valores aleatorios (normalize los elementos usando la fórmula z-score) (★☆☆)
`hint: (x -mean)/std`
#### 23. Cree un tipo de dato especial (dtype) llamada color que pueda describir el color como cuatro números del tipo unsigned bytes (RGBA) (★☆☆)
Create a custom dtype that describes a color as four unsigned bytes (RGBA) (★☆☆)
`hint: np.dtype`
#### 24. Multiplique una matriz 5x3 y otra 3x2 (producto cruz) (★☆☆)
`hint:`
#### 25. Dado un array 1D, multiplica por (-1) todos los elementos que esten en el rango 3 a 8 (★☆☆)
Given a 1D array, negate all elements which are between 3 and 8, in place. (★☆☆)
`hint: >, <`
#### 26. ¿Cuál es resulatdo de la ejecución del siguiente script? (★☆☆)
```python
# Autor: Jake VanderPlas

print(sum(range(5),-1))
from numpy import *
print(sum(range(5),-1))
```
`hint: np.sum`
#### 27. Considere un vector de enteros Z, ¿Cuál de las siguientes expresiones son válidas?
Consider an integer vector Z, which of these expressions are legal? (★☆☆)
```python
Z**Z
2 << Z >> 2
Z <- Z
1j*Z
Z/1/1
Z<Z>Z
```
`No hints provided...`
#### 28. ¿Cuál es el resultado de las siguientes operaciones? (★☆☆)
```python
np.array(0) / np.array(0)
np.array(0) // np.array(0)
np.array([np.nan]).astype(int).astype(float)
```
`No hints provided...`
#### 29. ¿Cómo redondear alejado de cero en un vector con valores tipo float? (★☆☆)
Es decir que si n = -0.12  redondear a -1 y si n = 1.2 redondear a 2
How to round away from zero a float array ? (★☆☆)
`hint: np.uniform, np.copysign, np.ceil, np.abs, np.where`
#### 30. ¿Cómo encontrar valores comunes entre dos vectores? (★☆☆)
`hint: np.intersect1d`
#### 31. ¿Cómo ignorar todos los mensajes de warning de numpy (no recomendado)? (★☆☆)
`hint: np.seterr, np.errstate`
#### 32. ¿Es la siguiente expresión verdadera (True)? (★☆☆)
```python
np.sqrt(-1) == np.emath.sqrt(-1)
```
`hint: número imaginario`
#### 33. ¿Cómo obtener las fechas de ayer, hoy y mañana? (★☆☆)
`hint: np.datetime64, np.timedelta64`
#### 34. ¿Cómo obtener todas la fechas correspondientes al mes de Julio del 2016? (★★☆)
`hint: np.arange(dtype=datetime64['D'])`
#### 35. ¿Cómo calcular ((A+B)*(-A/2)) (sin usar la función `copy`)?
How to compute ((A+B)*(-A/2)) in place (without copy)? (★★☆)
`hint: np.add(out=), np.negative(out=), np.multiply(out=), np.divide(out=)`
#### 36. Extraiga la parte entera de valores positivos de un vector que contenga valores aleatorios, usando 4 diferentes métodos (★★☆)
Extract the integer part of a random array of positive numbers using 4 different methods (★★☆)
`hint: %, np.floor, astype, np.trunc`
#### 37. Crea una matriz 5x5 con sus valores dentro del rango 0 - 4 (★★☆)
Create a 5x5 matrix with row values ranging from 0 to 4 (★★☆)
`hint: np.arange`
#### 38. Cree una función que use "yield" para obtener 10 números enteros y use la función para construir un array(★☆☆)
Consider a generator function that generates 10 integers and use it to build an array (★☆☆)
`hint: np.fromiter`
#### 39. Cree un vector de tamaño 10 con los valores en el rango 0 a 1 (0 y 1 excluidos). (★★☆)
`hint: np.linspace`
#### 40. Cree un vector de tamaño 10 con valores aleatorios, luego ordénelos (★★☆).
`hint: sort`
#### 41. ¿Cómo se sumaría un pequeño vector de manera que lo haga más rapidamente que usando la función np.sum? (★★☆)
`hint: np.add.reduce`
#### 42. Considere 2 vectores A y B ¿Cómo verifica que son iguales? (★★☆)
Consider two random array A and B, check if they are equal
`hint: np.allclose, np.array_equal`
#### 43. Cree un vector inmutable (de sólo lectura) (★★☆)
Make an array immutable (read-only)
`hint: flags.writeable`
#### 44. Cree una maetriz 10x2 con elementos aleatorios,representando coordenadas cartesianas, conviertalas a coordenadas polares (★★☆).
`hint: np.sqrt, np.arctan2`
#### 45. Crea un vector con 10 elementos aleatorios y reemplace el valor máximo con 0 (★★☆)
`hint: argmax`
#### 46. Crea un vector structurado (structured array) con `x` e `y` como coordenadas, que generen un grilla (meshgrid) en el área [0, 1]x[0, 1] (★★☆)
Create a structured array with `x` and `y` coordinates covering the [0,1]x[0,1] area
`hint: np.meshgrid`
#### 47. Dados dos vectores, X, e Y, construya la matriz de Cauchy C (Cij =1/(xi - yj)) (★★☆)
`hint: np.subtract.outer`
#### 48. Imprima el máximo y mínimo valor representable para un tipo de datos de numpy escalar (★★☆)
`hint: np.iinfo, np.finfo, eps`
#### 49. ¿Cómo imprimir todos los valores de un vector? (★★☆)
(Recuerde que cuando el vector es muy grade numpy suele mostrarlos en secciones o sólo una parte)
`hint: np.set_printoptions`
#### 50. ¿Cómo encontrar el valor más cercano a un valor(valor escalar) en un vector? (★★☆)
`hint: argmin`
#### 51. Crea un vector estructurada (structured array) representado la posición (x, y) y el color (r, g, b) (★★☆)
`hint: dtype`
#### 52. Considere un vector de elementos aleatorios, de dimensiones 100x2, representado coordenadas (x, y), encuentre las distancias de entre todos los puntos en una matriz 100x100 (★★☆)
`hint: np.atleast_2d, T, np.sqrt`
#### 53. ¿Cómo convertir un vector de float(32 bits) a un vector entero (32 bits) ?
`hint: view and [:] =`
#### 54. ¿Cómo podrías convertir el siguiente texto en una matriz de numpy? (★★☆)
```
1, 2, 3, 4, 5
6,  ,  , 7, 8
 ,  , 9,10,11
```
`hint: np.genfromtxt`
#### 55. ¿Cuál es el equivalente de la función `enumerate` para vectores numpy? (★★☆)
`hint: np.ndenumerate, np.ndindex`
#### 56. Genera una matriz 2d tipo campana de Gauss (sigma = 1, mu = 0) (2D Gaussian-like array) (★★☆)
`hint: np.meshgrid, np.exp`
#### 57. ¿Cómo poner aleatoriamente p elementos en un array 2d? (★★☆)
`hint: np.put, np.random.choice`
#### 58. Dada una matriz, resta a cada elemento de una fila el promedio de la fila (★★☆)
Subtract the mean of each row of a matrix (★★☆)
`hint: mean(axis=,keepdims=)`
#### 59. ¿Cómo ordenar una matriz teniendo como referencia la n ava columna? (★★☆)
How to sort an array by the nth column? (★★☆)
`hint: argsort`
#### 60. ¿Cómo averiguar si una matriz tiene columnas nulas? (★★☆)
`hint: any, ~`
#### 61. Encuentre el valor más cercano a un valor dado en un vector (★★☆)
`hint: np.abs, argmin, flat`
#### 62. Considere 2 arrays con dimensiones (1, 3) y (3, 1), ¿Cómo calcular su suma usando un iterador? (★★☆)
Considering two arrays with shape (1,3) and (3,1), how to compute their sum using an iterator? (★★☆)
`hint: np.nditer`
#### 63. Crea un clase vector (vector class) que tenga name como atributo (★★☆)
Create an array class that has a name attribute (★★☆)
`hint: class method`
#### 64. Dado un vector Z, ¿Cómo añadir 1 a cada elemento en las posiciones dadas por otro vector I? (tenga cuidado con los índices repetidos) (★★★)
Consider a given vector, how to add 1 to each element indexed by a second vector (be careful with repeated indices)? (★★★)
`hint: np.bincount | np.add.at`
#### 65. ¿Cómo acumular (sumar) los elementos de un vector X en un vector F de acuerdo a un vector de posiciones I? (★★★)
```python
X = [1,2,3,4,5,6]
I = [1,3,9,3,4,1]
# Resultado F = [0, 7, 0, 6, 5, 0, 0, 0, 0, 3]
```
`hint: np.bincount`
#### 66. Considere un numpy array de dimensiones (w, h, 3) que representa una imagen, calcule el número de colores únicos (★★☆)
Considering a (w,h,3) image of (dtype=ubyte), compute the number of unique colors (★★☆)
`hint: np.unique`
#### 67. Considere un array de 4 dimensiones, ¿Cómo obtener la suma de las dos últimas dimensiones ó ejes? (★★★)
Considering a four dimensions array, how to get sum over the last two axis at once? (★★★)
`hint: sum(axis=(-2,-1))`
#### 68. Considere un vector unidimensional D, ¿cómo calcular los promedios de los subsets de D, si se tienen un vector S del mismo tamaño describiendo los índices de las posiciones de las cuáles deben obtenerse los promedios?(★★★)
```python
# Sea por ejemplo D
D = [0.3, 0.5, 0.2, 0.7, 1., -0.6]
# y S
S = [0, 1, 1, 2, 2, 2]
# El vector de los promedios será
R = [0.3, 0.35, 0.36667]
```
`hint: np.bincount`
#### 69. ¿Cómo obtener la diagonal de una matriz que es resultado de la operación entre dos matrices `np.dot(A, B)`? Use las matrices A y B para su respuesta.(★★★)
`hint: np.diag`
#### 70. Sea el vector [1, 2, 3, 4, 5], ¿Cómo construir un nuevo vector con 3 consecutivos zeros intercalados entre cada valor?  (★★★)
Consider the vector [1, 2, 3, 4, 5], how to build a new vector with 3 consecutive zeros interleaved between each value? (★★★)
`hint: array[::4]`
#### 71. Sea un arrays de dimensiones (5, 5, 3), cómo multiplicarlo por un array de dimensiones (5, 5)? (★★★)
`hint: array[:, :, None]`
#### 72. ¿Cómo intercambiar dos filas en un array? (★★★)
`hint: array[[]] = array[[]]`
#### 73. Sea un set de tripletes describiendo 10 triangulos (con lados compartidos), encuentre el set de las líneas que componen todos lo triangulos. (★★★)
Consider a set of 10 triplets describing 10 triangles (with shared vertices), find the set of unique line segments composing all the  triangles (★★★)
`hint: repeat, np.roll, np.sort, view, np.unique`
#### 74. Dado un array ordenado C que corresponde a el resultado de un bitcount, ¿cómo producir un array A tal que np.bincount(A) = C ? (★★★)
`hint: np.repeat`
#### 75. ¿Cómo calcular los promedios de rango variable sobre un array? (★★★)
```python
# Sea
Z = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
# Sus promedios en un rango de n = 3
[1, 2, 3, 4, 5, 6, 7, 8]
```
`hint: np.cumsum, from numpy.lib.stride_tricks import sliding_window_view (np>=1.20.0)`
#### 76. Sea un vector Z unidimensional, contruya un vector de dos dimensiones (matriz) del cuál su primera fila sea (Z[0],Z[1],Z[2]), su segunda (Z[1],Z[2],Z[3]), es decir que cada siguiente fila empiece con el segundo elementos de la anterior fila, note que (la última fila debería ser (Z[-3],Z[-2],Z[-1]) (★★★)

```python
# Sea Z y R lo que se busca
Z = [0 1 2 3 4]
R = [[0 1 2]
     [1 2 3]
     [2 3 4]]
```
`hint: from numpy.lib import stride_tricks, from numpy.lib.stride_tricks import sliding_window_view (np>=1.20.0)`
#### 77. ¿Cómo negar un valor boolean, o cambiar el signo de un valor float? (inplace) (★★★)
`hint: np.logical_not, np.negative`
#### 78. Sean dos sets puntos P0 y P1 tienen el mismo tamaño, el primer punto de P0 describe un línea con el primer punto de P1 y así con todos los elementos de P0 y P1, también se nos da un punto P. 
¿Cómo calcular la distancia del punto P a cada linea que es descrita por los pares de puntos de los sets? (★★★)
`No hints provided...`
#### 79. Sean dos sets puntos P0 y P1 tienen el mismo tamaño, el primer punto de P0 describe un línea con el primer punto de P1 y así con todos los elementos de P0 y P1, también se nos da un set de puntos P. 
¿Cómo calcular la distancia de los puntos  de P a cada linea que es descrita por los pares de puntos de los sets? (★★★)
`No hints provided...`
#### 80. Considere una matriz arbitraria, escriba una función que extraiga una subparte con una forma fija y centrada en un elemento dado (rellene con un 'fill' cuando sea necesario)(★★★)
Consider an arbitrary array, write a function that extract a subpart with a fixed shape and centered on a given element (pad with a `fill` value when necessary) (★★★)
`hint: minimum maximum`
#### 81. Sea el vector Z = [1,2,3,4,5,6,7,8,9,10,11,12,13,14], ¿Cómo generar el vector R = [[1,2,3,4], [2,3,4,5], [3,4,5,6], ..., [11,12,13,14]]? (★★★)
`hint: stride_tricks.as_strided, from numpy.lib.stride_tricks import sliding_window_view (np>=1.20.0)`
#### 82. Obtenga el rango de un matriz (★★★)
`hint: np.linalg.svd, np.linalg.matrix_rank`
#### 83. ¿Cómo encontrar el valor más frecuente en un array? (★★★)
`hint: np.bincount, argmax`
#### 84. Extraiga todos los bloques contiguos 3x3 de una matriz de elementos aleatorios 10x10 (★★★)
Extract all the contiguous 3x3 blocks from a random 10x10 matrix (★★★)
`hint: stride_tricks.as_strided, from numpy.lib.stride_tricks import sliding_window_view (np>=1.20.0)`
#### 85. Crea un matriz cuya subclase tenga Z[i,j] = Z[j,i] (★★★)
Create a 2D array subclass such that Z[i,j] == Z[j,i] (★★★)
`hint: class method`
#### 86. Consideremos un conjunto de p matrices cuya forma (n,n) y un conjunto de p vectores con forma (n,1). ¿Cómo calcular la suma de los productos de la matriz p a la vez? (el resultado tiene forma (n,1))(★★★)
Consider a set of p matrices wich shape (n,n) and a set of p vectors with shape (n,1). How to compute the sum of of the p matrix products at once? (result has shape (n,1)) (★★★)
`hint: np.tensordot`
#### 87. Sea un 16x16 array, ¿cómo obtener la suma en bloques (tamaño del bloque 4x4)? (★★★)
`hint: np.add.reduceat, from numpy.lib.stride_tricks import sliding_window_view (np>=1.20.0)`
#### 88. ¿Cómo implementar el Juego de la Vida usando numpy arrays? (★★★)
Juego de la Vida (Game Life)
Se trata de un juego de cero jugadores, lo que quiere decir que su evolución está determinada por el estado inicial y no necesita ninguna entrada de datos posterior. El "tablero de juego" es una malla plana formada por cuadrados (las "células") que se extiende por el infinito en todas las direcciones. Por tanto, cada célula tiene 8 células "vecinas", que son las que están próximas a ella, incluidas las diagonales. Las células tienen dos estados: están "vivas" o "muertas" (o "encendidas" y "apagadas"). El estado de las células evoluciona a lo largo de unidades de tiempo discretas (se podría decir que por turnos). El estado de todas las células se tiene en cuenta para calcular el estado de las mismas al turno siguiente. Todas las células se actualizan simultáneamente en cada turno, siguiendo estas reglas:
    Nace: Si una célula muerta tiene exactamente 3 células vecinas vivas "nace" (es decir, al turno siguiente estará viva).
    Muere: una célula viva puede morir por uno de 2 casos:
        Sobrepoblación: si tiene más de tres vecinos alrededor.
        Aislamiento: si tiene solo un vecino alrededor o ninguno.
    Vive: una célula se mantiene viva si tiene 2 o 3 vecinos a su alrededor.
`![Juego de la Vida](https://es.wikipedia.org/wiki/Juego_de_la_vida)`
#### 89. ¿Cómo obtener el enésimo (n-avo) valor más grande de un vector? (★★★)
`hint: np.argsort | np.argpartition`
#### 90. Dado un arbitrario número de vectores, contruya el producto cartesiano (la combinación de cada elemento con todos lo elementos) (★★★)
`hint: np.indices`
#### 91. ¿Cómo crear un registro a partir de un arrys normal? (★★★)
How to create a record array from a regular array? (★★★)
`hint: np.core.records.fromarrays`
#### 92. Dado un vector muy largo Z, calcule Z elevado a la potencia 3 usando 3 diferentes métodos (★★★)
`hint: np.power, *, np.einsum`
#### 93. Dados dos arrays A y B de tamaños (8, 3) y (2, 2) repectivamente. Cómo encontrar las fila de A que contengan elementos de cada fila de B 
Consider two arrays A and B of shape (8,3) and (2,2). How to find rows of A that contain elements of each row of B regardless of the order of the elements in B? (★★★)
`hint: np.where`
#### 94. Dada una matriz 10x3, extraiga las filas con valores no iguales (Ejemplo [2,2,3]) (★★★)
`No hints provided...`
#### 95. Convierta un vector de enteros a una matriz que represente los enteros en binario (★★★)
Convert a vector of ints into a matrix binary representation (★★★)
`hint: np.unpackbits`
#### 96. Dadas dos matrices, ¿Cómo extraer filas que sean únicas? (★★★)
Given a two dimensional array, how to extract unique rows? (★★★)
`hint: np.ascontiguousarray | np.unique`
#### 97. Considere dos vectores A y B, escriba usando `eisum` el equivalente de las funciones `inner`, `sum`, `outer` y `mul` (★★★)
Considering 2 vectors A & B, write the einsum equivalent of inner, outer, sum, and mul function (★★★)
`hint: np.einsum`
#### 98. Considere un camino descrito por dos vectores (X,Y), ¿Cómo tomar muestras del mismo usando muestras equidistantes? (★★★)
Considering a path described by two vectors (X,Y), how to sample it using equidistant samples (★★★)?
`hint: np.cumsum, np.interp`
#### 99. Dado un entero n y una matriz X, seleccione de X las filas que pueden ser interpretadas como extraídas de una distribución multinomial con n grados.
Es decir las filas que contengan enteros y que suman n. (★★★)
Given an integer n and a 2D array X, select from X the rows which can be interpreted as draws from a multinomial distribution with n degrees, 
i.e., the rows which only contain integers and which sum to n. (★★★)
`hint: np.logical_and.reduce, np.mod`
#### 100. Calcule con un intervalo de confianza del 95% el promedio de un vector X.
(es decir, volver a muestrear los elementos ddel vector N veces, calcular la media de cada muestra y luego calcular percentiles sobre los promedios). (★★★)
Compute bootstrapped 95% confidence intervals for the mean of a 1D array X 
(i.e., resample the elements of an array with replacement N times, compute the mean of each sample, and then compute percentiles over the means). (★★★)
`hint: np.percentile`