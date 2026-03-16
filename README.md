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

- **g(n)** → costo desde el nodo inicial hasta el nodo actual  
- **h(n)** → estimación del costo desde el nodo actual hasta el objetivo  
- **f(n)** → costo total estimado del camino  



## 2.3 Fórmula del algoritmo

La función principal del algoritmo A* se define como:

