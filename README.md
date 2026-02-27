# PROYECTO 3. Grafo por nodos y enlaces + coloración (método greedy)

## 1. Objetivo
Implementar un grafo con lista de adyacencia y aplicar una coloración de vértices con un método **greedy** (voraz).

## 2. Requisitos de Implementación

* **Estructura Graph:** Implementada mediante listas de adyacencia utilizando diccionarios: `{vertice: [vecinos]}`.
* **Métodos Principales:**
    * `add_vertex(v)`: Agrega un vértice al sistema.
    * `add_edge(u, v)`: Establece una relación no dirigida entre dos nodos.
    * `neighbors(v)`: Obtiene la lista de adyacencia de un nodo.
* **Algoritmo `greedy_coloring`:**
    * Asigna colores enteros (0, 1, 2...).
    * Garantiza que vértices adyacentes tengan colores distintos.
    * Retorna un diccionario `{vertice: color}`.



## 3. Estrategias de Ordenamiento
Se implementaron dos formas de procesar los vértices para el algoritmo:
1.  **Orden natural:** Basado en el identificador o nombre del nodo.
2.  **Orden por grado descendente:** Prioriza los nodos con mayor número de conexiones (grado).

## 4. Validación y Salida
El sistema incluye la función `validate_coloring(coloring)` que verifica automáticamente la integridad de la solución. La salida en consola muestra:
* Asignación individual: `vertice > color`.
* Conteo total de colores utilizados.
* Resultado de validación: **(Válida / No válida)**.



## 5. Pruebas Ejecutadas
Se realizaron tres pruebas fundamentales para comprobar el funcionamiento:
1.  **Grafo completo K4:** Verificación del número cromático en un grafo donde todos se conectan con todos.
2.  **Grafo ciclo C5:** Prueba en un ciclo impar para observar la asignación de colores.
3.  **Comparación de órdenes:** Análisis de la eficiencia entre el orden natural y el grado descendente en un mismo grafo.

---
### Datos Institucionales
**Instituto Tecnológico de Software**
**Fecha de presentación:** Viernes 27 de febrero de 2026
