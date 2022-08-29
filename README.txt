-----INSTRUCCIONES DE EJECUCIÓN-----

1 - Para compilar ejecutar "make" en la terminal (por defecto ya hay un ejecutable en /bin),
por lo que no es necesario compilar.

2 - Para ejecutar el programa ir a la terminal y ejecutar "./bin/p2 <seed> <parametro>" donde
<seed> es la semilla que elijamos y
<parametro> puede ser:
		-> 1: en cuyo caso ejecutaremos conjunto de datos spectf-heart
		-> 2: conjunto de datos parkinsons
		-> 3: conjunto de datos ionosphere

--- Cualquier otra ejecucion dará error ---

[NOTA] -> Se adjunta script para una ejecución más cómoda de los resultados en ficheros de texto, el script en cuestión es "script_acp.sh".
Se puede ejecutar concurrentemente todos los conjuntos de datos (lo cuál hace que los tiempos invidivuales de cada programa sean mayores, pero que en conjunto es más rápido a la hora de obtener resultados).
Si por el contrario se desea, se puede ejecutar secuencialmente. Todo ello queda especificado en el propip script.
