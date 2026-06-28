# Suma y Diferencia de Cubos

<<<<<<< HEAD
## Introducción
**Suma y diferencia de cubos** es un pilar fundamental en este módulo. Entender esto te permitirá conectar conceptos previos con nuevas herramientas algebraicas.

## Objetivos de Aprendizaje
1. Dominar el concepto de Suma y diferencia de cubos.
2. Identificar patrones para resolución rápida.
3. Aplicar estas técnicas en ejercicios multinivel.

## Contenido Teórico
- a³ + b³ = (a+b)(a²-ab+b²)
- a³ - b³ = (a-b)(a²+ab+b²)

### Profundización
(Aquí se detalla la lógica interna de los conceptos presentados, conectando con a³ + b³ = (a+b)(a²-ab+b²)).

## Ejemplos Resueltos
### Ejemplo 1

**Problema**: x³ - 27

**Solución**:
```
Paso 1. Raíz cúbica x y 3
Paso 2: Aplicar fórmula menos

Respuesta: (x-3)(x²+3x+9)
```


## Errores Comunes
❌ **Error**: Saltarse pasos de verificación.
✅ **Correcto**: Comprobar siempre el resultado.

## Estrategias de Resolución
- Identifica la estructura del problema.
- Selecciona el método más eficiente (ej. factorización vs fórmula general).
- Verifica si la solución tiene sentido en el contexto.
=======
**Tiempo estimado**: 50 minutos  
**Nivel**: Avanzado  
**Prerrequisitos**: Productos notables (1.2.3), Factorización de trinomios (2.2)

## ¿Por qué importa este concepto?

La suma y diferencia de cubos son **identidades algebraicas especiales** que aparecen en:

- **Cálculo**: Simplificación de límites y derivadas
- **Teoría de números**: Factorización de números especiales (ej: $1729 = 1^3 + 12^3 = 9^3 + 10^3$)
- **Geometría**: Volúmenes de sólidos compuestos
- **Álgebra avanzada**: Resolución de ecuaciones cúbicas
- **Física**: Ecuaciones de estado de gases ideales

Mientras que la diferencia de cuadrados es ampliamente conocida, la suma/diferencia de cubos es menos intuitiva pero igualmente poderosa.

## Comprensión intuitiva

### Diferencia de cuadrados (repaso)

Ya conoces:
$$a^2 - b^2 = (a - b)(a + b)$$

Esto funciona porque los términos cruzados se cancelan:
$$(a-b)(a+b) = a^2 + ab - ab - b^2 = a^2 - b^2$$

### ¿Y con cubos?

**Diferencia de cubos**:
$$a^3 - b^3 = (a - b)(a^2 + ab + b^2)$$

**Suma de cubos**:
$$a^3 + b^3 = (a + b)(a^2 - ab + b^2)$$

**Nota crítica**: La **suma de cuadrados** $a^2 + b^2$ NO factoriza en números reales, pero la **suma de cubos** SÍ factoriza.

### Visualización geométrica

Imagina dos cubos:
- Cubo grande: lado $a$, volumen $a^3$
- Cubo pequeño: lado $b$, volumen $b^3$

La diferencia de volúmenes $a^3 - b^3$ se puede reorganizar en:
- Un paralelepípedo de base $(a-b)$ y altura relacionada con $a^2 + ab + b^2$

## Definición formal

### Fórmulas fundamentales

#### Diferencia de cubos
$$\boxed{a^3 - b^3 = (a - b)(a^2 + ab + b^2)}$$

#### Suma de cubos
$$\boxed{a^3 + b^3 = (a + b)(a^2 - ab + b^2)}$$

### Estructura de las fórmulas

Ambas fórmulas tienen la estructura:
$$\text{(Binomio)(Trinomio)}$$

Donde:
- **Binomio**: Raíces cúbicas con el mismo signo de la expresión original
- **Trinomio**: Cuadrados de las raíces $\pm$ producto simple

### Tabla de memorización

| Expresión | Binomio | Trinomio | Patrón del trinomio |
|:----------|:--------|:---------|:--------------------|
| $a^3 - b^3$ | $(a - b)$ | $a^2 + ab + b^2$ | **Mismo** signo, **opuesto** al binomio |
| $a^3 + b^3$ | $(a + b)$ | $a^2 - ab + b^2$ | **Opuesto** al binomio |

**Regla nemotécnica**: 
- Binomio: usa el mismo signo de la expresión
- Trinomio: comienza con cuadrados (positivos), el signo del medio es opuesto al binomio

## Algoritmo de factorización

### Método paso a paso

**PASO 1**: Identificar si la expresión es suma o diferencia de cubos
- Verificar que ambos términos son cubos perfectos
- Identificar las bases $a$ y $b$: $\sqrt[3]{\text{término 1}}$ y $\sqrt[3]{\text{término 2}}$

**PASO 2**: Escribir el binomio
- Usa las raíces con el signo de la expresión original

**PASO 3**: Construir el trinomio
- Primer término: $(\text{base}_1)^2$
- Segundo término: $\pm (\text{base}_1)(\text{base}_2)$ [signo opuesto al binomio]
- Tercer término: $(\text{base}_2)^2$

**PASO 4**: Verificar multiplicando

## Ejemplos resueltos

### Ejemplo 1: Diferencia de cubos básica

**Problema**: Factorizar $x^3 - 8$

**Solución**:
```
PASO 1 - Identificar:
  x³ es cubo perfecto: (x)³
  8 es cubo perfecto: 8 = 2³
  
  Tipo: Diferencia de cubos
  a = x, b = 2

PASO 2 - Binomio:
  (a - b) = (x - 2)

PASO 3 - Trinomio:
  a² + ab + b²
  = x² + x·2 + 2²
  = x² + 2x + 4

RESULTADO:
  x³ - 8 = (x - 2)(x² + 2x + 4)

VERIFICACIÓN:
  (x - 2)(x² + 2x + 4)
  = x·x² + x·2x + x·4 - 2·x² - 2·2x - 2·4
  = x³ + 2x² + 4x - 2x² - 4x - 8
  = x³ - 8 ✓
```

### Ejemplo 2: Suma de cubos

**Problema**: Factorizar $27x^3 + 64$

**Solución**:
```
PASO 1 - Identificar:
  27x³ = (3x)³
  64 = 4³
  
  Tipo: Suma de cubos
  a = 3x, b = 4

PASO 2 - Binomio:
  (a + b) = (3x + 4)

PASO 3 - Trinomio:
  a² - ab + b²
  = (3x)² - (3x)(4) + 4²
  = 9x² - 12x + 16

RESULTADO:
  27x³ + 64 = (3x + 4)(9x² - 12x + 16)

VERIFICACIÓN:
  (3x + 4)(9x² - 12x + 16)
  = 3x·9x² - 3x·12x + 3x·16 + 4·9x² - 4·12x + 4·16
  = 27x³ - 36x² + 48x + 36x² - 48x + 64
  = 27x³ + 64 ✓
```

### Ejemplo 3: Con coeficientes complejos

**Problema**: Factorizar $8a^3 - 125b^3$

**Solución**:
```
PASO 1:
  8a³ = (2a)³
  125b³ = (5b)³
  
  Diferencia de cubos
  Raíces: a = 2a, b = 5b

PASO 2: Binomio
  (2a - 5b)

PASO 3: Trinomio
  (2a)² + (2a)(5b) + (5b)²
  = 4a² + 10ab + 25b²

RESULTADO:
  8a³ - 125b³ = (2a - 5b)(4a² + 10ab + 25b²)
```

### Ejemplo 4: Con factor común previo

**Problema**: Factorizar $3x^3 - 24$

**Solución**:
```
PASO 1 - Extraer factor común:
  3x³ - 24 = 3(x³ - 8)

PASO 2 - Factorizar diferencia de cubos:
  x³ - 8 = x³ - 2³
        = (x - 2)(x² + 2x + 4)

RESULTADO FINAL:
  3x³ - 24 = 3(x - 2)(x² + 2x + 4)
```

### Ejemplo 5: Variable en el exponente

**Problema**: Factorizar $x^6 - y^6$

**Solución**:
```
OBSERVACIÓN: x⁶ es tanto cuadrado como cubo
  x⁶ = (x³)² = (x²)³

PUEDES FACTORIZAR DE DOS FORMAS:

OPCIÓN 1 - Diferencia de cuadrados:
  x⁶ - y⁶ = (x³)² - (y³)²
         = (x³ - y³)(x³ + y³)
  
  Ahora cada factor es suma/diferencia de cubos:
  = (x - y)(x² + xy + y²)(x + y)(x² - xy + y²)

OPCIÓN 2 - Diferencia de cubos:
  x⁶ - y⁶ = (x²)³ - (y²)³
         = (x² - y²)(x⁴ + x²y² + y⁴)
  
  El primer factor es diferencia de cuadrados:
  = (x - y)(x + y)(x⁴ + x²y² + y⁴)

Ambas son válidas, la Opción 1 está más factorizada.
```

## Errores comunes

❌ **Error 1**: Confundir signos en el trinomio  
**Problema**: $x^3 + 8$  
**Incorrecto**: $(x + 2)(x^2 + 2x + 4)$ ❌  
✅ **Correcto**: $(x + 2)(x^2 - 2x + 4)$ [signo medio opuesto al binomio]

❌ **Error 2**: Intentar factorizar suma de cuadrados como suma de cubos  
**Incorrecto**: $x^2 + 4 = (x + 2)(x^2 - 2x + 4)$ ❌  
✅ **Correcto**: $x^2 + 4$ NO factoriza en números reales (es primo)

❌ **Error 3**: Olvidar elevar al cuadrado los coeficientes  
**Problema**: $8x^3 - 27$  
**Incorrecto**: $(2x - 3)(2x^2 + 6x + 3^2)$ ❌  
✅ **Correcto**: $(2x - 3)(4x^2 + 6x + 9)$ [usar $(2x)^2 = 4x^2$]

❌ **Error 4**: Confundir con trinomio cuadrado perfecto  
El trinomio en suma/diferencia de cubos **NO es trinomio cuadrado perfecto** y generalmente no factoriza más.

## Casos especiales y extensiones

### Caso 1: Números especiales

**1729** (número de Ramanujan):
$$1729 = 1^3 + 12^3 = 9^3 + 10^3$$

Esto muestra que algunos números se pueden expresar como suma de cubos de múltiples formas.

### Caso 2: Factorización completa

El trinomio resultante **generalmente no factoriza** más en números reales, pero puede tener raíces complejas.

Ejemplo: $(x + 2)(x^2 - 2x + 4)$  
El trinomio $x^2 - 2x + 4$ tiene discriminante negativo: $\Delta = 4 - 16 = -12 < 0$

### Caso 3: Potencias mayores

Para $a^n - b^n$ con $n$ impar:
$$a^n - b^n = (a - b)(a^{n-1} + a^{n-2}b + a^{n-3}b^2 + \ldots + ab^{n-2} + b^{n-1})$$

Para $n=3$: recuperamos la fórmula de diferencia de cubos.

## Aplicación: Resolución de ecuaciones

**Problema**: Resolver $x^3 = 64$

**Solución tradicional**:
$$x^3 = 64 \Rightarrow x = \sqrt[3]{64} = 4$$

**Solución por factorización**:
```
x³ = 64
x³ - 64 = 0
(x - 4)(x² + 4x + 16) = 0

De aquí:
x - 4 = 0  ⟹  x = 4  (solución real)

x² + 4x + 16 = 0  (discriminante negativo, raíces complejas)
```

## Comparación con diferencia de cuadrados

| Aspecto | Diferencia de cuadrados | Diferencia/Suma de cubos |
|:--------|:------------------------|:-------------------------|
| **Fórmula** | $a^2 - b^2 = (a-b)(a+b)$ | $a^3 \pm b^3 = (a \pm b)(\text{trinomio})$ |
| **Factores** | 2 binomios | 1 binomio + 1 trinomio |
| **Suma** | NO factoriza | SÍ factoriza |
| **Complejidad** | Simple | Media |
| **Frecuencia** | Muy común | Menos común |

## Estrategia de reconocimiento rápido

### Checklist para identificar cubos perfectos

**Constantes comunes**:
- $1 = 1^3$
- $8 = 2^3$
- $27 = 3^3$
- $64 = 4^3$
- $125 = 5^3$
- $216 = 6^3$
- $1000 = 10^3$

**Variables**:
- $x^3, x^6, x^9, x^{12}, \ldots$ (exponentes múltiplos de 3)
- $a^3b^3 = (ab)^3$

## Resumen ejecutivo

1. **Diferencia de cubos**: $a^3 - b^3 = (a - b)(a^2 + ab + b^2)$
2. **Suma de cubos**: $a^3 + b^3 = (a + b)(a^2 - ab + b^2)$
3. **Estructura**: Binomio × Trinomio (trinomio NO factoriza más generalmente)
4. **Signos**: Binomio igual a la expresión original, trinomio opuesto en el término medio
5. **Verificación**: SIEMPRE multiplicar para confirmar
6. **Diferencia clave**: A diferencia de cuadrados, las sumas de cubos SÍ factorizan

## Conexión con el siguiente tema

Estas fórmulas son casos especiales de factorización. En el siguiente tema (2.3.2) verás **factorización por sustitución**, donde transformas expresiones complejas en formas más simples mediante cambios de variable, incluyendo casos que se reducen a suma/diferencia de cubos.
2. [Estrategia 2]
3. [Estrategia 3]
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48

## Aplicaciones
- Simplificación de expresiones en Física.
- Modelado de funciones de costos/ingresos.
- Base para el Cálculo Diferencial.
