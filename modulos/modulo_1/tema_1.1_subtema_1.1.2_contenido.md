# Multiplicación de Expresiones Algebraicas

**Tiempo estimado**: 60 minutos  
**Nivel**: Básico/Intermedio  
**Prerrequisitos**: Leyes de exponentes, Propiedad distributiva

## ¿Por qué importa este concepto?

La multiplicación es el motor de crecimiento en álgebra. Mientras la suma simplemente acumula cantidades, la multiplicación crea nuevas dimensiones. Multiplicar metros por metros crea metros cuadrados (área). Multiplicar $x$ por $x$ crea $x^2$ (no linealidad). Es la operación base para calcular áreas, volúmenes, potencias y fuerzas. Sin ella, estamos atrapados en un mundo lineal y plano.

## Comprensión intuitiva

Multiplicar en álgebra tiene dos pasos independientes que ocurren simultáneamente:

1. **Los números** (coeficientes) se multiplican normalmente.
2. **Las letras** (variables) sigue la regla de acumulación de potencias.

Si $x$ es "ancho" y multiplicas por $x$ ("largo"), obtienes $x^2$ ("área").
Si tienes $2$ rectángulos de área $3x^2$, tienes en total $6x^2$.

## Leyes Fundamentales

### 1. Producto de Potencias de Igual Base

$$ a^m \cdot a^n = a^{m+n} $$
Si multiplicas bases iguales, **SUMAS** los exponentes.

- $x^2 \cdot x^3 = x^{2+3} = x^5$
- $y \cdot y^4 = y^{1+4} = y^5$ (Recuerda: $y = y^1$)

### 2. Propiedad Distributiva Extendida

$$ a(b + c + d) = ab + ac + ad $$
El factor externo "saluda" a todos y cada uno de los términos internos.

### 3. Regla de Signos

Igual que en aritmética:

- $(+)(+) = +$
- $(-)(-) = +$
- $(+)(-) = -$

## Implementación práctica: Algoritmos

### Caso 1: Monomio por Monomio

**Algoritmo**: (Signo) $\times$ (Coeficiente) $\times$ (Variable A) $\times$ (Variable B)...
**Ejemplo**: $ (-3x^2y) \cdot (4xy^3) $

1. Signos: $(-)(+) = -$
2. Coeficientes: $3 \cdot 4 = 12$
3. Variable $x$: $x^2 \cdot x^1 = x^3$
4. Variable $y$: $y^1 \cdot y^3 = y^4$
**Resultado**: $ -12x^3y^4 $

### Caso 2: Monomio por Polinomio

**Algoritmo**: Aplicar distributiva.
**Ejemplo**: $ 2a^2(3a - 5b + 1) $

1. $ 2a^2 \cdot 3a = 6a^3 $
2. $ 2a^2 \cdot (-5b) = -10a^2b $
3. $ 2a^2 \cdot 1 = 2a^2 $
**Resultado**: $ 6a^3 - 10a^2b + 2a^2 $

### Caso 3: Polinomio por Polinomio (El método "Todos contra Todos")

Cada término del primer polinomio multiplica a cada término del segundo.
**Ejemplo**: $ (x + 2)(x - 5) $

1. $x$ multiplica a $(x - 5) \to x^2 - 5x$
2. $2$ multiplica a $(x - 5) \to 2x - 10$
3. Sumar todo: $ x^2 \underbrace{- 5x + 2x}_{\text{semejantes}} - 10 $
**Resultado**: $ x^2 - 3x - 10 $

## Análisis de Casos Complejos

### Multiplicación con exponentes literales

**Problema**: $ (x^{n+1}) \cdot (x^{2n-3}) $
**Resolución**:
Aplicar regla de suma de exponentes:
$$ (n + 1) + (2n - 3) $$
Sumar términos semejantes en el exponente:
$$ n + 2n = 3n $$
$$ 1 - 3 = -2 $$
**Resultado**: $ x^{3n-2} $

### Producto continuado

**Problema**: $ 2x(x-1)(x+3) $
No intentes multiplicar los tres a la vez. Hazlo por etapas.

1. Primero los paréntesis: $(x-1)(x+3) = x^2 + 3x - 1x - 3 = x^2 + 2x - 3$
2. Luego el factor externo: $2x(x^2 + 2x - 3)$
3. Distribuir: $ 2x^3 + 4x^2 - 6x $

## Trampas y errores comunes

### ❌ Error 1: Distribuir potencia

**Incorrecto**: $(xy)^2 = xy^2$
**Correcto**: $(xy)^2 = x^2y^2$
**Por qué**: El exponente afecta a TODO lo que está en el paréntesis.

### ❌ Error 2: Olvidar el término central

**Incorrecto**: $(x+3)(x-3)$ a veces lo confunden y suman cruzado mal.
(Este es un producto notable, pero si lo haces manual, cuidado con los signos).
**Correcto**: $x^2 - 3x + 3x - 9 = x^2 - 9$.

### ❌ Error 3: Sumar en lugar de multiplicar exponentes

**Incorrecto**: $x^2 \cdot x^3 = x^6$
**Correcto**: $x^5$
**Por qué**: $x^2$ es $xx$. $x^3$ es $xxx$. En total hay 5 equis multiplicándose.

## Visualización Geometría

Multiplicar binomios $(x+2)(x+3)$ es equivalente a calcular el área de un rectángulo de base $x+3$ y altura $x+2$.
El área total se compone de 4 piezas:

1. Un cuadrado grande $x^2$
2. Un rectángulo $3x$
3. Un rectángulo $2x$
4. Un cuadrado pequeño $6$
Total: $x^2 + 5x + 6$.

## Resumen Ejecutivo

1. **Coeficientes se multiplican** ($2 \cdot 3 = 6$).
2. **Exponentes se suman** ($x^2 \cdot x^3 = x^5$).
3. **Orden**: Signo $\to$ Número $\to$ Letras (en orden alfabético).
4. **Polinomios**: Todos contra todos. Si tienes un binomio (2 términos) por un trinomio (3 términos), debes obtener $2 \times 3 = 6$ términos antes de simplificar.
