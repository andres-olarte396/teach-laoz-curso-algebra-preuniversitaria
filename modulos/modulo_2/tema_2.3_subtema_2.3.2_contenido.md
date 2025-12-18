# Factorización por Sustitución

**Tiempo estimado**: 55 minutos  
**Nivel**: Avanzado  
**Prerrequisitos**: Todas las técnicas de factorización previas (2.1-2.3.1)

## ¿Por qué importa este concepto?

La factorización por sustitución es una **meta-técnica** que simplifica expresiones algebraicas complejas transformándolas en formas más manejables. Es como traducir un problema difícil a uno fácil, resolverlo, y traducir la respuesta de vuelta.

**Aplicaciones críticas**:

- **Ecuaciones de grado alto**: Reducir ecuaciones cuárticas (grado 4) a cuadráticas (grado 2)
- **Integrales en cálculo**: Técnica fundamental de integración por sustitución
- **Sistemas no lineales**: Simplificar sistemas de ecuaciones complejos
- **Optimización**: Simplificar funciones objetivo antes de derivar

Esta técnica es el puente entre álgebra básica y cálculo avanzado.

## Comprensión intuitiva

### Analogía: El problema del idioma extranjero

Imag

ina que tienes un problema escrito en un idioma complicado. Tu estrategia:

1. **Traducir** al español (sustitución)
2. **Resolver** en español (factorizar la forma simple)
3. **Traducir de vuelta** al idioma original (revertir sustitución)

**Ejemplo algebraico**:

- **Original complicado**: $x^4 + 5x^2 + 6$
- **Sustitución**: Llamemos $u = x^2$, entonces $x^4 = u^2$
- **Nuevo problema simple**: $u^2 + 5u + 6$
- **Factorizar**: $(u + 2)(u + 3)$
- **Revertir**: $(x^2 + 2)(x^2 + 3)$

## Definición formal

### Técnica de sustitución algebraica

Dada una expresión algebraica compleja $P(x)$ que contiene una subexpresión repetida $f(x)$:

1. **Identificar** la subexpresión $f(x)$ que aparece múltiples veces
2. **Sustituir** $u = f(x)$ para obtener $P(u)$
3. **Factorizar** $P(u)$ usando técnicas estándar
4. **Revertir** sustitución: reemplazar $u$ por $f(x)$
5. **Simplificar** (si es posible) los factores resultantes

### Criterio de aplicabilidad

La sustitución es útil cuando:

- Una expresión aparece **múltiples veces** en diferentes potencias
- La expresión resultante tras sustituir es **más simple** de factorizar
- Puedes **identificar un patrón** conocido (trinomio, diferencia de cuadrados, etc.)

## Patrones comunes de sustitución

### Patrón 1: Potencias pares (bicuadradas)

**Forma**: Expresiones con $x^4, x^2$ y constantes  
**Sustitución**: $u = x^2$

**Ejemplo**: $x^4 - 5x^2 + 4$  
$u = x^2 \Rightarrow u^2 - 5u + 4 = (u-1)(u-4) = (x^2-1)(x^2-4)$

### Patrón 2: Exponentes con proporción

**Forma**: $x^{2n}$ y $x^n$  
**Sustitución**: $u = x^n$

**Ejemplo**: $x^6 - 7x^3 - 8$  
$u = x^3 \Rightarrow u^2 - 7u - 8 = (u-8)(u+1) = (x^3-8)(x^3+1)$

### Patrón 3: Expresiones compuestas

**Forma**: $(x+a)^2$ y $(x+a)$  
**Sustitución**: $u = (x+a)$

**Ejemplo**: $(x+1)^2 - 5(x+1) + 6$  
$u = x+1 \Rightarrow u^2 - 5u + 6 = (u-2)(u-3) = (x-1)(x-2)$

## Algoritmo paso a paso

### Método general

**PASO 1**: Analizar la expresión y detectar patrones repetidos

**PASO 2**: Elegir sustitución apropiada $u = f(x)$

**PASO 3**: Reescribir toda la expresión en términos de $u$

**PASO 4**: Factorizar la expresión en $u$ usando técnicas conocidas

**PASO 5**: Sustituir $u$ de vuelta por $f(x)$

**PASO 6**: Factorizar más (si es posible) cada factor resultante

**PASO 7**: Verificar multiplicando

## Ejemplos resueltos

### Ejemplo 1: Ecuación bicuadrada básica

**Problema**: Factorizar $x^4 + x^2 - 12$

**Solución**:

```
PASO 1 - Detectar patrón:
  x⁴ y x² → potencias pares

PASO 2 - Sustitución:
  u = x²
  Entonces: x⁴ = (x²)² = u²

PASO 3 - Reescribir:
  x⁴ + x² - 12 = u² + u - 12

PASO 4 - Factorizar trinomio:
  u² + u - 12
  Buscar: producto = -12, suma = 1
  4 × (-3) = -12; 4 + (-3) = 1 ✓

  u² + u - 12 = (u + 4)(u - 3)

PASO 5 - Revertir sustitución:
  (u + 4)(u - 3) = (x² + 4)(x² - 3)

PASO 6 - Factorizar más:
  x² + 4: no factoriza en reales
  x² - 3: diferencia de cuadrados = (x - √3)(x + √3)

RESULTADO FINAL:
  x⁴ + x² - 12 = (x² + 4)(x - √3)(x + √3)

  O si prefieres factores enteros:
  x⁴ + x² - 12 = (x² + 4)(x² - 3)
```

### Ejemplo 2: Exponentes cúbicos

**Problema**: Factorizar $x^6 + 9x^3 + 8$

**Solución**:

```
PASO 1: x⁶ = (x³)², x³ aparece

PASO 2: u = x³

PASO 3: x⁶ + 9x³ + 8 = u² + 9u + 8

PASO 4: Factorizar
  u² + 9u + 8 = (u + 1)(u + 8)

PASO 5: Revertir
  (x³ + 1)(x³ + 8)

PASO 6: Ambos son suma de cubos
  x³ + 1 = (x + 1)(x² - x + 1)
  x³ + 8 = (x + 2)(x² - 2x + 4)

RESULTADO:
  x⁶ + 9x³ + 8 = (x + 1)(x² - x + 1)(x + 2)(x² - 2x + 4)
```

### Ejemplo 3: Expresión compuesta

**Problema**: Factorizar $(x^2 + 2x)^2 - 2(x^2 + 2x) - 3$

**Solución**:

```
PASO 1: (x² + 2x) aparece dos veces

PASO 2: u = x² + 2x

PASO 3: u² - 2u - 3

PASO 4: Factorizar
  u² - 2u - 3 = (u - 3)(u + 1)

PASO 5: Revertir
  (x² + 2x - 3)(x² + 2x + 1)

PASO 6: Factorizar cada trinomio
  x² + 2x - 3 = (x + 3)(x - 1)
  x² + 2x + 1 = (x + 1)²

RESULTADO:
  (x + 3)(x - 1)(x + 1)²
```

### Ejemplo 4: Sustitución con fracciones

**Problema**: Factorizar $\left(x + \frac{1}{x}\right)^2 - 5\left(x + \frac{1}{x}\right) + 6$

**Solución**:

```
PASO 1: (x + 1/x) se repite

PASO 2: u = x + 1/x

PASO 3: u² - 5u + 6

PASO 4: Factorizar
  u² - 5u + 6 = (u - 2)(u - 3)

PASO 5: Revertir
  (x + 1/x - 2)(x + 1/x - 3)

PASO 6: Simplificar cada factor
  x + 1/x - 2 = (x² - 2x + 1)/x = (x - 1)²/x
  x + 1/x - 3 = (x² - 3x + 1)/x

RESULTADO:
  [(x - 1)²/x] × [(x² - 3x + 1)/x]
  = (x - 1)²(x² - 3x + 1)/x²
```

### Ejemplo 5: Caso con dos sustituciones

**Problema**: Factorizar $(x^2 + x)^2 - 8(x^2 + x) + 12$

**Solución**:

```
PRIMERA SUSTITUCIÓN:
  u = x² + x
  u² - 8u + 12 = (u - 2)(u - 6)
  = (x² + x - 2)(x² + x - 6)

SEGUNDA FACTORIZACIÓN de cada factor:
  x² + x - 2 = (x + 2)(x - 1)
  x² + x - 6 = (x + 3)(x - 2)

RESULTADO:
  (x + 2)(x - 1)(x + 3)(x - 2)
```

## Errores comunes

❌ **Error 1**: Olvidar revertir la sustitución  
**Problema**: $x^4 - 5x^2 + 4$  
**Incorrecto**: Respuesta final $(u-1)(u-4)$ ❌  
✅ **Correcto**: $(x^2-1)(x^2-4)$ [después de revertir $u = x^2$]

❌ **Error 2**: No factorizar más los factores resultantes  
**Incorrecto**: $(x^2-1)(x^2-4)$ [detener aquí]  
✅ **Correcto**: $(x-1)(x+1)(x-2)(x+2)$ [factorizar diferencias de cuadrados]

❌ **Error 3**: Elegir sustitución incorrecta  
**Problema**: $x^4 + x^3 + 1$  
**Mal enfoque**: $u = x^2$ NO funciona (queda $x^3$ sin sustituir)  
**No todas las expresiones** se simplifican con sustitución

❌ **Error 4**: Error al reemplazar potencias  
**Problema**: $x^6 - 1$ con $u = x^2$  
**Incorrecto**: $u^6 - 1$ ❌  
✅ **Correcto**: $x^6 = (x^2)^3 = u^3$, entonces $u^3 - 1$

## Estrategias avanzadas

### Estrategia 1: Identificación de patrones

**Checklist antes de sustituir**:

1. ¿Hay una expresión que aparece en diferentes potencias?
2. ¿La sustitución elimina TODOS los términos complejos?
3. ¿La expresión resultante es MÁS SIMPLE que la original?

### Estrategia 2: Sustituciones trigonométricas (avanzado)

Para expresiones como $x^2 + y^2$ o $1 - x^2$, a veces se usan:

- $x = \sin\theta$ cuando $x^2 + y^2 = 1$
- $x = \tan\theta$ para $1 + x^2$

(Esto es más común en cálculo integral)

### Estrategia 3: Completar formas conocidas

A veces necesitas **manipular primero** para crear una expresión sustituible:

**Ejemplo**: $x^4 + x^2 + 1$

```
No es obvio, pero:
x⁴ + x² + 1 = x⁴ + 2x² + 1 - x²
           = (x²)² + 2x² + 1 - x²
           = (x² + 1)² - x²
           = (x² + 1 - x)(x² + 1 + x)   [diferencia de cuadrados]
           = (x² - x + 1)(x² + x + 1)
```

## Aplicación: Resolver ecuaciones de grado 4

**Problema**: Resolver $x^4 - 10x^2 + 9 = 0$

**Solución por sustitución**:

```
Sustitución: u = x²
  u² - 10u + 9 = 0
  (u - 1)(u - 9) = 0
  u = 1  ó  u = 9

Revertir:
  x² = 1  ⟹  x = ±1
  x² = 9  ⟹  x = ±3

Solución: x = {-3, -1, 1, 3}
```

## Comparación con otras técnicas

| Técnica                        | Cuándo usar                                   | Complejidad |
| :----------------------------- | :-------------------------------------------- | :---------- |
| **Factor común**               | Todos los términos comparten factor           | Baja        |
| **Agrupación**                 | 4+ términos sin factor común global           | Media       |
| **Trinomios**                  | Expresiones cuadráticas                       | Media       |
| **Diferencia cuadrados/cubos** | Dos términos, potencias especiales            | Baja        |
| **Sustitución**                | Expresiones de grado alto con patrón repetido | **Alta**    |

## Resumen ejecutivo

1. **Propósito**: Simplificar expresiones complejas mediante cambio de variable
2. **Método**: Identificar patrón → Sustituir → Factorizar → Revertir → Simplificar
3. **Patrones comunes**: $u = x^2$ para bicuadradas, $u = x^n$ para exponentes proporcionales
4. **Regla de oro**: SIEMPRE factorizar más los factores resultantes
5. **Verificación**: Multiplicar al final para confirmar
6. **Aplicación clave**: Resolver ecuaciones de grado 4 (cuárticas) reduciéndolas a cuadráticas

## Conexión con matemáticas avanzadas

La sustitución algebraica es preparatoria para:

- **Cálculo**: Integración por sustitución (cambio de variable en integrales)
- **Ecuaciones diferenciales**: Reducción de orden
- **Álgebra lineal**: Cambio de base
- **Geometría analítica**: Rotación de ejes

Dominar esta técnica ahora facilitará enormemente tu transición al cálculo universitario. 2. [Estrategia 2] 3. [Estrategia 3]

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
