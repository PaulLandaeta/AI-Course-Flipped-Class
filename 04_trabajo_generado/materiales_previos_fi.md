# Guía de estudio previo: matrices, determinantes y sistemas lineales

**Tiempo máximo:** 25 minutos.

**Alcance:** esta guía prepara el trabajo activo de la unidad; no reemplaza la resolución, comparación de métodos ni la retroalimentación de la clase.

## 1. Propósito de la preparación

Llegar a clase con un punto de partida común para reconocer una matriz de coeficientes, calcular determinantes sencillos y organizar la resolución de sistemas lineales. Durante la sesión se aplicarán, compararán y justificarán métodos de resolución.

## 2. Conocimientos previos necesarios

- Operaciones aritméticas con números reales: suma, resta, multiplicación y división.
- Manejo de ecuaciones lineales sencillas con una incógnita.
- Lectura de pares ordenados en el plano cartesiano.

## 3. Contenido esencial

### Matriz y sistema lineal

Un sistema lineal agrupa ecuaciones cuyas incógnitas aparecen en primer grado. Por ejemplo:

\[
\begin{cases}
x+y=5\\
x-y=1
\end{cases}
\]

puede representarse mediante la matriz de coeficientes

\[
\begin{pmatrix}1 & 1\\1 & -1\end{pmatrix}.
\]

### Determinante de una matriz 2x2

Para una matriz

\[
A=\begin{pmatrix}a & b\\c & d\end{pmatrix},
\]

su determinante se calcula como \(\det(A)=ad-bc\).

**Tomado del sílabo:** se estudiarán determinantes, sus propiedades y fórmulas para matrices 2x2 y 3x3; además, sistemas lineales mediante métodos gráfico, sustitución, eliminación, Cramer, Gauss-Jordan, matriz inversa y descomposición LU.

**Requiere verificación docente:** la introducción explícita a “matriz de coeficientes” y la secuencia inicial de la unidad fueron propuestas en el rediseño, pues las sesiones 1 y 2 del documento base estaban destinadas a otra materia.

## 4. Dos ejemplos

### Ejemplo 1: calcular un determinante

\[
A=\begin{pmatrix}3 & 2\\1 & 4\end{pmatrix}
\]

\[
\det(A)=(3)(4)-(2)(1)=12-2=10.
\]

La evidencia del cálculo es mostrar las dos multiplicaciones diagonales y la resta final.

### Ejemplo 2: resolver un sistema por sustitución

\[
\begin{cases}
x+y=5\\
x-y=1
\end{cases}
\]

De la segunda ecuación, \(x=1+y\). Al sustituir en la primera:

\[
(1+y)+y=5 \Rightarrow 2y=4 \Rightarrow y=2.
\]

Entonces \(x=1+2=3\). Verificación:

\[
3+2=5 \quad \text{y} \quad 3-2=1.
\]

Por lo tanto, la solución es \((x,y)=(3,2)\).

## 5. Autoverificación

Responde sin consultar una solución modelo:

1. Calcula \(\det\begin{pmatrix}2 & 5\\1 & 3\end{pmatrix}\). ¿Qué operaciones realizaste?
2. Escribe la matriz de coeficientes del sistema \(2x+y=7\), \(x-3y=4\).
3. Si obtienes una solución para un sistema de dos ecuaciones, ¿qué sustituciones debes hacer para verificarla?

## 6. Pregunta para llevar a clase

> ¿Qué características del sistema o de sus coeficientes me ayudan a decidir si conviene usar sustitución, eliminación, regla de Cramer o un método matricial?

## 7. Advertencia: errores frecuentes

- En \(ad-bc\), no se suman los productos diagonales: se resta el segundo al primero.
- Una matriz de coeficientes contiene solo los coeficientes de las incógnitas, no el término independiente.
- Una solución no se considera validada hasta reemplazar sus valores en **ambas** ecuaciones originales.
- Al despejar una incógnita, revisa con cuidado los signos antes de sustituir.

## 8. Fuentes utilizadas

**Fuentes listadas en el sílabo:**

- Grossman, S. (1992). *Álgebra lineal con aplicaciones*.
- Lay, D. (2001). *Álgebra lineal y sus aplicaciones*.
- Anton, H. (1994). *Elementary Linear Algebra. Elementary Linear Algebra Applications*.

**Nota de verificación docente:** el sílabo no indica capítulos ni páginas específicas de estas obras. El docente debe asignar el fragmento o recurso autorizado que corresponda a determinantes y sistemas lineales antes de distribuir esta guía.
