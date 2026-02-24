# Frozen Lake MDP - Value Iteration

Este proyecto contiene una implementación desde cero del entorno **Frozen Lake** y el algoritmo de **Value Iteration** (Iteración de Valores), utilizados en el aprendizaje por refuerzo y Procesos de Decisión de Markov (MDP).

El objetivo principal es resolver el problema de encontrar la ruta óptima desde un punto de inicio (Start) hasta una meta (Goal) en un mapa cuadriculado de hielo resbaladizo, mitigando el riesgo de caer en los agujeros (Holes).

## 🚀 Características

La implementación principal se encuentra en el Jupyter Notebook `frozen_lake.ipynb`, el cual está estructurado en las siguientes fases:

- **Modelado del MDP (Task 2.1)**: Definición de la clase base con sus estados, acciones, función de transiciones $T(s, a, s')$ (incorporando la estocasticidad del hielo) y la función de recompensa $R(s, a, s')$.
- **Value Iteration (Task 2.2)**: Implementación de la ecuación de Bellman para el cálculo iterativo de los valores óptimos de cada estado $V^*(s)$, y la extracción de su política óptima $\pi^*(s)$.
- **Visualización y Resultados**: Generación visual de un mapa de calor ilustrando en el grid (4x4) el valor asignado de cada celda incluyendo flechas direccionales que dictan la ruta y las acciones idóneas.

## 🛠️ Tecnologías y Dependencias

Para mantener un enfoque didáctico y matemático, la simulación se desarrolló íntegramente desde cero apoyándose únicamente en utilidades matemáticas y de graficación en Python:

- Python 3
- [NumPy](https://numpy.org/) (Operaciones vectoriales y matrices)
- [Pandas](https://pandas.pydata.org/) (Estructuración de datos)
- [Matplotlib](https://matplotlib.org/) (Generación visual y Heatmap)
- [Jupyter Notebook](https://jupyter.org/) (Entorno interactivo)

## ⚙️ Cómo probar y ejecutar el código

1. Asegúrate de tener Python y pip instalados en tu sistema.
2. Descarga o clona el repositorio localmente.
3. Verifica tener instaladas las dependencias gráficas y analíticas (si no las tienes, instálalas usando tu entorno virtual preferido o directamente global):
   ```bash
   pip install numpy pandas matplotlib jupyter
   ```
4. Ubícate en este directorio desde la terminal, e inicializa Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Abre el archivo interactivo `frozen_lake.ipynb` y ejecuta todas las celdas en orden.

## 📄 Estructura del directorio

```text
Frozen-Lake/
│
├── frozen_lake.ipynb     # Notebook principal con la simulación completa
├── README.md             # Documentación general y guía de usuario
└── .gitignore            # Archivos locales de sistema excluidos por Git
```
