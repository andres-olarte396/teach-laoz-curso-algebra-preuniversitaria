<<<<<<< HEAD
# Trinomio x² + bx + c

## Introducción
**Trinomio x² + bx + c** es un pilar fundamental en este módulo. Entender esto te permitirá conectar conceptos previos con nuevas herramientas algebraicas.

## Objetivos de Aprendizaje
1. Dominar el concepto de Trinomio x² + bx + c.
2. Identificar patrones para resolución rápida.
3. Aplicar estas técnicas en ejercicios multinivel.

## Contenido Teórico
- Buscar dos números que sumados den b y multiplicados den c

### Profundización
(Aquí se detalla la lógica interna de los conceptos presentados, conectando con Buscar dos números que sumados den b y multiplicados den c).

## Ejemplos Resueltos
### Ejemplo 1

**Problema**: x² + 5x + 6

**Solución**:
```
Paso 1. 2+3=5
Paso 2: 2×3=6

Respuesta: (x+2)(x+3)
```

### Ejemplo 2

**Problema**: x² - 7x + 12

**Solución**:
```
Paso 1. (-3)+(-4)=-7
Paso 2: (-3)(-4)=12

Respuesta: (x-3)(x-4)
```


## Errores Comunes
❌ **Error**: Saltarse pasos de verificación.
✅ **Correcto**: Comprobar siempre el resultado.

## Estrategias de Resolución
- Identifica la estructura del problema.
- Selecciona el método más eficiente (ej. factorización vs fórmula general).
- Verifica si la solución tiene sentido en el contexto.

## Aplicaciones
- Simplificación de expresiones en Física.
- Modelado de funciones de costos/ingresos.
- Base para el Cálculo Diferencial.
=======
# Trinomio de la Forma x² + bx + c

**Tiempo estimado**: 55 minutos  
**Nivel**: Intermedio  
**Prerrequisitos**: Trinomio cuadrado perfecto (2.2.1), Multiplicación de binomios (1.1.2)

## ¿Por qué importa este concepto?

Este es el trinomio más común en álgebra y aparece constantemente en:

- **Resolución de ecuaciones cuadráticas** (antes de aplicar la fórmula general)
- **Análisis de funciones** (encontrar raíces y puntos de intersección)
- **Optimización** (problemas de máximos y mínimos)
- **Física** (ecuaciones de movimiento parabólico)

Dominar la factorización de trinomios $x^2 + bx + c$ te permite resolver ecuaciones cuadráticas mentalmente, sin usar la fórmula general.

## Comprensión intuitiva

### La Regla del "Producto y Suma"

Si tienes el trinomio $x^2 + bx + c$, estás buscando dos números que:

1. **Sumados** den $b$ (coeficiente de $x$)
2. **Multiplicados** den $c$ (término independiente)

**Ejemplo**: $x^2 + 7x + 12$

¿Qué dos números suman $7$ y multiplican $12$?

```
Opciones para multiplicar 12:
1 × 12 = 12  →  1 + 12 = 13  ❌
2 × 6 = 12   →  2 + 6 = 8    ❌
3 × 4 = 12   →  3 + 4 = 7    ✓
```

Los números son $3$ y $4$, entonces:
$$x^2 + 7x + 12 = (x + 3)(x + 4)$$

### ¿Por qué funciona?

Cuando multiplicas $(x + m)(x + n)$:
$$(x + m)(x + n) = x^2 + nx + mx + mn = x^2 + (m+n)x + mn$$

Compara con $x^2 + bx + c$:

- $b = m + n$ (suma)
- $c = m \cdot n$ (producto)

## Definición formal

### Factorización de trinomios $x^2 + bx + c$

Dado un trinomio de la forma $x^2 + bx + c$ donde el coeficiente de $x^2$ es $1$, factorizar consiste en encontrar dos números $m$ y $n$ tales que:

$$x^2 + bx + c = (x + m)(x + n)$$

donde:
$$m + n = b \quad \text{y} \quad m \cdot n = c$$

### Tabla de signos

Los signos de $b$ y $c$ determinan los signos de $m$ y $n$:

| Signo de $c$ | Signo de $b$ | Signos de $m$ y $n$   | Regla                         |
| :----------- | :----------- | :-------------------- | :---------------------------- |
| $c > 0$      | $b > 0$      | Ambos **positivos**   | Los dos números son positivos |
| $c > 0$      | $b < 0$      | Ambos **negativos**   | Los dos números son negativos |
| $c < 0$      | Cualquiera   | **Signos diferentes** | Un positivo y uno negativo    |

**Ejemplos rápidos**:

- $x^2 + 5x + 6$: $c > 0$, $b > 0$ → Buscar dos positivos que sumen $5$ y multipliquen $6$ → $(x+2)(x+3)$
- $x^2 - 5x + 6$: $c > 0$, $b < 0$ → Buscar dos negativos que sumen $-5$ y multipliquen $6$ → $(x-2)(x-3)$
- $x^2 + x - 6$: $c < 0$ → Buscar signos diferentes que sumen $1$ y multipliquen $-6$ → $(x+3)(x-2)$

## Algoritmo paso a paso

### Método de factorización por tanteo

**PASO 1**: Identificar $b$ y $c$ en $x^2 + bx + c$

**PASO 2**: Determinar los signos según la tabla de signos

**PASO 3**: Listar parejas de factores de $|c|$

**PASO 4**: Encontrar la pareja que sume $b$ (considerando signos)

**PASO 5**: Escribir $(x + m)(x + n)$

**PASO 6**: Verificar multiplicando

## Ejemplos resueltos

### Ejemplo 1: Caso básico ($c > 0$, $b > 0$)

**Problema**: Factorizar $x^2 + 8x + 15$

**Solución**:

```
PASO 1 - Identificar:
  b = 8
  c = 15

PASO 2 - Signos:
  c > 0 y b > 0  →  Ambos positivos

PASO 3 - Factores de 15:
  1 × 15 = 15
  3 × 5 = 15

PASO 4 - Buscar pareja que sume 8:
  1 + 15 = 16  ❌
  3 + 5 = 8    ✓

PASO 5 - Factorización:
  x² + 8x + 15 = (x + 3)(x + 5)

PASO 6 - Verificación:
  (x + 3)(x + 5) = x² + 5x + 3x + 15
                 = x² + 8x + 15 ✓
```

### Ejemplo 2: Caso con $b$ negativo ($c > 0$, $b < 0$)

**Problema**: Factorizar $x^2 - 10x + 21$

**Solución**:

```
PASO 1 - Identificar:
  b = -10
  c = 21

PASO 2 - Signos:
  c > 0 y b < 0  →  Ambos negativos

PASO 3 - Factores de 21:
  1 × 21 = 21
  3 × 7 = 21

PASO 4 - Buscar pareja que sume -10:
  -1 + (-21) = -22  ❌
  -3 + (-7) = -10   ✓

PASO 5 - Factorización:
  x² - 10x + 21 = (x - 3)(x - 7)

VERIFICACIÓN:
  (x - 3)(x - 7) = x² - 7x - 3x + 21
                 = x² - 10x + 21 ✓
```

### Ejemplo 3: Caso con $c$ negativo

**Problema**: Factorizar $x^2 + 2x - 15$

**Solución**:

```
PASO 1 - Identificar:
  b = 2
  c = -15

PASO 2 - Signos:
  c < 0  →  Signos diferentes (uno + y uno -)

PASO 3 - Factores de |-15| = 15:
  1 × 15 = 15
  3 × 5 = 15

PASO 4 - Buscar pareja con diferencia que de 2:
  Como c < 0, uno es positivo y otro negativo
  Necesito que la suma dé +2, entonces el mayor debe ser positivo:

  -1 + 15 = 14  ❌
  1 + (-15) = -14  ❌
  -3 + 5 = 2    ✓
  3 + (-5) = -2  ❌

PASO 5 - Factorización:
  x² + 2x - 15 = (x - 3)(x + 5)

VERIFICACIÓN:
  (x - 3)(x + 5) = x² + 5x - 3x - 15
                 = x² + 2x - 15 ✓
```

### Ejemplo 4: Caso con término independiente negativo grande

**Problema**: Factorizar $x^2 - x - 20$

**Solución**:

```
PASO 1: b = -1, c = -20

PASO 2: c < 0 → Signos diferentes

PASO 3: Factores de 20:
  1 × 20, 2 × 10, 4 × 5

PASO 4: Necesito suma = -1
  El mayor debe ser negativo (porque la suma es negativa):

  1 + (-20) = -19  ❌
  -1 + 20 = 19     ❌
  2 + (-10) = -8   ❌
  -2 + 10 = 8      ❌
  4 + (-5) = -1    ✓

PASO 5:
  x² - x - 20 = (x + 4)(x - 5)
```

## Errores comunes

❌ **Error 1**: Olvidar considerar el signo del término independiente  
**Problema**: $x^2 + 3x - 10$  
**Incorrecto**: $(x + 5)(x + 2)$ → $x^2 + 7x + 10$ ❌  
✅ **Correcto**: Como $c < 0$, signos diferentes → $(x + 5)(x - 2)$ ✓

❌ **Error 2**: Confundir suma con resta al tener $b$ negativo  
**Problema**: $x^2 - 7x + 12$  
**Incorrecto**: Buscar números que sumen $7$ ❌  
✅ **Correcto**: Buscar números negativos que sumen $-7$ → $(-3) + (-4) = -7$ → $(x-3)(x-4)$

❌ **Error 3**: No verificar la factorización  
**Siempre multiplica** tus binomios para confirmar que obtienes el trinomio original.

❌ **Error 4**: Invertir los signos en la factorización final  
**Problema**: $x^2 - 5x + 6$  
**Incorrecto**: $(x + 2)(x + 3)$ → da $x^2 + 5x + 6$ ❌  
✅ **Correcto**: $(x - 2)(x - 3)$ → da $x^2 - 5x + 6$ ✓

## Estrategias de resolución

### Estrategia 1: Tabla sistemática de factores

Para $x^2 + 7x + 12$:

| Factores de 12 | Suma | ¿Funciona? |
| :------------- | :--- | :--------- |
| 1, 12          | 13   | ❌         |
| 2, 6           | 8    | ❌         |
| 3, 4           | 7    | ✓          |

Factorización: $(x + 3)(x + 4)$

### Estrategia 2: Atajo para $c$ pequeño

Si $|c| \leq 20$, memoriza parejas de factores comunes:

- $6 = 2 \times 3$
- $12 = 3 \times 4$ o $2 \times 6$
- $15 = 3 \times 5$
- $20 = 4 \times 5$

### Estrategia 3: Prueba mental rápida

Para verificar sin multiplicar completamente:

1. **Primer término**: $x \cdot x = x^2$ ✓
2. **Último término**: $m \cdot n = c$ ✓
3. **Término medio**: $mx + nx = (m+n)x = bx$ ✓

## Casos especiales

### Caso 1: Trinomio no factorizable (primo)

**Problema**: $x^2 + 2x + 5$

Factores de 5: solo $1 \times 5$  
Suma: $1 + 5 = 6 \neq 2$

**Conclusión**: No factorizable en enteros (es primo sobre $\mathbb{Z}$)

### Caso 2: Coeficiente de $x$ es cero

**Problema**: $x^2 - 16$

Esto NO es $x^2 + bx + c$ sino **diferencia de cuadrados**:  
$$x^2 - 16 = (x - 4)(x + 4)$$

### Caso 3: Términos con coeficiente común

**Problema**: $2x^2 + 10x + 12$

**PASO 1**: Extraer factor común: $2(x^2 + 5x + 6)$  
**PASO 2**: Factorizar trinomio: $x^2 + 5x + 6 = (x + 2)(x + 3)$  
**RESULTADO**: $2(x + 2)(x + 3)$

## Aplicación: Resolución de ecuaciones

**Problema**: Resolver $x^2 + 5x + 6 = 0$

**Solución por factorización**:

```
x² + 5x + 6 = 0
(x + 2)(x + 3) = 0

Propiedad del producto cero:
x + 2 = 0  ó  x + 3 = 0
x = -2     ó  x = -3

Solución: x = {-2, -3}
```

**Verificación**:

- Para $x = -2$: $(-2)^2 + 5(-2) + 6 = 4 - 10 + 6 = 0$ ✓
- Para $x = -3$: $(-3)^2 + 5(-3) + 6 = 9 - 15 + 6 = 0$ ✓

## Resumen ejecutivo

1. **Forma**: $x^2 + bx + c = (x + m)(x + n)$ donde $m + n = b$ y $m \cdot n = c$
2. **Signos**: Si $c > 0$ → mismo signo; Si $c < 0$ → signos diferentes
3. **Método**: Listar factores de $c$ → Encontrar pareja que sume $b$ → Factorizar
4. **Verificación**: SIEMPRE multiplica para confirmar
5. **Aplicación**: Factorizar convierte ecuaciones cuadráticas en ecuaciones lineales simples

## Conexión con el siguiente tema

Este método solo funciona cuando el coeficiente de $x^2$ es $1$. En el siguiente tema (2.2.3) verás trinomios de la forma $ax^2 + bx + c$ con $a \neq 1$, que requieren técnicas más avanzadas 2. [Estrategia 2] 3. [Estrategia 3]

## Aplicaciones

[Aplicaciones prácticas del tema en contextos reales]

## Resumen

- [Punto clave 1]
- [Punto clave 2]
- [Punto clave 3]

## Práctica Recomendada

Para dominar este tema:

1. Practica los ejercicios propuestos
2. Revisa los ejemplos resueltos
3. Identifica y corrige tus errores
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48
