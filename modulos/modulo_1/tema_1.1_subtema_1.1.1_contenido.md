# Suma y Resta de Expresiones Algebraicas

**Tiempo estimado**: 50 minutos  
**Nivel**: Básico/Fundamental  
**Prerrequisitos**: Operaciones con enteros (0.1.1), Variables (0.2.1)

## ¿Por qué importa este concepto?

En el mundo real, no sumamos "números", sumamos "cosas". Si eres ingeniero de logística, sumas "cajas de tipo A" con "cajas de tipo A", pero no puedes sumarlas con "litros de combustible". El álgebra formaliza esto con el concepto de **términos semejantes**. La suma y resta algebraica es la base de la simplificación de modelos: reduce un problema gigante de 50 variables a uno manejable de 3 variables.

## Comprensión intuitiva (La Regla de las Manzanas)

El álgebra es estricta con las categorías.

- $3$ manzanas + $2$ manzanas = $5$ manzanas. ($3x + 2x = 5x$)
- $3$ manzanas + $2$ peras = $3$ manzanas y $2$ peras. ($3x + 2y = 3x + 2y$)

No puedes mezclar categorías. En álgebra, la "categoría" viene definida por **las letras y sus exponentes exactos**.

- $x$ es una categoría.
- $x^2$ es OTRA categoría distinta (una línea vs un cuadrado). NO se pueden sumar.

## Definición formal

### Términos Semejantes

Dos o más términos son **semejantes** si comparten exactamente la misma **parte literal**:

1. Mismas variables.
2. Mismos exponentes para cada variable.

| Término 1 | Término 2 | ¿Semejantes? | Por qué |
| :--- | :--- | :--- | :--- |
| $3x^2$ | $-5x^2$ | ✅ SÍ | Ambos son $x^2$. Solo cambia cuánto hay. |
| $2xy$ | $7yx$ | ✅ SÍ | El orden en multiplicacion no importa ($xy = yx$). |
| $4x^2$ | $4x$ | ❌ NO | Exponentes distintos (2 vs 1). |
| $3a^2b$ | $3ab^2$ | ❌ NO | Exponentes cruzados ($a$ cuadrado vs $b$ cuadrado). |

### Reducción de Términos

Operación que consiste en sumar o restar los **coeficientes** de los términos semejantes y mantener la parte literal intacta.
$$ ax^n + bx^n = (a+b)x^n $$

## Implementación práctica: Algoritmo de Simplificación

### Suma de Polinomios

1. **Eliminar paréntesis**: Si hay un signo $+$ antes, los signos internos NO cambian.
2. **Identificar semejantes**: Agrupar mentalmente o visualmente.
3. **Operar coeficientes**: Sumar/restar los números.

**Ejemplo**: Sumar $(3x^2 - 5x + 2) + (x^2 + 7x - 8)$.

1. Liberar: $ 3x^2 - 5x + 2 + x^2 + 7x - 8 $
2. Agrupar:
   - $x^2$: $3 + 1 = 4$
   - $x$: $-5 + 7 = +2$
   - Constantes: $2 - 8 = -6$
3. Resultado: $ 4x^2 + 2x - 6 $

### Resta de Polinomios (¡Peligro!)

El signo menos **afecta a todo** lo que sigue.

1. **Eliminar paréntesis**: Si hay un signo $-$ antes, **invertr TODOS** los signos internos.
2. **Identificar y Operar**.

**Ejemplo**: Restar $(5a - 2b) - (2a - 6b + c)$.

1. Liberar: $ 5a - 2b \mathbf{-2a + 6b - c} $ (Nota el cambio de signos).
2. Agrupar:
   - $a$: $5 - 2 = 3$
   - $b$: $-2 + 6 = +4$
   - $c$: Solo hay $-c$.
3. Resultado: $ 3a + 4b - c $

## Análisis de Casos Complejos

### Caso 1: Semejanza oculta

**Problema**: Simplificar $ \frac{1}{2}xy + 0.3yx - xy $.
**Análisis**:

- Todos son términos de $xy$ (recordar $yx = xy$).
- Coeficientes: $\frac{1}{2}$ (0.5), $0.3$, y $-1$.
**Operación**:
$$ 0.5 + 0.3 - 1 = 0.8 - 1 = -0.2 $$
**Resultado**: $ -0.2xy $

### Caso 2: Signos anidados

**Problema**: $ 3x - [2y - (5x - y)] $.
**Resolución (de adentro hacia afuera)**:

1. Eliminar paréntesis redondo (cambio signos):
   $ 3x - [2y - 5x + y] $
2. Simplificar corchete:
   $ 2y + y = 3y \to [3y - 5x] $
   Expresión: $ 3x - [3y - 5x] $
3. Eliminar corchete (cambio signos):
   $ 3x - 3y + 5x $
4. Simplificar final:
   $ 3x + 5x = 8x $
**Resultado**: $ 8x - 3y $.

## Trampas y errores comunes

### ❌ Error 1: El "Menos" perezoso

**Incorrecto**: $ -(3x + 5) = -3x + 5 $
**Por qué falla**: El estudiante solo cambió el signo del primer término.
**Correcto**: $ -3x - 5 $. El negativo se debe distribuir a TODOS.

### ❌ Error 2: Sumar exponentes

**Incorrecto**: $ x^2 + x^2 = x^4 $
**Por qué falla**: Confusión con la regla de multiplicación ($x \cdot x = x^2$). En la suma, "manzanas más manzanas son manzanas", no "super-manzanas".
**Correcto**: $ x^2 + x^2 = 2x^2 $.

### ❌ Error 3: Desaparición de variables

**Incorrecto**: $ 5x - 5x = 0x \to $ (lo dejan vacío)
**Correcto**: Es 0.
**Pero**: $ 5x - 4x = 1x $ (o simplemente $x$). A veces olvidan poner la $x$.

## Aplicaciones Reales

### Inventarios

Una tienda tiene stock inicial $S$, ventas $V$ y devoluciones $D$.
Polinomio de flujo: $ (100x + 50y) - (20x + 10y) + (2x + y) $.
Si no simplificamos, tenemos que calcular 6 términos. Simplificado: $ 82x + 41y $. Mucho más eficiente.

### Física (Suma de Fuerzas)

En el eje X actúan: $F_1 = 30\cos(30^\circ)i$, $F_2 = -10i$.
Sumar fuerzas es simplemente reducir términos semejantes (los que tienen el vector unitario $i$).

## Resumen Ejecutivo

1. **Solo suma iguales**: Peras con peras ($x$ con $x$).
2. **Parte literal intocable**: Al sumar, los exponentes NO cambian.
3. **El signo menos es traicionero**: Cuando veas un "-" delante de un paréntesis, ALERTA ROJA: cambia todos los signos de adentro.
4. **Orden**: Escribe el resultado ordenado por potencia (descendente) o alfabéticamente para mayor claridad.
