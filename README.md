# MUAV Language

MUAV te facilita la obtención de resultados básicos diseñado para poder hacer análisis de datos básico, tales como la representación de gráficos por medio de arreglos bidimensionales y arreglos de una sola dimensión, representación de resultados con funciones tales como media, varianza, desviación estándar, moda y promedio.

## Instalación

Para poder compilar MUAV. necesitar tener Antlr v4 instalado.
Empieza la instalación de las librerías pip con los siguientes comandos:

```bash
pip install antlr4-python2-runtime
```
## Librerías
Una vez ya instalado antlr4, necesitas tener instaladas las siguientes librerías:

 * numpy
 * matplotlib
* defaultdict
* deque
* KMeans
* scipy


Puedes hacerlo manual o con los siguientes comandos:

```bash
pip install numpy
pip install matplotlib

```


Para compilar el archivo de la gramática (.g4):

1. Das click en el botón derecho del archivo MUAV.g4

2. Das click en la opcion de "Generate ANTLR recognizer"



## Usage

Siempre al inicio se debe declarar el nombre de tu programa donde dice "nombre_de_tu_programa" seguido de la palabra "program":
```bash
program "nombre_de_tu_programa";
```

Para declarar variables:
```bash
int a = 1, b = 3, c[2][3], i = 0, j = 0, x = 0;
```

Para declarar funciones:
```bash
function void nombreFuncion(int var1, int var2){
    int var3 = var1 + var2;
}
```

Para declarar un ciclo while:
```bash
 int d = 1, i = 1, s = 10;
   while(d <= i){
     s = d * s;
     d = d + 1;
   }
```

Para desplegar una gráfica:

1- Mandar la matriz

2- Título: Puedes utilizar el título que quieras solo ponerlo entre "".

3- Colores a elegir: rojo, azul, verde, amarillo, cyan y magenta.

4- Dirección a elegir: horizontal o vertical.


```bash
    matriz[0][0] = 2;
    matriz[1][0] = 4;
    matriz[2][0] = 6;


    plot(matriz, "Este es mi título", magenta, horizontal);
```

Funciones para poder hacer análisis de datos básico con las siguientes operaciones:
* Mediana
* Moda
* Media
* Varianza
* Desviación Estándar
* Valor Mínimo
* Valor Maximo

Función que regresa la Mediana de una matriz
```bash
 matriz[0][0] = 2;
 matriz[1][0] = 4;
 matriz[2][0] = 6;

getMedian(matriz); 
```

Función que regresa la Moda de una matriz
```bash
 matriz[0][0] = 2;
 matriz[1][0] = 4;
 matriz[2][0] = 6;

getModa(matriz);
```

Función que regresa la Media de una matriz
```bash
 matriz[0][0] = 2;
 matriz[1][0] = 4;
 matriz[2][0] = 6;

getMedia(matriz);
```

Función que regresa la Varianza de una matriz
```bash
 matriz[0][0] = 2;
 matriz[1][0] = 4;
 matriz[2][0] = 6;

getVar(matriz);
```

Función que regresa la Desviación Estándar de una matriz
```bash
 matriz[0][0] = 2;
 matriz[1][0] = 4;
 matriz[2][0] = 6;

getStdDev(matriz);
```

Función que regresa el Valor Mínimo de una matriz
```bash
 matriz[0][0] = 2;
 matriz[1][0] = 4;
 matriz[2][0] = 6;

getMin(matriz);
```

Función que regresa el Valor Máximo de una matriz
```bash
 matriz[0][0] = 2;
 matriz[1][0] = 4;
 matriz[2][0] = 6;

getMax(matriz);
```


Declaración del main:
```bash
main {
    /// codigo
}
```



## Developers
Alfredo Avila

Marian Muñoz
