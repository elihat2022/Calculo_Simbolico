# Cálculo Simbólico con SymPy

Este notebook demuestra el uso de la biblioteca SymPy para realizar operaciones de cálculo simbólico en Python.

## Contenido

### 1. Cálculo de Límites

Se utiliza la función $f(x)=\frac{1}{x+1}$ como ejemplo para calcular:

- Límites cuando $x \to \infty$
- Límites cuando $x \to -1$
- Límites laterales (por la izquierda)

**Métodos utilizados:**
- `sympy.Limit()` - Para definir límites
- `.doit()` - Para evaluar el límite

### 2. Cálculo de Derivadas

Se utiliza la función $f(x)=\frac{3x^3 + 17x^2 + 6x + 1}{2x^3 -x +3}$ para demostrar:

- Primera derivada usando `sympy.Derivative()`
- Segunda derivada usando `sympy.diff()`
- Resolución de ecuaciones con `sympy.solve()`
- Simplificación de expresiones con `sympy.simplify()`

### 3. Derivadas Parciales

Usando la función $f(x,y) = \sin^2x+\cos^2y$ se calculan:

- Derivada parcial con respecto a $x$
- Derivada parcial con respecto a $y$

### 4. Cálculo de Integrales

Se demuestra el cálculo de integrales indefinidas con la función $f(x) = kx$:

- Integral indefinida usando `sympy.Integral()`

### 5. Cálculo de Integrales Definidas

Se calculan integrales definidas (áreas bajo la curva entre dos límites):

- Integral definida de $x^2$ de 0 a 2
- Integral definida de $\sin(x)$ de 0 a $\pi$
- Evaluación usando `sympy.Integral(f, (x, a, b)).doit()`

## Requisitos

```python
import sympy 
from sympy.plotting import plot
from IPython.display import display, Math
```

## Características Principales

- **Visualización:** Uso de gráficos con `sympy.plotting.plot()`
- **Renderizado LaTeX:** Uso de `display(Math())` para mostrar fórmulas matemáticas de forma legible
- **Manipulación simbólica:** Operaciones algebraicas exactas sin aproximaciones numéricas

## Uso

Ejecuta las celdas secuencialmente para ver los ejemplos de cada operación de cálculo simbólico.
