# Trinomio de la Forma ax² + bx + c (Trinomio General)

**Tiempo estimado**: 65 minutos  
**Nivel**: Intermedio/Avanzado  
**Prerrequisitos**: Trinomio x²+bx+c (2.2.2), Agrupación (2.1.2), Factor común (2.1.1)

## ¿Por qué importa este concepto?

Este es el **trinomio más general** en álgebra, donde el coeficiente de $x^2$ es diferente de $1$. Aparece en:

- **Física avanzada**: Ecuaciones de trayectorias con aceleración variable
- **Economía**: Modelos de oferta y demanda cuadráticos
- **Ingeniería**: Análisis de circuitos RLC, vibraciones mecánicas
- **Estadística**: Regresión polinomial cuadrática

Factorizar trinomios generales es más desafiante pero esencial para resolver ecuaciones cuadráticas complejas sin depender siempre de la fórmula general.

## Comprensión intuitiva

### El Problema del Coeficiente $a$

Cuando tenías $x^2 + 7x + 12$, buscabas dos números que sumaran $7$ y multiplicaran $12$.

Pero con $2x^2 + 7x + 6$, el coeficiente $2$ complica todo porque:
$$(px + m)(qx + n) = pqx^2 + (pn + qm)x + mn$$

Ahora necesitas encontrar **cuatro números** ($p, q, m, n$) tales que:

- $p \cdot q = 2$ (coeficiente de $x^2$)
- $m \cdot n = 6$ (término independiente)
- $pn + qm = 7$ (coeficiente de $x$)

**Hay dos métodos principales para resolverlo:**

## Método 1: Factorización por Agrupación (AC)

### Concepto clave

Convertir el trinomio $ax^2 + bx + c$ en un polinomio de 4 términos que se pueda factorizar por agrupación.

### Algoritmo del Método AC

**Nombre**: "AC" porque multiplicas $a \times c$

**PASO 1**: Calcular $A \cdot C$ (producto del primer y último coeficiente)

**PASO 2**: Buscar dos números $m$ y $n$ tales que:

- $m \cdot n = A \cdot C$
- $m + n = B$ (coeficiente del término medio)

**PASO 3**: Reescribir $bx$ como $mx + nx$

**PASO 4**: Factorizar por agrupación

**PASO 5**: Verificar

### Ejemplo del método AC

**Problema**: Factorizar $2x^2 + 7x + 6$

**Solución**:

```
PASO 1 - Calcular A·C:
  a = 2, c = 6
  A·C = 2 × 6 = 12

PASO 2 - Buscar dos números:
  Necesito: m·n = 12  y  m + n = 7

  Factores de 12:
  1 × 12:  1 + 12 = 13  ❌
  2 × 6:   2 + 6 = 8    ❌
  3 × 4:   3 + 4 = 7    ✓

  m = 3, n = 4

PASO 3 - Reescribir el término medio:
  2x² + 7x + 6 = 2x² + 3x + 4x + 6

PASO 4 - Agrupar y factorizar:
  = (2x² + 3x) + (4x + 6)
  = x(2x + 3) + 2(2x + 3)
  = (2x + 3)(x + 2)

PASO 5 - Verificación:
  (2x + 3)(x + 2) = 2x² + 4x + 3x + 6
                  = 2x² + 7x + 6 ✓
```

## Método 2: Ensayo y Error (Prueba y Error)

### Concepto

Probar sistemáticamente diferentes combinaciones de binomios hasta encontrar la correcta.

### Estrategia del Método

Para $ax^2 + bx + c$:

1. **Factorizar** $a$ en dos números: $a = p \cdot q$
2. **Factorizar** $c$ en dos números: $c = m \cdot n$
3. **Probar** combinaciones de la forma $(px + m)(qx + n)$
4. **Verificar** si el término medio coincide

### Ejemplo del método de ensayo

**Problema**: Factorizar $3x^2 + 10x + 8$

**Solución**:

```
Factores de a = 3: 1 × 3 (no hay más opciones)
Factores de c = 8: 1×8, 2×4

Posibles factorizaciones:

INTENTO 1: (3x + 1)(x + 8)
  Término medio: 3x·8 + 1·x = 24x + x = 25x  ❌

INTENTO 2: (3x + 8)(x + 1)
  Término medio: 3x·1 + 8·x = 3x + 8x = 11x  ❌

INTENTO 3: (3x + 2)(x + 4)
  Término medio: 3x·4 + 2·x = 12x + 2x = 14x  ❌

INTENTO 4: (3x + 4)(x + 2)
  Término medio: 3x·2 + 4·x = 6x + 4x = 10x  ✓

RESPUESTA: 3x² + 10x + 8 = (3x + 4)(x + 2)
```

## Ejemplos resueltos completos

### Ejemplo 1: Método AC con coeficiente negativo

**Problema**: Factorizar $6x^2 - 11x + 3$

**Solución**:

```
Método AC:

PASO 1: A·C = 6 × 3 = 18

PASO 2: Buscar m·n = 18 y m + n = -11
  Como ambos negativos (c > 0, b < 0):
  -2 × -9 = 18;  -2 + (-9) = -11  ✓
  m = -2, n = -9

PASO 3: Reescribir:
  6x² - 11x + 3 = 6x² - 2x - 9x + 3

PASO 4: Agrupar:
  = (6x² - 2x) + (-9x + 3)
  = 2x(3x - 1) - 3(3x - 1)
  = (3x - 1)(2x - 3)

VERIFICACIÓN:
  (3x - 1)(2x - 3) = 6x² - 9x - 2x + 3
                   = 6x² - 11x + 3 ✓
```

### Ejemplo 2: Término independiente negativo

**Problema**: Factorizar $2x^2 + x - 15$

**Solución**:

```
Método AC:

PASO 1: A·C = 2 × (-15) = -30

PASO 2: Buscar m·n = -30 y m + n = 1
  Signos diferentes (c < 0):
  -5 × 6 = -30;  -5 + 6 = 1  ✓
  m = -5, n = 6

PASO 3: Reescribir:
  2x² + x - 15 = 2x² - 5x + 6x - 15

PASO 4: Agrupar:
  = (2x² - 5x) + (6x - 15)
  = x(2x - 5) + 3(2x - 5)
  = (2x - 5)(x + 3)
```

### Ejemplo 3: Coeficiente grande

**Problema**: Factorizar $12x^2 + 17x + 6$

**Solución**:

```
Método AC:

PASO 1: A·C = 12 × 6 = 72

PASO 2: Buscar m·n = 72 y m + n = 17
  Factores de 72: muchos, buscar sistemáticamente
  8 × 9 = 72;  8 + 9 = 17  ✓

PASO 3: 12x² + 17x + 6 = 12x² + 8x + 9x + 6

PASO 4:
  = (12x² + 8x) + (9x + 6)
  = 4x(3x + 2) + 3(3x + 2)
  = (3x + 2)(4x + 3)
```

### Ejemplo 4: Con factor común previo

**Problema**: Factorizar $6x^2 + 24x + 18$

**Solución**:

```
PASO 1: Extraer factor común
  MCD(6, 24, 18) = 6
  6x² + 24x + 18 = 6(x² + 4x + 3)

PASO 2: Factorizar trinomio simple
  x² + 4x + 3 = (x + 1)(x + 3)

RESULTADO FINAL:
  6x² + 24x + 18 = 6(x + 1)(x + 3)
```

## Errores comunes

❌ **Error 1**: Olvidar buscar factor común primero  
**Problema**: $4x^2 + 12x + 8$  
**Mal enfoque**: Aplicar método AC directamente (complicado)  
✅ **Correcto**: $4(x^2 + 3x + 2) = 4(x+1)(x+2)$

❌ **Error 2**: Error en signos al agrupar  
**Problema**: $2x^2 - 5x + 3 = 2x^2 - 2x - 3x + 3$  
**Incorrecto**: $= 2x(x - 1) - 3(x + 1)$ [factores no coinciden]  
✅ **Correcto**: $= 2x(x - 1) - 3(x - 1) = (x-1)(2x-3)$

❌ **Error 3**: Equivocar el orden en el método de ensayo  
**Problema**: $2x^2 + 5x + 2$  
**Incorrecto**: $(2x + 1)(x + 2) = 2x^2 + 5x + 2$... [¡coincide!]  
**Pero también**: $(x + 2)(2x + 1)$ [mismo resultado]  
**Clave**: El orden del producto no importa en la respuesta final

❌ **Error 4**: No verificar al final  
**SIEMPRE** multiplica tu factorización para confirmar

## Comparación de métodos

| Aspecto                     | Método AC   | Ensayo y Error |
| :-------------------------- | :---------- | :------------- |
| **Sistemático**             | ✅ Sí       | ⚠️ Parcial     |
| **Rápido para $a$ pequeño** | ⚠️ Moderado | ✅ Sí          |
| **Rápido para $a$ grande**  | ✅ Sí       | ❌ No          |
| **Requiere agrupación**     | ✅ Sí       | ❌ No          |
| **Fácil de enseñar**        | ✅ Sí       | ⚠️ Moderado    |

**Recomendación**:

- Usa **Método AC** para trinomios con coeficientes grandes o cuando quieras un proceso sistemático
- Usa **Ensayo y Error** para trinomios con $a$ pequeño ($a = 2, 3$) y cuando tengas práctica

## Estrategia híbrida (para expertos)

### Atajo visual

Para $ax^2 + bx + c$:

1. **Verificar MCD**: ¿Hay factor común? Extráelo primero
2. **Verificar TCP**: ¿Es trinomio cuadrado perfecto? Factoriza instantáneamente
3. **Si $a$ es pequeño** ($a = 2, 3$): Ensayo y error
4. **Si $a$ es grande**: Método AC

## Aplicación: Resolver ecuaciones cuadráticas

**Problema**: Resolver $3x^2 + 10x - 8 = 0$

**Solución por factorización**:

```
Factorizar usando método AC:
  A·C = 3 × (-8) = -24
  Buscar: m·n = -24, m + n = 10
  -2 × 12 = -24; -2 + 12 = 10 ✓

  3x² + 10x - 8 = 3x² - 2x + 12x - 8
                = x(3x - 2) + 4(3x - 2)
                = (3x - 2)(x + 4)

Resolver:
  (3x - 2)(x + 4) = 0

  3x - 2 = 0  ó  x + 4 = 0
  x = 2/3     ó  x = -4

Solución: x = {2/3, -4}
```

## Resumen ejecutivo

1. **Forma general**: $ax^2 + bx + c$ con $a \neq 1$
2. **Dos métodos principales**:
   - **Método AC**: Sistemático, convierte en agrupación
   - **Ensayo y Error**: Rápido para $a$ pequeño
3. **Siempre primero**: Verificar factor común
4. **Método AC**: $m \cdot n = a \cdot c$ y $m + n = b$
5. **Verificación**: Obligatoria para confirmar

## Conexión con el siguiente tema

Ahora dominas todos los trinomios cuadráticos. En el tema 2.3 verás **factorizaciones especiales** como suma/diferencia de cubos y factorización por sustitución, técnicas avanzadas para polinomios de grado mayor 2. [Estrategia 2] 3. [Estrategia 3]

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
