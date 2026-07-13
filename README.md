# Práctica 7: Investigación del Método Montecarlo

Este repositorio contiene la investigación formal, desarrollo teórico y dos ejemplos de aplicación prácticos del **Método Montecarlo** utilizando simulación computacional de números pseudoaleatorios.

---

## Estructura del Repositorio

El repositorio se organiza de la siguiente manera:

* **[metodo_montecarlo.md](metodo_montecarlo.md)**: Documento teórico detallado. Contiene el origen histórico del método (Proyecto Manhattan, Stanislaw Ulam), sus fundamentos probabilísticos (Ley de los Grandes Números y Teorema del Límite Central), el algoritmo general de simulación, la teoría sobre generadores de números pseudoaleatorios (PRNG) y una comparación técnica frente a los métodos deterministas tradicionales.
* **[ejemplo1_estimacion_pi.md](ejemplo1_estimacion_pi.md)**: Primer ejemplo práctico. Explica la aproximación geométrica de $\pi$ mediante la razón de áreas de un círculo inscrito en un cuadrado unitario, incluyendo su algoritmo detallado, una tabla de convergencia del error y su respectiva gráfica de puntos.
* **[ejemplo2_integracion_montecarlo.md](ejemplo2_integracion_montecarlo.md)**: Segundo ejemplo práctico. Describe el cálculo del área bajo la curva (integración numérica) de la función $f(x) = \sin(x)$ en el intervalo $[0, \pi]$ mediante el método *Hit-or-Miss*, mostrando el análisis de convergencia y una gráfica que clasifica los puntos aleatorios en aciertos y fallos.
* **[scripts/](scripts/)**: Directorio que aloja el código fuente ejecutable:
  * **[scripts/simulaciones.py](scripts/simulaciones.py)**: Código en Python encargado de realizar las simulaciones para los ejemplos, evaluar el comportamiento del error en diversas magnitudes de muestra ($N$) y exportar los resultados estadísticos e imágenes.
  * **[scripts/generate_pdf.py](scripts/generate_pdf.py)**: Script encargado de compilar automáticamente la teoría, las tablas de resultados de simulación y las imágenes de las gráficas en un archivo PDF final estilizado de entrega.
* **[img/](img/)**: Carpeta que contiene las gráficas generadas dinámicamente por las simulaciones:
  * **[img/pi_estimation.png](img/pi_estimation.png)**: Distribución de puntos aleatorios en el plano cartesiano para la estimación de $\pi$.
  * **[img/integration_montecarlo.png](img/integration_montecarlo.png)**: Clasificación gráfica de aciertos y fallos para la integral definida de $\sin(x)$.
* **[Practica_7_Metodo_Montecarlo.pdf](Practica_7_Metodo_Montecarlo.pdf)**: Reporte consolidado definitivo de la investigación, el cual incluye una hoja de presentación/portada institucional, índice automático de secciones y formato impreso unificado.

---

