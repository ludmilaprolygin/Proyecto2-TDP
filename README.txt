La disposición de la numeración de las filas, columnas y paneles es la siguiente.

     c0   c1   c2     c3   c4   c5     c6   c7   c8  
   +-------------------------------------------------
f0 |  0    0    0   |  1    1    1  |   2    2    2
f1 |  0    0    0   |  1    1    1  |   2    2    2
f2 |  0    0    0   |  1    1    1  |   2    2    2
   +----------------+---------------+----------------
f3 |  3    3    3   |  4    4    4  |   5    5    5
f4 |  3    3    3   |  4    4    4  |   5    5    5
f5 |  3    3    3   |  4    4    4  |   5    5    5
   +----------------+---------------+----------------
f6 |  6    6    6   |  7    7    7  |   8    8    8
f7 |  6    6    6   |  7    7    7  |   8    8    8
f8 |  6    6    6   |  7    7    7  |   8    8    8


Los índices se obtuvieron haciendo la suma de la división entera entre el número de fila y 3 y, el prodcuto entre la división entera entre el número de columna y tres, con tres.
Simbólicamente: 3*(fila/3) + (columna/3).

Asimismo, teniendo los números de fila y columna de un índice particular de la matriz, se pueden obtener la primera fila y columna de ese panel restandole el resto de la divión entera entre el número de fila/columna y tres, al número de fila/columna.
Simbólicamente: f=fila - fila%3; c=columna - columna%3;

Por otro lado, teniendo el número de panel, se pueden obtener los primeros índices del panel correspondiente controlando el resto de la division entera entre el n´´umero de panel y 3.
Simbólicamente: Si nroPanel%3 == i, i=0, 1 o 2; c = 3*(nroPanel%3); f = nroPanel - nroPanel%3.
