# README

El código se ha implementado con Python 3.11, y el entorno de desarrollo utilizado es Jupyter Notebook. Todos los scripts de este trabajo tienen este formato, e incluyen comentarios acerca del código.

Los ficheros Jupyter Notebook se dividen en dos carpetas, uno por cada dataset utilizado (CICIDS2017 y UNSW-NB15). En cada una de estas carpetas el código se organiza en ficheros de forma completamente análoga, 
aunque para cada dataset el código implementado es sensiblemente distinto.

En los ficheros **CICIDS_preproc.ipynb** y **UNSW-NB15_preproc.ipynb** se incluye el código necesario para el preprocesamiento inicial de los datos, el análisis estadístico de
los mismos, y el estudio de la importancia de los parámetros en cada caso. Tras la ejecución de este código, se habrán generado los ficheros CSV (tanto para cada tipo de
ataque como para el conjunto total de datos, en ambos casos ambos ya preprocesados) que se utilizarán en las siguientes fases de ejecución.

En los ficheros **CICIDS_attacks_sup.ipynb** y **UNSW-NB15_attacks_sup.ipynb** se incluye el código para la implementación de los sistemas de detección de anomalías distinguiendo por 
cada tipo de ataque, utilizando 12 algoritmos distintos de aprendizaje
automático supervisado. Para poder ejecutar este código, es necesario que se hayan
generado los ficheros CSV por cada tipo de ataque. Al ejecutar las celdas de código de
este fichero, se obtendrán los resultados de rendimiento por cada tipo de ataque y cada
algoritmo.

En los ficheros **CICIDS_attacks_unsup.ipynb** y **UNSW-NB15_attacks_unsup.ipynb** se
incluye el código para la implementación de los sistemas de detección de anomalías
distinguiendo por cada tipo de ataque, utilizando 4 algoritmos distintos de aprendizaje
automático no supervisado. Para poder ejecutar este código, es necesario que se hayan
generado los ficheros CSV por cada tipo de ataque. Al ejecutar las celdas de código de
este fichero, se obtendrán los resultados de rendimiento por cada tipo de ataque y cada
algoritmo.

En los ficheros **CICIDS_all_sup.ipynb** y **UNSW-NB15_all_sup.ipynb** se incluye el código para la implementación de los sistemas de detección de anomalías sobre el conjunto total de datos, 
utilizando 12 algoritmos distintos de aprendizaje automático supervisado. Para poder ejecutar este código, es necesario que se hayan generado los
ficheros CSV con todos los datos preprocesados. Se distinguen a su vez dos configuraciones distintas de parámetros, una combinando los parámetros más importantes
por cada tipo de ataque (18 parámetros para CICIDS2017 y 12 para UNSW-NB15), y
otra seleccionando los 7 más importantes sobre el conjunto total. Al ejecutar las celdas de código de este fichero, se obtendrán los resultados de rendimiento para ambos
enfoques y cada algoritmo.

En los ficheros **CICIDS_all_unsup.ipynb** y **UNSW-NB15_all_unsup.ipynb** se incluye
el código para la implementación de los sistemas de detección de anomalías sobre el
conjunto total de datos, utilizando 4 algoritmos distintos de aprendizaje automático
no supervisado. Para poder ejecutar este código, es necesario que se hayan generado
los ficheros CSV con todos los datos preprocesados. Se distinguen a su vez dos configuraciones distintas de parámetros, una combinando los parámetros más importantes por cada tipo de 
ataque (18 parámetros para CICIDS2017 y 12 para UNSW-NB15),
y otra seleccionando los 7 más importantes sobre el conjunto total. Al ejecutar las celdas de código de este fichero, se obtendrán los resultados de rendimiento para ambos
enfoques y cada algoritmo.
