# Factor Común

<<<<<<< HEAD
## Introducción
**Factor común** es un pilar fundamental en este módulo. Entender esto te permitirá conectar conceptos previos con nuevas herramientas algebraicas.

## Objetivos de Aprendizaje
1. Dominar el concepto de Factor común.
2. Identificar patrones para resolución rápida.
3. Aplicar estas técnicas en ejercicios multinivel.

## Contenido Teórico
- MCD de coeficientes
- Variable común con menor exponente
- Propiedad distributiva inversa

### Profundización
(Aquí se detalla la lógica interna de los conceptos presentados, conectando con MCD de coeficientes).

## Ejemplos Resueltos
### Ejemplo 1

**Problema**: 12x³ - 8x²

**Solución**:
```
Paso 1. MCD(12,8)=4
Paso 2: Menor exponente x²
Paso 3: Dividir cada término por 4x²

Respuesta: 4x²(3x - 2)
```

### Ejemplo 2

**Problema**: 5a³b - 15a²b² + 10ab³

**Solución**:
```
Paso 1. Factor común 5ab

Respuesta: 5ab(a² - 3ab + 2b²)
```


## Errores Comunes
❌ **Error 1**: Olvidar un término cuando el factor es igual al término: 5x/5x = 0
✅ **Correcto**: Es 1. 5x(1...)


## Estrategias de Resolución
- Identifica la estructura del problema.
- Selecciona el método más eficiente (ej. factorización vs fórmula general).
- Verifica si la solución tiene sentido en el contexto.

## Aplicaciones
- Simplificación de expresiones en Física.
- Modelado de funciones de costos/ingresos.
- Base para el Cálculo Diferencial.
=======
**Tiempo estimado**: 45 minutos  
**Nivel**: Básico/Fundamental  
**Prerrequisitos**: Operaciones con expresiones algebraicas (1.1.1), Productos notables (1.2)

## ¿Por qué importa este concepto?

La factorización por factor común es la técnica más fundamental del álgebra. Es como "deshacer" la propiedad distributiva al revés. En el mundo real, esto equivale a encontrar el denominador común en un grupo de cantidades: si tienes $3$ cajas de $x$ manzanas y $5$ cajas de $x$ manzanas, puedes expresarlo como $8$ cajas de $x$ manzanas, pero factorizar te permite ir al revés.

En ingeniería y ciencias, factorizar es esencial para:

- **Simplificar ecuaciones** antes de resolverlas (reduce complejidad computacional)
- **Optimizar código** extrayendo operaciones repetidas
- **Modelar físicamente** al extraer constantes comunes (ej: fuerza gravitacional $g$ en física)

Dominar el factor común es prerequisito para todas las técnicas avanzadas de factorización y resolución de ecuaciones cuadráticas.

## Comprensión intuitiva

### La Regla del "¿Qué tienen en común?"

Imagina que tienes estas cantidades en una bodega:

- $6$ cajas de tornillos
- $9$ cajas de clavos
- $15$ cajas de tuercas

Si cada caja pesa lo mismo, ¿cuántas cajas tienes en total? $6 + 9 + 15 = 30$ cajas.

En álgebra, si tienes:
$$6x + 9y + 15z$$

Observa que $6, 9, 15$ tienen un factor común: **todos son divisibles entre $3$**.

Factorizar es escribir:
$$6x + 9y + 15z = 3(2x + 3y + 5z)$$

Es como decir: "Tengo $3$ grupos, y en cada grupo hay $2x + 3y + 5z$".

## Definición formal

### Factor Común Numérico

Dado un polinomio con coeficientes enteros, el **factor común numérico** es el **Máximo Común Divisor (MCD)** de todos los coeficientes.

**Algoritmo de extracción**:

1. Calcular el MCD de todos los coeficientes
2. Dividir cada término entre el MCD
3. Escribir como: $\text{MCD} \times (\text{resultado de la división})$

### Factor Común Literal (Algebraico)

Dado un polinomio con variables, el **factor común literal** está formado por:

- **Cada variable** que aparece en TODOS los términos
- **Elevada al menor exponente** con el que aparece

| Expresión        | Factor Común Literal | Explicación                                          |
| :--------------- | :------------------- | :--------------------------------------------------- |
| $x^3 + x^2$      | $x^2$                | $x$ aparece en ambos, mínimo exponente es $2$        |
| $5a^2b + 10ab^2$ | $ab$                 | $a$ aparece con mín. exp. $1$, $b$ con mín. exp. $1$ |
| $3xy + 5xz$      | $x$                  | Solo $x$ está en ambos términos                      |
| $2m + 3n$        | Ninguno              | No hay variables comunes                             |

### Factor Común Total

Es el producto del **factor común numérico** y el **factor común literal**.

## Implementación práctica: Algoritmo paso a paso

### Método de extracción del factor común

**PASO 1**: Identificar el MCD de los coeficientes

**PASO 2**: Identificar las variables comunes con su menor exponente

**PASO 3**: Construir el factor común (producto de PASO 1 y PASO 2)

**PASO 4**: Dividir cada término del polinomio entre el factor común

**PASO 5**: Verificar multiplicando el factor común por el resultado

## Ejemplos resueltos

### Ejemplo 1: Factor común numérico puro

**Problema**: Factorizar $12x + 18y - 24z$

**Solución**:

```
PASO 1 - MCD de coeficientes:
  12 = 2² × 3
  18 = 2 × 3²
  24 = 2³ × 3
  MCD(12, 18, 24) = 2 × 3 = 6

PASO 2 - Variables comunes:
  12x (solo x)
  18y (solo y)
  24z (solo z)
  → NO hay variables comunes

PASO 3 - Factor común = 6

PASO 4 - Dividir cada término:
  12x ÷ 6 = 2x
  18y ÷ 6 = 3y
  24z ÷ 6 = 4z

PASO 5 - Resultado:
  12x + 18y - 24z = 6(2x + 3y - 4z)

VERIFICACIÓN:
  6(2x + 3y - 4z) = 6·2x + 6·3y + 6·(-4z) = 12x + 18y - 24z ✓
```

### Ejemplo 2: Factor común literal

**Problema**: Factorizar $5a^3b^2 + 10a^2b^3 - 15a^2b^2$

**Solución**:

```
PASO 1 - MCD numérico:
  MCD(5, 10, 15) = 5

PASO 2 - Variables comunes:
  a³b² → a con exponente 3, b con exponente 2
  a²b³ → a con exponente 2, b con exponente 3
  a²b² → a con exponente 2, b con exponente 2

  Menor exponente de a: 2
  Menor exponente de b: 2
  Factor común literal = a²b²

PASO 3 - Factor común total:
  5 × a²b² = 5a²b²

PASO 4 - Dividir:
  5a³b² ÷ 5a²b² = a
  10a²b³ ÷ 5a²b² = 2b
  15a²b² ÷ 5a²b² = 3

PASO 5 - Resultado:
  5a³b² + 10a²b³ - 15a²b² = 5a²b²(a + 2b - 3)
```

### Ejemplo 3: Caso con coeficiente negativo

**Problema**: Factorizar $-3x^4 - 6x^3 + 9x^2$

**Solución**:

```
ESTRATEGIA: Cuando el primer término es negativo,
conviene extraer el factor común negativo.

PASO 1 - MCD considerando signo:
  MCD(3, 6, 9) = 3
  Como el primer término es negativo: -3

PASO 2 - Variables comunes:
  x⁴, x³, x² → menor exponente de x es 2
  Factor común literal = x²

PASO 3 - Factor común total:
  -3x²

PASO 4 - Dividir:
  -3x⁴ ÷ (-3x²) = x²
  -6x³ ÷ (-3x²) = 2x
  9x² ÷ (-3x²) = -3

PASO 5 - Resultado:
  -3x⁴ - 6x³ + 9x² = -3x²(x² + 2x - 3)

NOTA: También es válido:
  3x²(-x² - 2x + 3)

Pero la forma con el signo negativo afuera
es más estándar en álgebra.
```

## Errores comunes

❌ **Error 1**: Olvidar el factor común literal  
**Incorrecto**: $6x^2 + 9x = 3(2x^2 + 3x)$  
✅ **Correcto**: $6x^2 + 9x = 3x(2x + 3)$  
**Diagnóstico**: No extrajiste la $x$ que es común a ambos términos

❌ **Error 2**: Usar exponente incorrecto en el factor literal  
**Incorrecto**: $x^5 + x^3 = x^3(x^2 + 1)$ ❌ (falta un término)  
✅ **Correcto**: $x^5 + x^3 = x^3(x^2 + 1)$  
**Verificación**: $x^3 \cdot x^2 = x^5$ ✓, $x^3 \cdot 1 = x^3$ ✓

❌ **Error 3**: No simplificar el MCD completamente  
**Incorrecto**: $12x + 18y = 2(6x + 9y)$ (parcial, falta seguir)  
✅ **Correcto**: $12x + 18y = 6(2x + 3y)$  
**Diagnóstico**: $6$ y $9$ siguen teniendo factor común $3$

❌ **Error 4**: Confundir el signo al extraer factor negativo  
**Incorrecto**: $-5x - 10 = -5(x + 10)$ ❌  
✅ **Correcto**: $-5x - 10 = -5(x + 2)$  
**Regla**: $-10 ÷ (-5) = +2$ (negativo entre negativo da positivo)

## Estrategias de resolución

### Estrategia 1: Detección visual rápida

**Pregunta clave**: ¿Todos los coeficientes terminan en el mismo dígito o son múltiplos de un número pequeño ($2, 3, 5$)?

- Si todos son pares → factor común mínimo es $2$
- Si todos terminan en $0$ o $5$ → factor común mínimo es $5$
- Si la suma de dígitos de cada coeficiente es múltiplo de $3$ → factor común de $3$

### Estrategia 2: Tabla de divisores

Para polinomios complejos, construye una tabla:

| Coeficiente | Divisores primos        |
| :---------- | :---------------------- |
| $24$        | $2^3 \times 3$          |
| $36$        | $2^2 \times 3^2$        |
| $60$        | $2^2 \times 3 \times 5$ |

MCD = producto de las **menores potencias comunes**: $2^2 \times 3 = 12$

### Estrategia 3: Verificación obligatoria

**SIEMPRE** multiplica tu resultado final para verificar:
$$\text{Factor común} \times \text{Paréntesis} = \text{Expresión original}$$

Si no coincide, revisa tu división término por término.

## Aplicaciones en resolución de ecuaciones

### Caso 1: Simplificar antes de resolver

**Problema**: Resolver $6x^2 + 9x = 0$

**Sin factorizar** (complicado):
$$x = \frac{-9 \pm \sqrt{81 - 0}}{12}$$ (fórmula cuadrática)

**Factorizando primero**:
$$6x^2 + 9x = 0$$
$$3x(2x + 3) = 0$$
$$x = 0 \quad \text{o} \quad 2x + 3 = 0 \Rightarrow x = -\frac{3}{2}$$

**Conclusión**: Factorizar convierte ecuaciones complejas en productos simples de resolver.

## Casos especiales

### Factor común en expresiones fraccionarias

**Problema**: Simplificar $\displaystyle\frac{15x^2 + 25x}{5x}$

**Solución**:

```
Numerador: 15x² + 25x = 5x(3x + 5)

Expresión completa:
  15x² + 25x     5x(3x + 5)
  ───────────  = ──────────  = 3x + 5
      5x             5x
```

### Factor común con coeficientes fraccionarios

**Problema**: Factorizar $\displaystyle\frac{1}{2}x + \frac{1}{4}y$

**Solución**:

```
MCD de fracciones = MCD(numeradores) / MCM(denominadores)
                  = MCD(1, 1) / MCM(2, 4)
                  = 1/4

Factor común = 1/4

1/2 x + 1/4 y = 1/4(2x + y)
```

## Resumen ejecutivo

1. **Factor común numérico** = MCD de todos los coeficientes
2. **Factor común literal** = variables comunes con menor exponente
3. **Factor común total** = producto de ambos
4. **Algoritmo**: Identificar → Extraer → Dividir → Verificar
5. **Regla de oro**: SIEMPRE verifica multiplicando el resultado
6. **Aplicación clave**: Simplifica ecuaciones antes de resolver

## Conexión con el siguiente tema

Una vez domines el factor común, podrás aplicar **factorización por agrupación** (tema 2.1.2), que es básicamente aplicar factor común a "grupos" de términos. Es como factorizar en dos etapas.
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48
