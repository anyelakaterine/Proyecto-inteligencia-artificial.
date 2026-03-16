# 🤖 Proyecto de Inteligencia Artificial
## Algoritmo A*, Heurísticas y Teoría de Juegos

**Estudiante:** Anyela Katerine Renteria Cuama  



# 1. Introducción

La Inteligencia Artificial utiliza diferentes algoritmos y modelos matemáticos para resolver problemas complejos relacionados con la toma de decisiones, búsqueda de soluciones óptimas y análisis estratégico.

En este proyecto se estudian tres conceptos fundamentales dentro de la inteligencia artificial:

- Algoritmo A* (A Star)  
- Heurísticas  
- Teoría de juegos  

Primero se presenta la investigación teórica de cada concepto y posteriormente su implementación en Python, permitiendo observar de manera práctica cómo funcionan estos algoritmos en problemas de búsqueda y toma de decisiones.

El objetivo principal de este proyecto es comprender cómo estos métodos pueden aplicarse en distintos contextos como navegación, videojuegos, economía y sistemas inteligentes.



# 2. Algoritmo A*

## 2.1 ¿Qué es el algoritmo A*?

El algoritmo A* es un algoritmo de búsqueda informada ampliamente utilizado en inteligencia artificial para encontrar el camino más corto entre un nodo inicial y un nodo objetivo dentro de un grafo.

Este algoritmo combina el costo real recorrido con una estimación del costo restante hasta el objetivo, permitiendo encontrar soluciones eficientes de manera rápida.

Entre sus aplicaciones se encuentran:

- Videojuegos (búsqueda de rutas de personajes)  
- Sistemas de navegación GPS  
- Robótica  
- Sistemas de planificación automática  
- Inteligencia artificial en juegos  



## 2.2 Funcionamiento del algoritmo

El algoritmo funciona evaluando los nodos disponibles y seleccionando aquel que tenga el menor costo estimado.

Para lograr esto utiliza tres funciones principales:

- $g(n)$ → costo desde el nodo inicial hasta el nodo actual  
- $h(n)$ → estimación del costo desde el nodo actual hasta el objetivo  
- $f(n)$ → costo total estimado del camino  



## 2.3 Fórmula del algoritmo

La función principal del algoritmo A* se define como:

$$
f(n) = g(n) + h(n)
$$

donde:

- $g(n)$ representa el costo acumulado desde el inicio  
- $h(n)$ representa la heurística o estimación del costo restante  
- $f(n)$ representa el costo total estimado  



## 2.4 Ejemplo conceptual

Supongamos un mapa con varias ciudades conectadas entre sí.

El algoritmo A* debe encontrar la ruta más corta entre la ciudad **A** y la ciudad **F**.

Para lograrlo, analiza los costos entre ciudades y utiliza una heurística que estima la distancia restante al destino.



# 3. Heurísticas

## 3.1 ¿Qué es una heurística?

Una heurística es una función utilizada para estimar el costo o distancia entre un nodo actual y el nodo objetivo.

Las heurísticas ayudan a mejorar la eficiencia de los algoritmos de búsqueda, ya que permiten dirigir la exploración hacia las rutas más prometedoras.



## 3.2 ¿Para qué sirven?

Las heurísticas permiten:

- Reducir el número de nodos explorados  
- Acelerar los algoritmos de búsqueda  
- Mejorar el rendimiento computacional  
- Encontrar soluciones más eficientes  



## 3.3 Ejemplos de heurísticas

### 3.3.1 Distancia Manhattan

$$
|x_1 - x_2| + |y_1 - y_2|
$$

Se utiliza principalmente en mapas tipo cuadrícula.



### 3.3.2 Distancia Euclidiana

$$
\sqrt{(x_1 - x_2)^2 + (y_1 - y_2)^2}
$$

Esta heurística calcula la distancia directa entre dos puntos.



# 4. Teoría de Juegos

## 4.1 ¿Qué es la teoría de juegos?

La teoría de juegos es una rama de las matemáticas y la economía que estudia la toma de decisiones estratégicas entre varios participantes o jugadores.

En estos escenarios, las decisiones de un jugador afectan directamente los resultados de los demás.



## 4.2 ¿Para qué sirve?

La teoría de juegos se utiliza en áreas como:

- Economía  
- Política  
- Inteligencia artificial  
- Estrategia empresarial  
- Biología evolutiva  



## 4.3 Ejemplos

En este proyecto se implementan tres ejemplos en Python:

- Dilema del prisionero  
- Piedra, papel o tijera  
- Competencia de precios entre empresas  



# 5. Implementación en Python

El proyecto incluye la implementación de varios algoritmos en Python.


## 5.1 Algoritmo A*

El algoritmo fue implementado utilizando estructuras de datos como:

- Diccionarios  
- Listas  
- Colas de prioridad (`heapq`)  



## 5.2 Visualización del grafo

Para representar el grafo se utilizaron las librerías:

- NetworkX  
- Matplotlib  



# 6. Resultados

Después de ejecutar el algoritmo A*, el programa encuentra la ruta óptima entre el nodo inicial y el nodo objetivo.

Ejemplo:
Ruta encontrada:
A → B → E → F




# 7. Conclusiones

El algoritmo A* es una herramienta poderosa dentro de la inteligencia artificial para resolver problemas de búsqueda de caminos.

Gracias al uso de heurísticas, el algoritmo puede reducir significativamente el número de nodos explorados y encontrar soluciones de manera más eficiente.

Por otro lado, la teoría de juegos permite analizar cómo diferentes agentes toman decisiones estratégicas en situaciones de competencia o cooperación.

