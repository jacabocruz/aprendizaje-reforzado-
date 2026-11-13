# Reinforcement Learning: Entorno FrozenLake-v1 con Q-Learning

Este repositorio contiene la implementación en Python del algoritmo de aprendizaje por refuerzo **Q-Learning** (*off-policy temporal difference*) aplicado al entorno matricial `FrozenLake-v1` de Gymnasium, junto con la generación del informe técnico y análisis de convergencia.

---

## 📌 Descripción del Proyecto

El objetivo principal es entrenar a un agente autónomo dentro de una grilla de $4 \times 4$ para que aprenda la política óptima $\pi^*(s)$ de navegación. El agente debe desplazarse desde la casilla de origen (**S**) hasta la casilla meta (**G**) minimizando la cantidad de pasos y evitando caer en los hoyos congelados (**H**).

### 🛠️ Características del Modelo
* **Entorno:** `FrozenLake-v1` (configuración determinista $4 \times 4$, `is_slippery=False`).
* **Algoritmo:** Q-Learning con actualización de Bellman TD(0).
* **Estrategia de Selección de Acciones:** Política $\epsilon$-greedy con decaimiento exponencial.
* **Métricas Alcanzadas:** 100% de tasa de éxito en la evaluación final y ruta óptima conseguida en 6 pasos.

---

## 📁 Estructura del Repositorio

```text
.
├── scripts/
│   └── q_learning_frozenlake.py   # Script principal de entrenamiento y evaluación
├── docs/
│   └── Informe_Reinforcement_Learning.pdf # Informe escrito completo en formato APA 7
├── data/
│   └── Tabla_Q_Optimizada_FrozenLake.xlsx # Matriz Q* exportada a Excel
├── requirements.txt               # Lista de dependencias y versiones
└── README.md                      # Guía de ejecución e información del proyecto
