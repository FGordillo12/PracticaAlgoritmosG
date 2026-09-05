# Práctica de Laboratorio: Algoritmos Genéticos
**Universidad de Cundinamarca**  
# Ferney Gordillo y Rolando Castellanos

## Descripción del Proyecto
Este repositorio creado esta con el fin de darle solución a los problemas de optimización combinatoria y restricciones basados en el 
Problema de la Mochila presentado por el Ingeniero en la clase anterior mediante el uso de genotipos binarios.
- Estos ejercicios fueron solucionados en archivos Jupyter como lo era requerido, sin embargo inicialemnte se hicieron commits en python sin querer
por falta de atencion

* **`ejercicio_1.ipynb`**: Solución para el portafolio de inversiones con decodificación, cálculo de aptitud y penalización por exceso de presupuesto[cite: 1].
* **`ejercicio_2.ipynb`**: Solución para la selección de personal estricta, con penalización estricta por restricciones de tamaño de equipo[cite: 1].

### `ejercicio_3.ipynb`

Contiene la solución del **Ejercicio 3 - Operador de Cruzamiento de Dos Puntos**. Se modifica el operador de cruzamiento tradicional para seleccionar dos puntos aleatorios e intercambiar el segmento central entre dos cromosomas, generando dos nuevos individuos.

### `README.md`

Contiene la documentación general del proyecto, la descripción de los ejercicios, el flujo de trabajo utilizado con Git y GitHub y el análisis del efecto del factor de penalización desarrollado en el Ejercicio 4.


## 4. Ejercicio 4 - Análisis de Resultados

En el Ejercicio 1 se plantea un problema de selección de proyectos de inversión. Se tienen 10 proyectos posibles, donde cada proyecto posee un costo y un retorno esperado. El objetivo del algoritmo genético es encontrar una combinación de proyectos que permita maximizar el retorno de la inversión sin superar el presupuesto máximo establecido.

Para representar las posibles soluciones se utiliza un cromosoma binario de 10 posiciones. Cada posición representa un proyecto: el valor `1` indica que el proyecto es seleccionado, mientras que el valor `0` indica que no es seleccionado.

El presupuesto máximo establecido para el problema es de 100 unidades:

```python
PREMAXIMO = 100