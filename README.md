# Market Base

[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/narratech/market-base/blob/main/notebooks/market_base.ipynb)

Asignatura: 
Grupo: 
Autores:
Nombre Alumno 1 (@usuario_github)
Nombre Alumno 2 (@usuario_github)

Este repositorio contiene el punto de partida para hacer Minería de Datos sobre un conjunto de datos sobre el catálogo de videojuegos e la tienda Steam, recorriendo las etapas de adquisición, limpieza, transformación, visualización y extracción de conocimiento para la toma de decisiones en el sector del videojuego.

## Estructura del proyecto

El repositorio sigue la siguiente arquitectura de archivos y carpetas estándar para proyectos de Ciencia de Datos:

```text
market-base/
├── data/
│   ├── raw/          # Datasets brutos descargados automáticamente (ignorado por Git)
│   └── sample/       # Muestras o datos auxiliares pequeños
├── notebooks/
│   └── market_base.ipynb  # Cuaderno principal con el análisis (Bloques A-E)
├── .gitignore        # Configuración de exclusiones de Git (evita subir datos pesados)
└── README.md         # Documentación general del repositorio

Los archivos dentro de data/raw/ (como games.csv) no se almacenan en el control de versiones debido a su tamaño. El propio cuaderno interactivo se encarga de descargarlos e importarlos automáticamente desde la Release oficial de este mismo repositorio.

## Requisitos e instalación

Para ejecutar y reproducir el análisis en un entorno local (como **Visual Studio Code** con la extensión de Python y Jupyter), se requieren las siguientes dependencias de Python (3.9+):

Asegúrate de tener instalados los paquetes principales ejecutando en tu entorno virtual o Anaconda Prompt:

### 1. Clonar el repositorio
```bash
git clone [https://github.com/tu-organizacion/tu-repositorio.git](https://github.com/tu-organizacion/tu-repositorio.git)
cd tu-repositorio

No se suben los ficheros de datos que se encuentren en data/raw y data/processed

## Bloques del estudio

A. Descarga automatizada del dataset desde la Release oficial del repositorio a data/raw/ y verificación de la estructura de datos sin desfasajes de cabecera.

B. Tratamiento de valores ausentes, transformación de cadenas de géneros/tags a listas iterables y cálculo de la métrica de tasa de positividad (filtrando juegos con más de 50 reseñas totales para evitar sesgos).

C. Análisis de frecuencia del Top 10 de géneros frente a su popularidad real y estudio estadístico de la distribución de precios en la plataforma.

D. Correlaciones y análisis temporal: Evaluación de la relación entre el precio, el volumen de reseñas y la recepción del público, sumado al estudio de la evolución histórica de lanzamientos por año.

E. Nichos de Oportunidad: Identificación de combinaciones de géneros o etiquetas poco saturadas con alta valoración media y redacción del informe de conclusiones generales de mercado.

## Referencias
* Bustos, M.: Steam Games Dataset (Kaggle).
* Valve Corporation: Steam Store.
* SteamSpy API & Analytics.
