# Operaciones con Números Reales

**Tiempo estimado**: 45 minutos  
**Nivel**: Básico/Nivelación  
**Prerrequisitos**: Aritmética elemental de primaria

<<<<<<< HEAD
**Operaciones con números reales** es un tema fundamental en este curso. Dominar estos conceptos te permitirá avanzar hacia problemas más complejos con confianza.
=======
## ¿Por qué importa este concepto?
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48

Las operaciones con números reales son el "sistema operativo" sobre el cual corre todo el software del álgebra. Un error aquí es fatal: puedes plantear la ecuación diferencial más elegante para modelar un puente, pero si fallas al sumar signos negativos en el paso 3, el puente se cae. Este subtema no es solo un repaso; es una recalibración para eliminar "vicios" aritméticos antes de entrar a la abstracción algebraica.

<<<<<<< HEAD
1. Comprender los conceptos clave de operaciones con números reales.
2. Resolver problemas aplicando las reglas y propiedades estudiadas.
3. Evitar errores comunes mediante la práctica consciente.
=======
## Conexión con conocimientos previos

Asumimos que sabes sumar y restar números naturales. Aquí expandiremos ese conocimiento para incluir todo el espectro de los reales (negativos, fracciones, decimales) y, lo más importante, la jerarquía estricta que los gobierna (PEMDAS).
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48

## Comprensión intuitiva

<<<<<<< HEAD
### Conceptos Fundamentales

- Números naturales, enteros, racionales e irracionales
- Operaciones básicas: suma, resta, multiplicación, división
- Reglas de signos en operaciones
- Orden de operaciones (PEMDAS/BODMAS)
- Propiedades: conmutativa, asociativa, distributiva

### Desarrollo del Tema

Para entender Operaciones con números reales, debemos analizar cada componente...
(Aquí se desarrollaría más teoría específica basada en los conceptos listados)
=======
Imagina las operaciones como movimientos en una línea.

- **Sumar** es moverse a la derecha.
- **Restar** es moverse a la izquierda.
- **Multiplicar** es escalar (estirar o encoger) esos movimientos.
- **Los signos** son simplemente instrucciones de dirección.

Un número negativo como $-5$ no es "menos que un número", es una deuda o un movimiento en dirección opuesta. Operar con ellos es simplemente gestionar esas direcciones y magnitudes acumuladas.

### Ejemplo motivador

Tienes $\$100$ en tu cuenta. Emites un cheque por $\$150$ (sobringiro de $\$50$, o $-50$). El banco te cobra una multa de $\$20$ ($-20$). Luego depositas la mitad de tu sueldo de $\$500$ ($+250$). ¿Cuál es tu saldo final?
$$ -50 + (-20) + 250 = 180 $$
El álgebra formaliza este sentido común.

## Definición formal
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48

El conjunto de los números reales $\mathbb{R}$ es un cuerpo ordenado completo. Esto significa que para todo $a, b, c \in \mathbb{R}$, se cumplen axiomas de operaciones internas ($+$ y $\cdot$).

<<<<<<< HEAD
### Ejemplo 1

**Problema**: (-8) + 12 ÷ (-3) × 2

**Solución**:

```
Paso 1. 12 ÷ (-3) = -4
Paso 2: (-4) × 2 = -8
Paso 3: (-8) + (-8) = -16

Respuesta: -16
```

### Ejemplo 2

**Problema**: 3 + 2 × (8 - 3)² ÷ 5

**Solución**:

```
Paso 1. (8-3) = 5
Paso 2: 5² = 25
Paso 3: 2×25 = 50
Paso 4: 50÷5 = 10
Paso 5: 3+10 = 13

Respuesta: 13
```

### Ejemplo 3

**Problema**: 1/2 + 3/4 × 2/3

**Solución**:

```
Paso 1. 3/4 × 2/3 = 6/12 = 1/2
Paso 2: 1/2 + 1/2 = 1

Respuesta: 1
```
=======
### Jerarquía de Operaciones (PEMDAS/BODMAS)

El orden no es negociable en matemáticas. Se resuelve estrictamente en esta secuencia:

1. **P**aréntesis y signos de agrupación $\{ [ ( ) ] \}$. De adentro hacia afuera.
2. **E**xponentes y raíces.
3. **M**ultiplicación y **D**ivisión (tienen la misma jerarquía, se resuelven de **izquierda a derecha**).
4. **A**dición y **S**ustracción (misma jerarquía, de **izquierda a derecha**).
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48

## Implementación práctica: Algoritmos de Resolución

<<<<<<< HEAD
❌ **Error 1**: Ignorar orden de operaciones: 3 + 2 × 5 = 25
✅ **Correcto**: Multiplicar primero: 3 + 10 = 13

❌ **Error 2**: Confundir signos: (-3) × (-4) = -12
✅ **Correcto**: Signos iguales dan positivo: (-3) × (-4) = 12
=======
### 1. Operaciones con Enteros (Regla de Signos)

**Suma/Resta**:
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48

- Signos iguales $\to$ Se suman y se mantiene el signo. ($ -3 - 5 = -8 $)
- Signos diferentes $\to$ Se restan y gana el signo del mayor valor absoluto. ($ -10 + 3 = -7 $)

<<<<<<< HEAD
1. **Analizar el problema**: Identifica qué se pide y qué datos tienes.
2. **Identificar patrones**: Busca estructuras conocidas.
3. **Verificar paso a paso**: Revisa cada operación intermedia.
=======
**Multiplicación/División**:
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48

- Signos iguales $\to$ Positivo ($ + \cdot + = + $, $ - \cdot - = + $)
- Signos opuestos $\to$ Negativo ($ + \cdot - = - $)

<<<<<<< HEAD
- Resolución de problemas de física y geometría.
- Modelado de situaciones cotidianas.
=======
### 2. Operaciones con Fracciones
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48

**Suma/Resta**: Requieren **Mínimo Común Múltiplo (MCM)** en denominadores.
$$ \frac{a}{b} + \frac{c}{d} = \frac{ad + bc}{bd} $$

<<<<<<< HEAD
- Hemos revisado: Números naturales, enteros, racionales e irracionales, Operaciones básicas: suma, resta, multiplicación, división, Reglas de signos en operaciones.
- Recuerda practicar los ejemplos resueltos.
=======
**Multiplicación**: Directa.
$$ \frac{a}{b} \cdot \frac{c}{d} = \frac{a \cdot c}{b \cdot d} $$

**División**: Multiplicación cruzada o "sándwich".
$$ \frac{a}{b} \div \frac{c}{d} = \frac{a}{b} \cdot \frac{d}{c} = \frac{ad}{bc} $$

## Análisis de Casos Resueltos

### Caso 1: Jerarquía Compleja

**Problema**: $ 5 - 3[ 2 - (4 - 7) ] + 12 \div (-3) $

**Resolución paso a paso**:

1. Paréntesis más interno: $(4 - 7) = -3$.
   $$ 5 - 3[ 2 - (-3) ] + 12 \div (-3) $$
2. Simplificar corchete: $2 - (-3) = 2+3 = 5$.
   $$ 5 - 3[ 5 ] + 12 \div (-3) $$
3. Multiplicaciones y Divisiones (izq a der):
   - $3[5] = 15$
   - $12 \div (-3) = -4$
   $$ 5 - 15 + (-4) $$
4. Sumas y Restas:
   $$ 5 - 15 - 4 = -10 - 4 = -14 $$

**Resultado**: $-14$

### Caso 2: Fracciones Compuestas

**Problema**: $ \frac{ \frac{1}{2} + \frac{1}{3} }{ \frac{1}{4} - \frac{1}{5} } $

**Resolución**:

1. Operar numerador: MCM(2,3) = 6.
   $$ \frac{1}{2} + \frac{1}{3} = \frac{3+2}{6} = \frac{5}{6} $$
2. Operar denominador: MCM(4,5) = 20.
   $$ \frac{1}{4} - \frac{1}{5} = \frac{5-4}{20} = \frac{1}{20} $$
3. División de fracciones (extremos por extremos, medios por medios):
   $$ \frac{ \frac{5}{6} }{ \frac{1}{20} } = \frac{ 5 \cdot 20 }{ 6 \cdot 1 } = \frac{100}{6} $$
4. Simplificar:
   $$ \frac{50}{3} $$

## Trampas y errores comunes

### ❌ Error 1: "Multiplicar" signos en sumas

**Incorrecto**: $ -5 - 3 = +8 $ (Porque "menos por menos es más").
**Correcto**: $ -5 - 3 = -8 $.
**Por qué**: La regla "menos por menos da más" **solo** aplica en multiplicación y división. En suma/resta, si debes 5 y gastas 3, debes 8.

### ❌ Error 2: Jerarquía de multiplicación vs suma

**Incorrecto**: $ 4 + 2 \cdot 3 = 18 $ (Sumaron 4+2 primero).
**Correcto**: $ 4 + 6 = 10 $.
**Por qué**: La multiplicación tiene mayor "peso" jerárquico que la suma.

### ❌ Error 3: Cancelación ilegal en fracciones

**Incorrecto**: $ \frac{2 + x}{2} = 1 + x $ (Cancelan el 2).
**Correcto**: $ \frac{2 + x}{2} = \frac{2}{2} + \frac{x}{2} = 1 + \frac{x}{2} $.
**Por qué**: El denominador divide a **todo** el numerador, no solo a una parte.

## Aplicaciones Reales

### Ingeniería Civil

Calcular cargas estructurales requiere sumar vectores de fuerza (positivos y negativos) con precisión absoluta. Un error de signo significa una fuerza calculada hacia arriba cuando en realidad va hacia abajo, lo que puede derrumbar una viga.

### Programación

En cualquier lenguaje (Python, JS, C++), la expresión `result = a + b * c` se evaluará siguiendo PEMDAS. Si el programador no lo entiende, el software tendrá *bugs* lógicos difíciles de rastrear.

## Resumen Ejecutivo

- **Jerarquía (PEMDAS)** es la ley suprema: Agrupación > Exponentes > Mult/Div > Suma/Resta.
- **Signos**: En suma, signos iguales se suman. En multiplicación, signos iguales dan positivo.
- **Fracciones**: Nunca sumes denominadores. Usa MCM.
- **Verificación**: Realiza cálculos inversos para comprobar (si restaste, suma el resultado para volver al original).
>>>>>>> 1beb0ab266191ed7f8a2fe9b8315ea8588747f48
