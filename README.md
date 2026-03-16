Proyecto de Inteligencia Artificial

Algoritmo A*, Heur´ısticas y Teor´ıa de Juegos

Anyela Katerine Renteria Cuama

1. Introduccion
La Inteligencia Artificial utiliza diferentes algoritmos y modelos matematicos para resolver
problemas complejos relacionados con la toma de decisiones, busqueda de soluciones optimas
y analisis estrategico.
En este proyecto se estudian tres conceptos fundamentales dentro de la inteligencia arti-
ficial:
Algoritmo A* (A Star)
Heurısticas
Teorıa de juegos

Primero se presenta la investigacion teorica de cada concepto y posteriormente su im-
plementacion en Python, permitiendo observar de manera practica como funcionan estos
algoritmos en problemas de busqueda y toma de decisiones.
El objetivo principal de este proyecto es comprender c´omo estos m´etodos pueden aplicarse
en distintos contextos como navegaci´on, videojuegos, econom´ıa y sistemas inteligentes.

2. Algoritmo A*
   
2.1. ¿Qu´e es el algoritmo A*?
El algoritmo A* es un algoritmo de b´usqueda informada ampliamente utilizado en inteli-
gencia artificial para encontrar el camino m´as corto entre un nodo inicial y un nodo objetivo
dentro de un grafo.

Este algoritmo combina el costo real recorrido con una estimaci´on del costo restante hasta
el objetivo, permitiendo encontrar soluciones eficientes de manera r´apida.
Entre sus aplicaciones se encuentran:
-Videojuegos (b´usqueda de rutas de personajes)
-Sistemas de navegaci´on GPS
-Rob´otica
-Sistemas de planificaci´on autom´atica
-Inteligencia artificial en juegos

2.2. Funcionamiento del algoritmo

El algoritmo funciona evaluando los nodos disponibles y seleccionando aquel que tenga el
menor costo estimado.
Para lograr esto utiliza tres funciones principales:
-g(n) costo desde el nodo inicial hasta el nodo actual
-h(n) estimaci´on del costo desde el nodo actual hasta el objetivo
-f (n) costo total estimado del camino

2.3. F´ormula del algoritmo
La funci´on principal del algoritmo A* se define como:
f (n) = g(n) + h(n)
donde:
-g(n) representa el costo acumulado desde el inicio
-h(n) representa la heur´ıstica o estimaci´on del costo restante
-f (n) representa el costo total estimado

2.4. Ejemplo conceptual
Supongamos un mapa con varias ciudades conectadas entre s´ı.
El algoritmo A* debe encontrar la ruta m´as corta entre la ciudad A y la ciudad F.
Para lograrlo, analiza los costos entre ciudades y utiliza una heur´ıstica que estima la
distancia restante al destino.

3. Heur´ısticas
   
3.1. ¿Qu´e es una heur´ıstica?
Una heur´ıstica es una funci´on utilizada para estimar el costo o distancia entre un nodo
actual y el nodo objetivo.
Las heur´ısticas ayudan a mejorar la eficiencia de los algoritmos de b´usqueda, ya que
permiten dirigir la exploraci´on hacia las rutas m´as prometedoras.

3.2. ¿Para qu´e sirven?
Las heur´ısticas permiten:
-Reducir el n´umero de nodos explorados
-Acelerar los algoritmos de b´usqueda
-Mejorar el rendimiento computacional
-Encontrar soluciones m´as eficientes

3.3. Ejemplos de heur´ısticas

3.3.1. Distancia Manhattan

|x1 − x2| + |y1 − y2|
Se utiliza principalmente en mapas tipo cuadr´ıcula.

3.3.2. Distancia Euclidiana

p(x1 − x2)2 + (y1 − y2)2
Esta heur´ıstica calcula la distancia directa entre dos puntos.

4. Teor´ıa de Juegos
   
4.1. ¿Qu´e es la teor´ıa de juegos?

La teor´ıa de juegos es una rama de las matem´aticas y la econom´ıa que estudia la toma
de decisiones estrat´egicas entre varios participantes o jugadores.
En estos escenarios, las decisiones de un jugador afectan directamente los resultados de
los dem´as.

4.2. ¿Para qu´e sirve?

La teor´ıa de juegos se utiliza en ´areas como:
-Econom´ıa
-Pol´ıtica
-Inteligencia artificial
-Estrategia empresarial
-Biolog´ıa evolutiva

4.3. Ejemplos

En este proyecto se implementan tres ejemplos en Python:
-Dilema del prisionero
-Piedra, papel o tijera
-Competencia de precios entre empresas

5. Implementaci´on en Python
El proyecto incluye la implementaci´on de varios algoritmos en Python.

5.1. Algoritmo A*
El algoritmo fue implementado utilizando estructuras de datos como:
-Diccionarios
-Listas
-Colas de prioridad (heapq)

5.2. Visualizaci´on del grafo
Para representar el grafo se utilizaron las librer´ıas:
-NetworkX
-Matplotlib

6. Resultados
Despu´es de ejecutar el algoritmo A*, el programa encuentra la ruta ´optima entre el nodo
inicial y el nodo objetivo.
Ejemplo:
Ruta encontrada:
A → B → E → F

8. Conclusiones
El algoritmo A* es una herramienta poderosa dentro de la inteligencia artificial para
resolver problemas de b´usqueda de caminos.
Gracias al uso de heur´ısticas, el algoritmo puede reducir significativamente el n´umero de
nodos explorados y encontrar soluciones de manera m´as eficiente.
Por otro lado, la teor´ıa de juegos permite analizar c´omo diferentes agentes toman deci-
siones estrat´egicas en situaciones de competencia o cooperaci´on.
