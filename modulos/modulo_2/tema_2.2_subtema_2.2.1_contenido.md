# Trinomio Cuadrado Perfecto

**Tiempo estimado**: 45 minutos  
**Nivel**: Intermedio  
**Prerrequisitos**: Productos notables (1.2.1), Factor común (2.1.1)

## ¿Por qué importa este concepto?

El trinomio cuadrado perfecto (TCP) es la "huella dactilar" algebraica del producto notable $(a \pm b)^2$. Reconocerlo te permite factorizar instantáneamente sin tanteo, lo cual es crítico para:

- **Completar el cuadrado** (método para resolver ecuaciones cuadráticas)
- **Optimización en cálculo** (encontrar máximos y mínimos)
- **Geometría analítica** (ecuaciones de círculos y parábolas)
- **Procesamiento de señales** (análisis de Fourier)

Dominar el TCP reduce problemas complejos a formas binomiales simples.

## Comprensión intuitiva

### La Regla del "Sandwich Perfecto"

Un trinomio cuadrado perfecto tiene esta estructura:

$$\boxed{\text{Cuadrado}} + \boxed{\text{Doble Producto}} + \boxed{\text{Cuadrado}}$$

**Analogía geométrica**: $(a + b)^2$ representa el área de un cuadrado de lado $(a + b)$:

```
  ┌─────┬─────┐
  │  a² │ ab  │ a
  ├─────┼─────┤
  │ ab  │ b²  │ b
  └─────┴─────┘
    a     b

Área total = a² + 2ab + b²
```

El término central $2ab$ es exactamente el **doble** del producto de las bases de los cuadrados.

## Definición formal

### Trinomio Cuadrado Perfecto (TCP)

Un trinomio $T$ es TCP si cumple:

$$T = A^2 \pm 2AB + B^2$$

donde $A$ y $B$ son expresiones algebraicas, y factoriza como:

$$T = (A \pm B)^2$$

### Criterio de identificación

Un trinomio $ax^2 + bx + c$ es TCP si:

1. **El primer y tercer término son cuadrados perfectos**: $a$ y $c$ son cuadrados de números o expresiones
2. **El segundo término es el doble producto**: $b = \pm 2\sqrt{a} \cdot \sqrt{c}$

### Tabla de reconocimiento rápido

| Trinomio         | ¿Es TCP? | Factorización                                                              |
| :--------------- | :------- | :------------------------------------------------------------------------- |
| $x^2 + 6x + 9$   | ✅ SÍ    | $(x + 3)^2$ porque $9 = 3^2$ y $6x = 2 \cdot x \cdot 3$                    |
| $x^2 + 10x + 25$ | ✅ SÍ    | $(x + 5)^2$                                                                |
| $4x^2 - 12x + 9$ | ✅ SÍ    | $(2x - 3)^2$ porque $4x^2 = (2x)^2$, $9 = 3^2$, $12x = 2 \cdot 2x \cdot 3$ |
| $x^2 + 5x + 9$   | ❌ NO    | $2\sqrt{1}\sqrt{9} = 6 \neq 5$                                             |
| $x^2 + 8x + 16$  | ✅ SÍ    | $(x + 4)^2$                                                                |

## Algoritmo de identificación y factorización

### Método de las tres preguntas

**PREGUNTA 1**: ¿El primer término es un cuadrado perfecto?  
→ Calcula $A = \sqrt{\text{primer término}}$

**PREGUNTA 2**: ¿El tercer término es un cuadrado perfecto?  
→ Calcula $B = \sqrt{\text{tercer término}}$

**PREGUNTA 3**: ¿El segundo término es $\pm 2AB$?  
→ Verifica si $\text{término medio} = \pm 2 \cdot A \cdot B$

Si las tres respuestas son **SÍ** → TCP confirmado

Factorización: $(A \pm B)^2$ (usa el signo del término medio)

## Ejemplos resueltos

### Ejemplo 1: TCP básico con signo positivo

**Problema**: Factorizar $x^2 + 10x + 25$

**Solución**:

```
PREGUNTA 1: ¿x² es cuadrado perfecto?
  √(x²) = x ✓
  A = x

PREGUNTA 2: ¿25 es cuadrado perfecto?
  √25 = 5 ✓
  B = 5

PREGUNTA 3: ¿10x = 2·x·5?
  2·x·5 = 10x ✓
  Signo: + (positivo)

CONCLUSIÓN: Es TCP
Factorización: (x + 5)²

VERIFICACIÓN:
  (x + 5)² = x² + 2·x·5 + 5²
           = x² + 10x + 25 ✓
```

### Ejemplo 2: TCP con signo negativo

**Problema**: Factorizar $9a^2 - 30a + 25$

**Solución**:

```
PREGUNTA 1: ¿9a² es cuadrado perfecto?
  √(9a²) = 3a ✓
  A = 3a

PREGUNTA 2: ¿25 es cuadrado perfecto?
  √25 = 5 ✓
  B = 5

PREGUNTA 3: ¿-30a = -2·3a·5?
  -2·3a·5 = -30a ✓
  Signo: - (negativo)

CONCLUSIÓN: Es TCP
Factorización: (3a - 5)²

VERIFICACIÓN:
  (3a - 5)² = (3a)² - 2·3a·5 + 5²
            = 9a² - 30a + 25 ✓
```

### Ejemplo 3: TCP con coeficientes fraccionarios

**Problema**: Factorizar $\displaystyle x^2 + x + \frac{1}{4}$

**Solución**:

```
PREGUNTA 1: A = √(x²) = x ✓

PREGUNTA 2: B = √(1/4) = 1/2 ✓

PREGUNTA 3: ¿x = 2·x·(1/2)?
  2·x·(1/2) = x ✓

CONCLUSIÓN: Es TCP
Factorización: (x + 1/2)²

FORMA EQUIVALENTE:
  (x + 1/2)² = (2x + 1)²/4
```

### Ejemplo 4: Caso con variables múltiples

**Problema**: Factorizar $4x^2 + 12xy + 9y^2$

**Solución**:

```
PREGUNTA 1: √(4x²) = 2x ✓
  A = 2x

PREGUNTA 2: √(9y²) = 3y ✓
  B = 3y

PREGUNTA 3: ¿12xy = 2·2x·3y?
  2·2x·3y = 12xy ✓

CONCLUSIÓN: Es TCP
Factorización: (2x + 3y)²
```

## Errores comunes

❌ **Error 1**: Confundir TCP con trinomio genérico  
**Problema**: $x^2 + 7x + 12$  
**Incorrecto**: $(x + ?)^2$ [No es TCP porque $2\sqrt{1}\sqrt{12} = 2\sqrt{12} \approx 6.9 \neq 7$]  
✅ **Correcto**: No es TCP, usar método de tanteo → $(x + 3)(x + 4)$

❌ **Error 2**: Olvidar el exponente 2 en la factorización  
**Incorrecto**: $x^2 + 6x + 9 = (x + 3)$ ❌  
✅ **Correcto**: $x^2 + 6x + 9 = (x + 3)^2$

❌ **Error 3**: Equivocar el signo del término medio  
**Problema**: $x^2 - 8x + 16$  
**Incorrecto**: $(x + 4)^2 = x^2 + 8x + 16$ ❌ (signo incorrecto)  
✅ **Correcto**: $(x - 4)^2 = x^2 - 8x + 16$ ✓

❌ **Error 4**: No simplificar raíces de coeficientes  
**Problema**: $16x^2 + 24x + 9$  
**Incorrecto**: $(16x + 9)^2$ ❌  
✅ **Correcto**: $A = \sqrt{16x^2} = 4x$, $B = \sqrt{9} = 3$ → $(4x + 3)^2$

## Estrategias avanzadas

### Estrategia 1: Completar el cuadrado

Si un trinomio NO es TCP pero se le puede agregar/quitar un término para hacerlo TCP:

**Ejemplo**: $x^2 + 6x + 5$

```
Para que sea TCP, necesito que el término independiente sea (6/2)² = 9

x² + 6x + 5 = x² + 6x + 9 - 9 + 5
            = (x² + 6x + 9) - 4
            = (x + 3)² - 4
            = (x + 3)² - 2²
            = [(x + 3) - 2][(x + 3) + 2]  [diferencia de cuadrados]
            = (x + 1)(x + 5)
```

### Estrategia 2: TCP oculto con factor común previo

**Ejemplo**: $2x^2 + 8x + 8$

```
PASO 1 - Extraer factor común:
  2x² + 8x + 8 = 2(x² + 4x + 4)

PASO 2 - Factorizar TCP interno:
  x² + 4x + 4 es TCP: (x + 2)²

RESULTADO:
  2x² + 8x + 8 = 2(x + 2)²
```

### Estrategia 3: Verificación rápida mental

Para $ax^2 + bx + c$, calcula mentalmente:

$$\left(\frac{b}{2\sqrt{a}}\right)^2 \stackrel{?}{=} \frac{c}{1}$$

Si es igual → TCP

**Ejemplo**: $9x^2 + 12x + 4$
$$\left(\frac{12}{2\sqrt{9}}\right)^2 = \left(\frac{12}{6}\right)^2 = 2^2 = 4 \checkmark$$

Factorización: $(\sqrt{9}x + \sqrt{4})^2 = (3x + 2)^2$

## Aplicación: Resolución de ecuaciones

**Problema**: Resolver $x^2 - 10x + 25 = 0$

**Solución reconociendo TCP**:

```
x² - 10x + 25 = 0
(x - 5)² = 0
x - 5 = 0
x = 5

Solución única: x = 5 (raíz doble)
```

**Sin reconocer TCP** (más trabajo):

```
Fórmula cuadrática:
x = (10 ± √(100 - 100))/2 = (10 ± 0)/2 = 5
```

## Resumen ejecutivo

1. **TCP** = Trinomio de la forma $A^2 \pm 2AB + B^2 = (A \pm B)^2$
2. **Criterio**: Extremos son cuadrados perfectos Y término medio = $\pm 2\sqrt{\text{extremos}}$
3. **Algoritmo**: Extraer raíces de extremos → Verificar doble producto → Factorizar
4. **Ventaja**: Factorización instantánea sin tanteo
5. **Signo**: El signo del término medio se conserva en $(A \pm B)^2$
6. **Aplicación**: Fundamental para completar el cuadrado y resolver ecuaciones

## Conexión con el siguiente tema

El TCP es un caso especial. En el siguiente tema (2.2.2) verás trinomios de la forma $x^2 + bx + c$ que NO son TCP, requiriendo el método de **tanteo o descomposición**.
