# Evaluación de Expresiones Algebraicas

**Tiempo estimado**: 50 minutos  
**Nivel**: Básico/Práctico  
**Prerrequisitos**: Jerarquía de operaciones (PEMDAS), Variables (0.2.1)

## ¿Por qué importa este concepto?

Evaluar una expresión es el acto de "colapsar" la abstracción a la realidad. Es cuando decimos "Ok, la fórmula de velocidad es $v = d/t$, pero ¿a qué velocidad voy SI la distancia es 100km y el tiempo 2h?". En programación, esto es **ejecutar** una función pasando parámetros. En ingeniería, es obtener el dato numérico para ver si el edificio aguanta. Sin evaluación, el álgebra se queda en papel; con evaluación, obtenemos resultados medibles.

## Comprensión intuitiva

Evaluar es **Sustituir y Calcular**.

1. **Sustituir**: Tienes un molde (la expresión) con huecos (las variables). Te dan los materiales (valores numéricos) para llenar esos huecos.
2. **Calcular**: Una vez llenos los huecos, ya no hay letras, solo números. Usas aritmética normal (PEMDAS) para hallar el resultado final.

**Analogía**: La expresión es la receta. Evaluar es cocinar el plato para 4 personas (x=4) o para 10 personas (x=10).

## Definición formal

Dada una expresión algebraica $E(x, y, ...)$ y un conjunto de valores asignados $x=a, y=b, ...$, la **evaluación** consiste en sustituir cada ocurrencia de las variables por sus valores asignados y simplificar la expresión numérica resultante hasta obtener un único número real (si está definido).

## Algoritmo de Resolución (La Regla de Oro de los Paréntesis)

Para evaluar sin errores, especialmente con números negativos, sigue este protocolo estricto:

1. **Pre-procesamiento**: Escribe la expresión original.
2. **Preparación**: Reescribe la expresión reemplazando cada variable por un **paréntesis vacío** $()$.
3. **Inserción**: Coloca el valor numérico asignado dentro de cada paréntesis.
4. **Cálculo**: Resuelve respetando PEMDAS.

### ¿Por qué paréntesis?

Para proteger los signos negativos y las potencias.
Evaluar $x^2$ para $x=-3$:

- Sin paréntesis: $-3^2 = -9$ (¡INCORRECTO! El cuadrado solo afecta al 3).
- Con paréntesis: $(-3)^2 = 9$ (¡CORRECTO! El cuadrado afecta a todo el número).

## Análisis de Casos Resueltos

### Caso 1: Polinomio Simple con Negativos

**Problema**: Evaluar $3x^2 - 5x + 2$ para $x = -2$.

**Resolución**:

1. Paréntesis vacíos: $ 3( )^2 - 5( ) + 2 $
2. Inserción: $ 3(-2)^2 - 5(-2) + 2 $
3. Potencias (PEMDAS): $(-2)^2 = 4$.
   $ 3(4) - 5(-2) + 2 $
4. Multiplicaciones: $ 3 \cdot 4 = 12 $ y $ -5 \cdot -2 = +10 $.
   $ 12 + 10 + 2 $
5. Sumas: $ 24 $

**Resultado**: $24$.

### Caso 2: Expresión Racional Multivariable

**Problema**: Evaluar $\frac{a - b}{a + b}$ para $a = \frac{1}{2}$ y $b = -\frac{1}{3}$.

**Resolución**:

1. Sustitución:
   $$ \frac{ (\frac{1}{2}) - (-\frac{1}{3}) }{ (\frac{1}{2}) + (-\frac{1}{3}) } $$
2. Simplificar signos en paréntesis:
   - Numerador: $\frac{1}{2} + \frac{1}{3}$
   - Denominador: $\frac{1}{2} - \frac{1}{3}$
3. Operar fracciones (MCM = 6):
   - Num: $\frac{3+2}{6} = \frac{5}{6}$
   - Den: $\frac{3-2}{6} = \frac{1}{6}$
4. División compleja (Sándwich):
   $$ \frac{ \frac{5}{6} }{ \frac{1}{6} } = \frac{ 5 \cdot 6 }{ 6 \cdot 1 } = 5 $$

**Resultado**: $5$.

### Caso 3: Evaluación Física (Caída Libre)

**Problema**: La altura es $h(t) = h_0 + v_0 t - 4.9t^2$.
Calcular altura para: $h_0 = 100$ m (altura inicial), $v_0 = 0$ m/s (caída libre), $t = 3$ s.

**Resolución**:

1. Sustitución:
   $ h(3) = 100 + 0(3) - 4.9(3)^2 $
2. Potencia:
   $ 100 + 0 - 4.9(9) $
3. Multiplicación:
   $ 4.9 \times 9 = 44.1 $
   $ 100 - 44.1 $
4. Resta:
   $ 55.9 $

**Interpretación**: A los 3 segundos, el objeto está a 55.9 metros del suelo.

## Trampas y errores comunes

### ❌ Error 1: Potencias de negativos

**Incorrecto**: Si $x = -4$, entonces $x^2 \to -16$.
**Correcto**: $(-4)^2 = 16$.
**Raíz del error**: Escribir $-4^2$ en la calculadora. La calculadora entiende $-(4^2)$. Tú quieres $(-4)^2$.

### ❌ Error 2: Coeficiente negativo

**Incorrecto**: Evaluar $-x$ para $x = -5 \to -5$.
**Correcto**: $-(-5) = +5$.
**Concepto**: El signo menos delante de la variable significa "el opuesto de". El opuesto de -5 es 5.

### ❌ Error 3: Distributiva ilegal en potencias

**Incorrecto**: Para evaluar $(a+b)^2$, calculan $a^2 + b^2$.
**Correcto**: Primero sumar dentro del paréntesis, luego elevar.
Si $a=3, b=4$: $(3+4)^2 = 7^2 = 49$.
(El error daría $3^2+4^2 = 9+16 = 25$).

## Resumen Ejecutivo

1. **Paréntesis siempre**: Usa paréntesis para encerrar el valor que estás sustituyendo. Es tu escudo contra errores de signo.
2. **PEMDAS estricto**: Una vez sustituido, olvida las variables, es un problema de aritmética pura.
3. **Cuidado con el menos**:
   - $x^2$ siempre es positivo (para $x$ real).
   - $-x^2$ siempre es negativo.
   - $(-x)^2$ siempre es positivo.
4. **Verificación**: Si tienes tiempo, vuelve a calcular siguiendo los pasos inversos o usando calculadora para la aritmética final.
