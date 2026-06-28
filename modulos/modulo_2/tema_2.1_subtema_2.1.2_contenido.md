# Agrupación de Términos

<<<<<<< HEAD
## Introducción
**Agrupación de términos** es un pilar fundamental en este módulo. Entender esto te permitirá conectar conceptos previos con nuevas herramientas algebraicas.

## Objetivos de Aprendizaje
1. Dominar el concepto de Agrupación de términos.
2. Identificar patrones para resolución rápida.
3. Aplicar estas técnicas en ejercicios multinivel.

## Contenido Teórico
- Agrupar parejas con factor común
- Factor común polinomio

### Profundización
(Aquí se detalla la lógica interna de los conceptos presentados, conectando con Agrupar parejas con factor común).

## Ejemplos Resueltos
### Ejemplo 1

**Problema**: ax + ay + bx + by

**Solución**:
```
Paso 1. a(x+y) + b(x+y)
Paso 2: Factor común (x+y)

Respuesta: (a+b)(x+y)
```

### Ejemplo 2

**Problema**: x³ + x² + 2x + 2

**Solución**:
```
Paso 1. x²(x+1) + 2(x+1)

Respuesta: (x+1)(x²+2)
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
**Tiempo estimado**: 50 minutos  
**Nivel**: Básico/Intermedio  
**Prerrequisitos**: Factor común (2.1.1), Operaciones con polinomios (1.1)

## ¿Por qué importa este concepto?

La agrupación de términos es una técnica de factorización para polinomios de **4 o más términos** que no tienen un factor común obvio en todos ellos, pero que pueden organizarse estratégicamente en grupos más pequeños donde sí existe factor común.

Es como organizar una bodega desordenada: si no puedes encontrar un patrón global, agrupa por categorías y luego busca patrones dentro de cada categoría.

**Aplicaciones reales**:

- **Optimización de código**: Agrupar operaciones similares reduce cálculos redundantes
- **Simplificación de circuitos**: Agrupar componentes con comportamiento similar
- **Álgebra de ecuaciones**: Primer paso para resolver ecuaciones polinómicas de grado alto

## Comprensión intuitiva

### Analogía: Organizando una biblioteca

Imagina que tienes estos libros mezclados:

- 3 libros de matemáticas en español
- 5 libros de física en español
- 3 libros de matemáticas en inglés
- 5 libros de física en inglés

**Estrategia de agrupación**:

**Opción 1 - Agrupar por idioma**:

- (3 matemáticas ES + 5 física ES) + (3 matemáticas EN + 5 física EN)
- Factor común por grupo: Idioma español y idioma inglés

**Opción 2 - Agrupar por materia**:

- (3 matemáticas ES + 3 matemáticas EN) + (5 física ES + 5 física EN)
- Factor común por grupo: Matemáticas y Física

En álgebra, **buscamos la agrupación que revele factores comunes**.

### Ejemplo algebraico introductorio

Factoriza: $ax + ay + bx + by$

**No hay factor común global** (no todos los términos tienen $a$, $b$, $x$, o $y$).

**Agrupamos en pares**:
$$(ax + ay) + (bx + by)$$

**Extraemos factor común de cada grupo**:
$$a(x + y) + b(x + y)$$

**¡Ahora vemos un nuevo factor común!**: $(x + y)$ aparece en ambos grupos.

**Factorizamos nuevamente**:
$$(x + y)(a + b)$$

## Definición formal

### Método de factorización por agrupación

Técnica aplicable a polinomios de **4 o más términos** mediante el siguiente algoritmo:

1. **Verificar**: No existe factor común global
2. **Agrupar**: Dividir el polinomio en grupos (usualmente pares o tercias)
3. **Factorizar cada grupo**: Extraer factor común de cada uno
4. **Factorizar el binomio resultante**: El factor común de los factores comunes

### Criterio de agrupabilidad

Un polinomio es factorizable por agrupación si:
$$P(x) = t_1 + t_2 + t_3 + t_4$$
donde al agrupar en pares $(t_1 + t_2)$ y $(t_3 + t_4)$, ambos grupos tienen:

- Factor común extraíble
- El resultado de ambas factorizaciones tiene un factor común

## Algoritmo paso a paso

### Método estándar para 4 términos

**PASO 1**: Verificar que NO hay factor común en los 4 términos

**PASO 2**: Agrupar en dos pares (usualmente los dos primeros y los dos últimos)

**PASO 3**: Extraer factor común de cada par

**PASO 4**: Factorizar el factor común resultante

**PASO 5**: Verificar multiplicando

## Ejemplos resueltos

### Ejemplo 1: Agrupación directa (caso ideal)

**Problema**: Factorizar $2x^2 + 6x + xy + 3y$

**Solución**:

```
PASO 1 - Verificar factor común global:
  No hay variable o número común a los 4 términos

PASO 2 - Agrupar en pares:
  (2x² + 6x) + (xy + 3y)

PASO 3 - Factor común de cada grupo:
  Primer grupo: 2x² + 6x = 2x(x + 3)
  Segundo grupo: xy + 3y = y(x + 3)

  Resultado: 2x(x + 3) + y(x + 3)

PASO 4 - Factor común final:
  Ambos tienen (x + 3)

  2x(x + 3) + y(x + 3) = (x + 3)(2x + y)

PASO 5 - Verificación:
  (x + 3)(2x + y) = x·2x + x·y + 3·2x + 3·y
                  = 2x² + xy + 6x + 3y
                  = 2x² + 6x + xy + 3y ✓
```

### Ejemplo 2: Requiere cambio de signo

**Problema**: Factorizar $3a - 3b + xa - xb$

**Solución**:

```
PASO 1 - Verificar: No hay factor común global

PASO 2 - Agrupar:
  (3a - 3b) + (xa - xb)

PASO 3 - Factor común por grupo:
  Primer grupo: 3a - 3b = 3(a - b)
  Segundo grupo: xa - xb = x(a - b)

  Resultado: 3(a - b) + x(a - b)

PASO 4 - Factor común:
  (a - b)(3 + x)

VERIFICACIÓN:
  (a - b)(3 + x) = 3a + ax - 3b - bx
                 = 3a - 3b + ax - bx
                 = 3a - 3b + xa - xb ✓
```

### Ejemplo 3: Agrupación con ajuste de signos

**Problema**: Factorizar $xy - 2y - 5x + 10$

**Solución**:

```
PASO 1 - Verificar: No hay factor común global

PASO 2 - Agrupación inicial:
  (xy - 2y) + (-5x + 10)

PASO 3 - Factor común por grupo:
  Primer grupo: xy - 2y = y(x - 2)
  Segundo grupo: -5x + 10 = -5(x - 2)
                          o también: 5(-x + 2)

  Para que coincidan, uso: -5(x - 2)

  Resultado: y(x - 2) - 5(x - 2)

PASO 4 - Factor común:
  (x - 2)(y - 5)

VERIFICACIÓN:
  (x - 2)(y - 5) = xy - 5x - 2y + 10
                 = xy - 2y - 5x + 10 ✓
```

### Ejemplo 4: Agrupación no obvia (requiere reordenar)

**Problema**: Factorizar $ac + bd + ad + bc$

**Solución**:

```
INTENTO 1 - Agrupación directa:
  (ac + bd) + (ad + bc)
  → No hay factor común en el primer grupo (a,c vs b,d)

ESTRATEGIA: Reordenar términos
  ac + bd + ad + bc = ac + ad + bc + bd

INTENTO 2 - Nueva agrupación:
  (ac + ad) + (bc + bd)

  Primer grupo: ac + ad = a(c + d)
  Segundo grupo: bc + bd = b(c + d)

  Resultado: a(c + d) + b(c + d)

FACTOR COMÚN:
  (c + d)(a + b)

VERIFICACIÓN:
  (c + d)(a + b) = ac + ab + cd + bd
                 = ac + bd + ad + bc ✓ (reordenando)
```

## Errores comunes

❌ **Error 1**: No verificar que los factores comunes parciales coincidan  
**Incorrecto**: $ax + ay + bx + by = a(x + y) + b(x + y) = ?$ [se detiene aquí]  
✅ **Correcto**: Continúa extrayendo $(x + y)$ → $(x + y)(a + b)$

❌ **Error 2**: No ajustar signos al extraer factor negativo  
**Incorrecto**: $x - 3 + xy - 3y = (x - 3) + y(x - 3) = (x - 3)(1 + y)$  
✅ **Correcto**: Segundo grupo debe ser $y(x - 3)$ → $(x - 3)(1 + y)$ ✓  
**Diagnóstico**: Al verificar: $(1 + y)(x - 3) = x - 3 + xy - 3y$ ✓

❌ **Error 3**: No reordenar términos cuando la agrupación inicial falla  
**Problema**: $am + bn + an + bm$  
**Mal enfoque**: $(am + bn) + (an + bm)$ → No funciona  
✅ **Reordenar**: $am + an + bm + bn = a(m + n) + b(m + n) = (m + n)(a + b)$

❌ **Error 4**: Olvidar verificar al final  
**Siempre multiplica** tu respuesta final para confirmar que obtienes el polinomio original.

## Estrategias de resolución

### Estrategia 1: Diagrama de términos

Para $ax + bx + ay + by$, crea una tabla:

|     | $x$  | $y$  |
| --- | ---- | ---- |
| $a$ | $ax$ | $ay$ |
| $b$ | $bx$ | $by$ |

Esto te ayuda a ver que puedes factorizar por filas: $a(x + y) + b(x + y)$

### Estrategia 2: Prueba múltiples agrupaciones

Si la primera agrupación no funciona, intenta:

- Agrupar primero y tercero, segundo y cuarto
- Reordenar términos completamente
- Buscar patrones de productos notables ocultos

### Estrategia 3: Caso con 6 términos

Para polinomios de 6 términos, agrupa en **tercias** en lugar de pares:

**Ejemplo**: $ax^2 + bx^2 + ay^2 + by^2 + az^2 + bz^2$

Agrupa por coeficientes:
$$(ax^2 + ay^2 + az^2) + (bx^2 + by^2 + bz^2)$$
$$= a(x^2 + y^2 + z^2) + b(x^2 + y^2 + z^2)$$
$$= (x^2 + y^2 + z^2)(a + b)$$

## Casos especiales

### Caso 1: Tres términos con agrupación oculta

**Problema**: $x^2 + 3x + xy + 3y$

**Solución**:

```
Aunque parece trinomio, son 4 términos
  = (x² + 3x) + (xy + 3y)
  = x(x + 3) + y(x + 3)
  = (x + 3)(x + y)
```

### Caso 2: Polinomio con término cuadrático

**Problema**: $x^2 - 4x + xy - 4y$

**Solución**:

```
  = (x² - 4x) + (xy - 4y)
  = x(x - 4) + y(x - 4)
  = (x - 4)(x + y)
```

## Aplicación: Resolución de ecuaciones

**Problema**: Resolver $x^3 + 2x^2 - 9x - 18 = 0$

**Solución por agrupación**:

```
  x³ + 2x² - 9x - 18 = 0

  Agrupar: (x³ + 2x²) + (-9x - 18) = 0

  Factor común: x²(x + 2) - 9(x + 2) = 0

  Factorizar: (x + 2)(x² - 9) = 0

  Diferencia de cuadrados: (x + 2)(x - 3)(x + 3) = 0

  Soluciones: x = -2, x = 3, x = -3
```

## Resumen ejecutivo

1. **Agrupación** se usa cuando NO hay factor común global en todos los términos
2. **Método**: Agrupar → Factor común parcial → Factor común total
3. **Clave**: Los factores comunes parciales deben coincidir
4. **Si falla**: Reordena los términos y vuelve a intentar
5. **Verificación**: SIEMPRE multiplica para comprobar
6. **Aplicación**: Útil para factorizar antes de resolver ecuaciones

## Conexión con el siguiente tema

La agrupación es preparatoria para factorizar **trinomios cuadráticos** (tema 2.2), donde a veces necesitas "crear" un cuarto término para poder agrupar. Esta técnica se llama "factor por agrupación con trinomios".
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48
