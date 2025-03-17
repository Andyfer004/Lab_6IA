# Connect Four: Implementación de IA con Minimax y Alpha-Beta Pruning

## Introducción
Este laboratorio consiste en la implementación de una Inteligencia Artificial (IA) para jugar **Connect Four** utilizando el algoritmo **Minimax**. Se han desarrollado dos versiones: una sin optimizaciones y otra con **poda Alpha-Beta**, una técnica que mejora la eficiencia del algoritmo reduciendo la cantidad de nodos evaluados sin afectar la calidad de las decisiones.

El objetivo es analizar cómo la poda alfa-beta mejora el tiempo de ejecución sin comprometer el rendimiento del agente, y comparar el desempeño de ambas IAs en una partida autónoma.

## Desarrollo del Laboratorio
### 1. Implementación de la IA
- Se diseñó un tablero de juego con reglas básicas de **Connect Four**.
- Se implementó el algoritmo **Minimax**, que busca la mejor jugada evaluando todas las posibles secuencias de movimientos hasta una cierta profundidad.
- Se añadió una función de evaluación heurística para determinar la calidad de una jugada basada en alineaciones y control del centro.
- Se optimizó el algoritmo utilizando **poda alfa-beta**, lo que permite descartar ramas innecesarias y mejorar la eficiencia.

### 2. Modos de Juego
Se desarrollaron dos modos principales:
- **Humano vs IA:** El jugador humano realiza un movimiento y la IA responde automáticamente con su mejor jugada.
- **IA vs IA:** Un agente utiliza **Minimax sin poda** y otro usa **Minimax con poda alfa-beta**. Se asignan fichas y turnos de manera aleatoria para evaluar de forma justa cuál realiza mejores decisiones dentro del tiempo dado.

### 3. Evaluación del Desempeño
- Se realizaron partidas entre las dos versiones de la IA para comparar el impacto de la poda alfa-beta en la velocidad de decisión.
- Se midió el tiempo de ejecución de Minimax con y sin poda a diferentes profundidades para evaluar la reducción en la complejidad computacional.
- Se generó una gráfica comparativa mostrando cómo la poda alfa-beta reduce el tiempo de cómputo en función de la profundidad del árbol de búsqueda.

## Resultados Obtenidos
- **Reducción del tiempo de cómputo:** La poda alfa-beta redujo significativamente el tiempo de ejecución, permitiendo evaluar hasta el doble de profundidad en el mismo tiempo.
- **Estrategia de juego:** La IA con poda alfa-beta toma **las mismas decisiones** que la IA sin poda, pero de manera más eficiente.
- **Impacto del primer movimiento:** En **Connect Four**, el jugador que inicia suele tener ventaja, lo que influyó en los resultados de las partidas entre IAs.

## Conclusiones
Este laboratorio demostró la importancia de optimizar algoritmos de búsqueda en juegos de estrategia. La **poda alfa-beta** permitió reducir drásticamente el tiempo de ejecución sin afectar la calidad de las decisiones.

Se comprobó que, si bien la optimización mejora el rendimiento en términos de velocidad, **no influye directamente en la calidad de las jugadas**, ya que Minimax, con o sin poda, evalúa las mismas posiciones dentro de su profundidad de búsqueda.

Esta implementación es una base sólida para futuros desarrollos en IA para juegos, permitiendo aplicar técnicas más avanzadas como **redes neuronales o aprendizaje por refuerzo**.

