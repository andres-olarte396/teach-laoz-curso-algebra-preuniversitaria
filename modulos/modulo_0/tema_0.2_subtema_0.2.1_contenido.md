# Variables y Constantes en el Lenguaje Algebraico

**Tiempo estimado**: 40 minutos  
**Nivel**: Introductorio  
**Prerrequisitos**: Ninguno

## ¿Por qué importa este concepto?

El álgebra nace cuando dejamos de calcular con números específicos ($3+5$) y empezamos a calcular con **patrones generales**. Las variables son contenedores vacíos que pueden guardar cualquier número. Las constantes son los anclajes fijos de nuestro universo. Saber distinguirlos es entender la diferencia entre lo que *cambia* y lo que *permanece* en un sistema matemático. Sin variables, no hay fórmulas, no hay código de programación, no hay física moderna.

## Comprensión intuitiva

Piensa en una **fórmula de Excel** o una **receta de cocina**.

- **Variable**: "Cantidad de harina". Depende de cuántas pizzas quieras hacer. Si haces 1 pizza, es 200g. Si haces 10, son 2000g. El valor *varía*. Generalmente usamos letras como $x, y, z$ o $n$.
- **Constante**: "Minutos en el horno". La receta dice 20 minutos fijos, sin importar cuántas pizzas hagas. El valor es *constante*. Usamos números ($5, -3, \pi$) o primeras letras del alfabeto ($a, b, c$) para constantes genéricas.

El álgebra es el lenguaje para escribir estas "recetas" de forma compacta.

## Definición formal

### 1. Variable (Incógnita o Indeterminada)

Símbolo que representa un elemento no especificado de un conjunto dado.

- En $f(x) = 2x + 1$, **$x$** es la variable independiente (input).
- En $x + 3 = 7$, **$x$** es una incógnita (un valor específico a descubrir).

### 2. Constante

Símbolo que representa un valor fijo y determinado.

- **Absoluta**: Números como $2, -7, \frac{1}{2}, \pi, e$.
- **Paramétrica**: Letras como $a, b, c$ en $ax^2 + bx + c$. Representan números fijos en un contexto dado, aunque no sepamos cuáles son.

### 3. Término Algebraico

Es la estructura básica del lenguaje algebraico. Se compone de cuatro partes:
$$ -5x^3 $$

- **Signo**: ($-$) Indica si es positivo o negativo.
- **Coeficiente**: ($5$) El factor numérico que multiplica a la variable. Indica "cuántas veces" tenemos la variable.
- **Variable**: ($x$) La base literal.
- **Exponente**: ($3$) El grado de la variable.

## Implementación práctica: Traducción Lenguaje Natural $\leftrightarrow$ Agebraico

La habilidad crítica aquí es **traducir**.

| Lenguaje Natural | Lenguaje Algebraico | Análisis |
| :--- | :--- | :--- |
| "Un número cualquiera" | $x$ | Variable genérica. |
| "El doble de un número" | $2x$ | Coeficiente 2 multiplica variable. |
| "Un número aumentado en 5" | $x + 5$ | Suma de variable y constante. |
| "El cuadrado del siguiente número" | $(x+1)^2$ | Operación compuesta. |
| "La suma de dos números distintos" | $x + y$ | Dos variables diferentes. |
| "El 20% de un número" | $0.20x$ | Porcentaje como decimal. |

### Ejemplo de Modelado

**Situación**: Un plan de celular cuesta \$20 de base mensual más \$0.50 por cada minuto de llamada.

- **Constante**: \$20 (Costo fijo).
- **Variable**: $m$ (Minutos consumidos, esto cambia cada mes).
- **Coeficiente**: \$0.50 (Costo por unidad de variable).
- **Expresión Final**: $Costo = 20 + 0.50m$.

## Trampas y errores comunes

### ❌ Error 1: Confundir coeficiente con sumando

**Incorrecto**: "Un número más dos" $\to 2x$.
**Correcto**: $x + 2$.
**Explicación**: $2x$ es "dos veces un número" (multiplicación). $x+2$ es suma.

### ❌ Error 2: Variables distintas vs misma variable

**Incorrecto**: "La suma de dos números" $\to x + x$.
**Correcto**: $x + y$.
**Explicación**: Si usas $x$ dos veces, obligas a que los números sean iguales. Si el problema dice "dos números" (en general), debes usar letras distintas.

### ❌ Error 3: Signo del coeficiente

En el término $-x$:

- Muchos piensan que no tiene coeficiente.
- **Correcto**: El coeficiente es $-1$.
- **Explicación**: $-x$ es abreviatura de $-1 \cdot x$.

## Resumen Ejecutivo

- **Variable ($x, y, z$)**: Contenedor de valores cambiantes o desconocidos.
- **Constante ($5, \pi, -2$)**: Valor fijo.
- **Coeficiente**: Número que multiplica a la variable. (En $3x$, el 3).
- **Traducción**: El álgebra es un idioma. Debes aprender a traducir frases a símbolos.
  - "De", "del", "veces" $\to$ Multiplicación.
  - "Aumentado", "más", "suma" $\to$ Suma.
  - "Disminuido", "diferencia" $\to$ Resta.
  - "Razón", "cociente" $\to$ División.
