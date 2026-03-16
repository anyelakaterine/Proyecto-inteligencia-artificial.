# 🤖 Proyecto de Inteligencia Artificial

## Algoritmo A*, Heurísticas y Teoría de Juegos

👩‍🎓 **Estudiante:** Anyela Katerine  
🐍 **Lenguaje utilizado:** Python  
💻 **Herramienta de desarrollo:** Google Colab / Jupyter Notebook  

# 📑 Tabla de Contenidos

1. Introducción  
2. Algoritmo A*  
3. Heurísticas  
4. Teoría de Juegos  
5. Implementación en Python  
6. Resultados  
7. Conclusiones  
8. Repositorio del proyecto  


# 📌 1. Introducción

La Inteligencia Artificial utiliza diferentes algoritmos y modelos matemáticos para resolver problemas complejos relacionados con la toma de decisiones, búsqueda de soluciones óptimas y análisis estratégico.

En este proyecto se estudian tres conceptos fundamentales dentro de la inteligencia artificial:

- Algoritmo **A\*** (A Star)
- **Heurísticas**
- **Teoría de juegos**

Primero se presenta la investigación teórica de cada concepto y posteriormente su implementación en Python, permitiendo observar de manera práctica cómo funcionan estos algoritmos en problemas de búsqueda y toma de decisiones.

El objetivo principal de este proyecto es comprender cómo estos métodos pueden aplicarse en distintos contextos como navegación, videojuegos, economía y sistemas inteligentes.



# ⭐ 2. Algoritmo A*

## 2.1 ¿Qué es el algoritmo A*?

El algoritmo **A\*** es un algoritmo de búsqueda informada ampliamente utilizado en inteligencia artificial para encontrar el camino más corto entre un nodo inicial y un nodo objetivo dentro de un grafo.

Este algoritmo combina el costo real recorrido con una estimación del costo restante hasta el objetivo, permitiendo encontrar soluciones eficientes de manera rápida.

### Aplicaciones del algoritmo A*

- 🎮 Videojuegos (búsqueda de rutas de personajes)
- 🛰️ Sistemas de navegación GPS
- 🤖 Robótica
- 📊 Sistemas de planificación automática
- 🧠 Inteligencia artificial en juegos



## 2.2 Funcionamiento del algoritmo

El algoritmo funciona evaluando los nodos disponibles y seleccionando aquel que tenga el menor costo estimado.

Para lograr esto utiliza tres funciones principales:

- **g(n)** → costo desde el nodo inicial hasta el nodo actual  
- **h(n)** → estimación del costo desde el nodo actual hasta el objetivo (heurística)  
- **f(n)** → costo total estimado del camino  

El algoritmo explora los nodos utilizando una **cola de prioridad**, siempre seleccionando el nodo con menor valor de **f(n)**.


## 2.3 Fórmula del algoritmo

La función principal del algoritmo A* es:
f(n) = g(n) + h(n)


donde:

| Función | Significado |
|-------|-------------|
| g(n) | costo acumulado desde el inicio |
| h(n) | estimación del costo restante |
| f(n) | costo total estimado |

Esta combinación permite al algoritmo explorar caminos prometedores y evitar rutas innecesarias.



## 2.4 Ejemplo conceptual

Supongamos un mapa con varias ciudades conectadas entre sí.

El algoritmo **A\*** debe encontrar la ruta más corta entre la ciudad **A** y la ciudad **F**.

Para lograrlo, analiza los costos entre ciudades y utiliza una heurística que estima la distancia restante al destino.

El algoritmo evaluará diferentes caminos y seleccionará aquel que tenga el menor costo estimado.



# 🔍 3. Heurísticas

## 3.1 ¿Qué es una heurística?

Una **heurística** es una función utilizada para estimar el costo o distancia entre un nodo actual y el nodo objetivo.

Las heurísticas ayudan a mejorar la eficiencia de los algoritmos de búsqueda, ya que permiten dirigir la exploración hacia las rutas más prometedoras.



## 3.2 ¿Para qué sirven las heurísticas?

Las heurísticas cumplen varias funciones importantes:

- Reducir el número de nodos explorados
- Acelerar los algoritmos de búsqueda
- Mejorar el rendimiento computacional
- Encontrar soluciones más eficientes

Sin heurísticas, los algoritmos de búsqueda pueden tardar mucho más tiempo en encontrar una solución.



## 3.3 ¿Cómo funcionan las heurísticas?

Las heurísticas funcionan estimando el costo restante hasta el objetivo.

Esta estimación se combina con el costo actual del camino recorrido.

El algoritmo utiliza esta información para priorizar qué nodos deben explorarse primero.

### Características de una buena heurística

- Admisible (no sobreestimar el costo real)
- Consistente
- Rápida de calcular


## 3.4 Ejemplos de heurísticas

### 1️⃣ Distancia Manhattan

Se utiliza principalmente en mapas tipo cuadrícula, como laberintos o videojuegos.
|x1 - x2| + |y1 - y2|


Esta heurística calcula la distancia en horizontal y vertical entre dos puntos.


### 2️⃣ Distancia Euclidiana

Calcula la distancia directa entre dos puntos en el plano.
√((x1-x2)² + (y1-y2)²)


Se utiliza en navegación real, robótica y sistemas de posicionamiento.



# 🎮 4. Teoría de Juegos

## 4.1 ¿Qué es la teoría de juegos?

La **teoría de juegos** es una rama de las matemáticas y la economía que estudia la toma de decisiones estratégicas entre varios participantes o jugadores.

En estos escenarios, las decisiones de un jugador afectan directamente los resultados de los demás.



## 4.2 ¿Para qué sirve?

La teoría de juegos se utiliza en múltiples áreas:

- Economía
- Política
- Inteligencia artificial
- Estrategia empresarial
- Biología evolutiva

Permite analizar cómo diferentes jugadores toman decisiones racionales en situaciones de competencia o cooperación.



## 4.3 ¿Cómo funciona?

En un modelo de teoría de juegos existen varios elementos principales:

- **Jugadores** → quienes toman decisiones
- **Estrategias** → opciones disponibles
- **Resultados** → consecuencias de las decisiones
- **Pagos** → beneficios o pérdidas

Cada jugador intenta elegir la estrategia que maximice su beneficio.



## 4.4 Ejemplos de teoría de juegos

En este proyecto se implementan tres ejemplos en Python:

1️⃣ **Dilema del prisionero**  
Dos jugadores deben decidir entre cooperar o traicionar.

2️⃣ **Piedra, papel o tijera**  
Juego clásico donde cada jugador elige una estrategia.

3️⃣ **Competencia de precios entre empresas**  
Dos empresas deciden si vender a precio alto o precio bajo.



# 💻 5. Implementación en Python

El proyecto incluye la implementación de varios algoritmos en Python.

### Algoritmo A*

El algoritmo fue implementado utilizando:

- Diccionarios
- Listas
- Colas de prioridad (`heapq`)

El algoritmo recorre el grafo evaluando los nodos disponibles y seleccionando el camino con menor costo estimado.


### Visualización del grafo

Para representar el grafo se utilizaron las librerías:

- `NetworkX`
- `Matplotlib`

Estas herramientas permiten visualizar los nodos y conexiones del grafo.



### Implementación de heurísticas

Se desarrollaron funciones para calcular:

- Distancia Manhattan
- Distancia Euclidiana

Estas funciones estiman el costo restante hasta el objetivo.



### Simulación de juegos estratégicos

Se implementaron diferentes ejemplos de teoría de juegos utilizando:

- condicionales
- generación aleatoria de decisiones



# 📊 6. Resultados

Después de ejecutar el algoritmo **A\***, el programa encuentra la ruta óptima entre el nodo inicial y el nodo objetivo.

Ejemplo de resultado:
Ruta encontrada:
A → B → E → F


Esto demuestra cómo el algoritmo evalúa diferentes caminos y selecciona el más eficiente.

Además, los ejemplos de teoría de juegos muestran cómo las decisiones de los jugadores influyen en los resultados finales.


# 🧾 7. Conclusiones

El algoritmo **A\*** es una herramienta poderosa dentro de la inteligencia artificial para resolver problemas de búsqueda de caminos.

Gracias al uso de **heurísticas**, el algoritmo puede reducir significativamente el número de nodos explorados y encontrar soluciones de manera más eficiente.

Por otro lado, la **teoría de juegos** permite analizar cómo diferentes agentes toman decisiones estratégicas en situaciones de competencia o cooperación.

La implementación práctica de estos conceptos en Python permite comprender mejor su funcionamiento y su aplicación en problemas reales.




