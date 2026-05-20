# Laboratorio 7 - Teoría de Probabilidades

## Datos del estudiante

**Nombre:** Samuel Robledo  
**Carné:** 241282  
**Curso:** MM3014 Teoría de Probabilidades  
**Laboratorio:** Laboratorio 7  

## Descripción general

Este repositorio contiene el desarrollo del Laboratorio 7 del curso de Teoría de Probabilidades. El trabajo consiste en simular el proceso de llenado de un álbum de estampas utilizando métodos de Monte Carlo y comparando los resultados obtenidos con la teoría del coleccionista.

El caso analizado se basa en un álbum de estampas del Mundial FIFA 2026, considerando sobres con una cantidad fija de estampas distintas dentro de cada sobre. A través de las simulaciones se estudia cuántos sobres se necesitan para completar un álbum reducido, cuántas estampas repetidas aparecen durante el proceso y cómo cambia la probabilidad de completar el álbum al comprar una cantidad fija de sobres.

## Contenido del repositorio

El repositorio incluye los siguientes archivos principales:

- `Mundial.ipynb`: notebook con las simulaciones, cálculos, tablas, gráficas y análisis del laboratorio.
- `Laboratorio7T`: documento en LaTeX utilizado para generar el informe formal.
- `histograma_etapa1.png`: histograma del número de sobres necesarios para completar el álbum.
- `grafica_etapa2.png`: gráfica de probabilidad de completar el álbum según la cantidad de sobres comprados.
- `README.md`: descripción general del repositorio.

## Etapas desarrolladas

### Etapa 1: Simulación básica con álbum reducido

El notebook puede ejecutarse completo usando la opción Run All en Visual Studio Code o en cualquier entorno compatible con Jupyter Notebook.

Observaciones

Los resultados obtenidos muestran que el número promedio de sobres necesarios para completar el álbum es mucho mayor que el mínimo teórico, debido a la aparición de estampas repetidas. Además, se observa que la parte final del álbum es la más difícil, ya que cuando faltan pocas estampas aumenta la probabilidad de obtener repetidas.

En esta etapa se simuló el llenado de un álbum reducido de 100 estampas, con sobres de 7 estampas cada uno. Se realizaron 10000 simulaciones para estimar la media, desviación estándar, cantidad de estampas repetidas y probabilidad de necesitar más de 30 sobres.

### Etapa 2: Probabilidad de completar el álbum

En esta etapa se evaluó la probabilidad de completar el álbum al comprar una cantidad fija de sobres. Se probaron distintos valores de sobres comprados y se calculó la proporción de simulaciones en las que el álbum fue completado.

## Herramientas utilizadas

- Python
- Jupyter Notebook
- NumPy
- Pandas
- Matplotlib
- LaTeX

## Reproducibilidad

Para que los resultados puedan reproducirse, todas las simulaciones utilizan la semilla:

```python
np.random.seed(2026)
