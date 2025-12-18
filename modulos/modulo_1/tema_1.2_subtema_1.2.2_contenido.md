# Diferencia de Cuadrados

**Tiempo estimado**: 40 minutos  
**Nivel**: Básico/Crítico  
**Prerrequisitos**: Binomio al cuadrado (1.2.1)

## ¿Por qué importa este concepto?

La diferencia de cuadrados es el único caso donde multiplicar dos binomios resulta en *menos* términos de los esperados. Es una herramienta de simplificación masiva. Se usa para racionalizar denominadores, resolver límites en cálculo, factorizar ecuaciones cuadráticas $x^2 - 9 = 0$ y simplificar fracciones algebraicas complejas. Es, esencialmente, una técnica de "eliminación quirúrgica" del término central.

## Comprensión intuitiva (Binomios Conjugados)

Si multiplicas dos binomios que son idénticos excepto por el signo del medio $(A+B)$ y $(A-B)$, ocurre algo especial.

1. Multiplicas $A \cdot A = A^2$.
2. Multiplicas $A \cdot (-B) = -AB$.
3. Multiplicas $B \cdot A = +AB$.
4. Multiplicas $B \cdot (-B) = -B^2$.

Observa el centro: $-AB + AB = 0$. ¡Se anulan mutuamente!
Solo sobreviven los extremos.

## Definición Formal

El producto de la suma por la diferencia de dos cantidades es igual a la diferencia de sus cuadrados.

### Fórmula Directa (Producto)

$$ (a + b)(a - b) = a^2 - b^2 $$

### Fórmula Inversa (Factorización)

$$ a^2 - b^2 = (a + b)(a - b) $$
Esta dirección es incluso más poderosa: convierte una resta (difícil de manejar) en un producto (fácil de simplificar).

## Implementación práctica: Algoritmos

### Dirección 1: Multiplicar Conjugados

**Problema**: $(3x + 5)(3x - 5)$
**Proceso**:

1. Identificar $a = 3x$ y $b = 5$.
2. Elevar $a$ al cuadrado: $(3x)^2 = 9x^2$.
3. Elevar $b$ al cuadrado: $5^2 = 25$.
4. Restarlos: $ 9x^2 - 25 $.
**Atajo Mental**: Cuadrado del positivo menos cuadrado del negativo.

### Dirección 2: Factorizar Diferencias

**Problema**: Factorizar $16x^4 - 81$.
**Proceso**:

1. ¿Es una resta? Sí.
2. ¿Son cuadrados perfectos?
   - $\sqrt{16x^4} = 4x^2$ (Sí)
   - $\sqrt{81} = 9$ (Sí)
3. Escribir conjugados: $(RaizA + RaizB)(RaizA - RaizB)$.
**Resultado intermedio**: $(4x^2 + 9)(4x^2 - 9)$.
**¡ALERTA!**: El segundo factor $(4x^2 - 9)$ es OTRA diferencia de cuadrados.

- $\sqrt{4x^2} = 2x$
- $\sqrt{9} = 3$
**Resultado Final**: $(4x^2 + 9)(2x + 3)(2x - 3)$.

## Análisis de Casos Complejos

### Caso 1: Orden engañoso

**Problema**: $(x + 5)(5 - x)$.
**Análisis**:

- El primer paréntesis es $(5 + x)$ (conmutativa).
- El segundo es $(5 - x)$.
- ¡Son conjugados! $a=5, b=x$.
**Resultado**: $ 25 - x^2 $. (Nota que es distinto a $x^2 - 25$).

### Caso 2: Agrupación

**Problema**: $(a + b + c)(a + b - c)$.
**Análisis**:

- Agrupamos $(a+b)$ como un solo término $X$.
- Expresión: $(X + c)(X - c)$.
- Resultado: $X^2 - c^2$.
- Expandir $X$: $(a+b)^2 - c^2$.
**Resultado Final**: $ a^2 + 2ab + b^2 - c^2 $.

## Trampas y errores comunes

### ❌ Error 1: Suma de Cuadrados

**Problema**: Factorizar $x^2 + 25$.
**Error**: Escribir $(x+5)(x+5)$ o $(x+5)(x-5)$.
**Realidad**: La **suma de cuadrados** $a^2 + b^2$ **NO SE PUEDE FACTORIZAR** en los números reales. Es "primo". (Solo se factoriza con números complejos).

### ❌ Error 2: Raíces parciales

**Problema**: Factorizar $4x^2 - 9$.
**Error**: $(4x + 3)(4x - 3)$.
**Por qué**: Olvidaron sacar la raíz al 4.
**Correcto**: $(2x + 3)(2x - 3)$.

## Resumen Ejecutivo

1. **Reconocimiento**: Busca siempre "Algo al cuadrado MENOS Algo al cuadrado".
2. **Conjugados**: Parejas $(A+B)$ y $(A-B)$. Son los mejores amigos de la racionalización.
3. **Recursividad**: Revisa siempre si el resultado se puede volver a factorizar (como en $x^4 - 1$).
4. **Suma = Pared**: $a^2 + b^2$ no se toca. Déjalo así.
