# Explicación Sencilla: Estimación de $\pi$ (Método de Montecarlo)

Imagina que este problema es como **jugar a los dardos con los ojos vendados**. A través de este juego, podemos descubrir el valor de $\pi$ usando solo el azar y la geometría básica.

---

## 1. El Escenario del Juego
Imagina que tienes una pared con un **cuadrado pintado** y, justo adentro y bien centrado, hay un **blanco circular** (un círculo cuyos bordes tocan exactamente los lados del cuadrado).

* El área de todo el **cuadrado** es igual a **4**.
* El área del **círculo** interior es exactamente igual a **$\pi$** (aproximadamente 3.1416).

---

## 2. La Regla del Juego
Empiezas a lanzar dardos al cuadrado de forma completamente aleatoria. Como no estás apuntando (tienes los ojos vendados), algunos dardos van a caer **dentro del círculo** y otros van a caer **fuera del círculo** (pero todos dentro del cuadrado).

La lógica nos dice lo siguiente: 
> Si el círculo ocupa la mayor parte del cuadrado, **la gran mayoría de los dardos deberían caer dentro del círculo**.

Matemáticamente, la probabilidad de que un dardo caiga dentro del círculo depende de qué tan grande es el círculo en comparación con el cuadrado completo:

$$\text{Probabilidad} = \frac{\text{Área del Círculo}}{\text{Área del Cuadrado}} = \frac{\pi}{4}$$

---

## 3. El Truco para Descubrir $\pi$
Como nuestro objetivo es averiguar cuánto vale $\pi$, podemos despejar la fórmula matemática anterior. Si pasamos el 4 multiplicando, obtenemos:

$$\pi = 4 \times \text{Probabilidad}$$

Para calcular esa probabilidad en el mundo real, simplemente hacemos el experimento de lanzar muchos dardos y contar los resultados:

$$\pi \approx 4 \times \frac{\text{Dardos DENTRO del círculo}}{\text{Total de dardos lanzados}}$$

---

## 4. ¿Cómo sabe la computadora dónde cayó el dardo?
Cada dardo cae en una coordenada $(x, y)$. Para saber si está dentro del círculo, la computadora calcula la distancia desde el centro del tablero hasta el punto donde se clavó el dardo (usando algo muy similar al Teorema de Pitágoras):

$$d^2 = x^2 + y^2$$

* Si el resultado es **menor o igual a 1**: ¡El dardo está **DENTRO** del círculo! (Se cuenta para la aproximación).
* Si el resultado es **mayor a 1**: El dardo está **FUERA** del círculo (en las esquinas del cuadrado).

---

## 5. La Clave: La Ley de los Grandes Números
¿Qué pasa cuando empezamos a lanzar dardos?

* **Si lanzas 100 dardos:** El azar puede hacer que falles muchos o aciertes demasiados por pura suerte. Tu estimación de $\pi$ podría ser tosca (por ejemplo, `3.08`).
* **Si lanzas 1,000,000 de dardos:** La suerte individual ya no influye tanto. La proporción de dardos se vuelve increíblemente exacta y el resultado se estabiliza muy cerca del valor real de $\pi$ (`3.1415...`).

A este método de usar la aleatoriedad (el azar) para resolver problemas matemáticos se le conoce en la ciencia como **Método de Montecarlo** (en honor al famoso casino de Mónaco).
