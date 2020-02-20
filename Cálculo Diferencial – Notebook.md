---
pinned: true
tags: [Notebook, School]
title: Cálculo Diferencial – Notebook
created: '2020-02-16T06:42:49.001Z'
modified: '2020-02-20T17:22:42.795Z'
---

# Cálculo Diferencial – Notebook

Libreta para la materia de *Cálculo Diferencial*.

# Índice <a name="index">

1. [Unidad 1](#U1)
   1. [Números reales](#U1T1)
      1. [Distintos tipos de números](#U1T1S1)
      2. [Los números reales](#U1T1S2)
      3. [Axiomas y propiedades de los números reales](#U1T1S3)
      4. [Axiomas de los números reales](#U1T1S4)
      5. [Propiedades de los exponentes](#U1T1S5)
      6. [Errores comunes](#U1T1S6)
      7. [Intervalos](#U1T1S7)
      8. [Tipos de intervalos](#U1T1S8)
      9. [Unión e intersección de conjuntos](#U1T1S9)
      10. [Resta y complemento de conjuntos](#U1T1S10)
      11. [Inecuaciones (Desigualdades)](#U1T1S11)
      12. [Inecuaciones Lineales](#U1T1S12)
      13. [Inecuaciones Cuadráticas](#U1T1S13)
      14. [Inecuaciones Racionales](#U1T1S14)
      15. [Inecucaciones con valor absoluto](#U1T1S15)
   16. [Funciones](#U1T2)
       1. [Clasificación de las funciones](#U2T1)
       2. [Dominio de funciones](#U2T2)
       3. [Gráficas de funciones](#U2T3)
       4. [Gráficas y ecuaciones](#U2T4)
       5. [Gráficas importantes en cálculo](#U2T5)
       6. [Funciones definidas por partes](#U2T6)
       7. [Simetría](#U2T7)
       8. [Funciones crecientes o decrecientes](#U2T8)
       9. [Traslación de funciones](#U2T9)
       10. [Operaciones con funciones](#U2T10)
       11. [Composición de funciones](#U2T11)
       12. [Funciones Inversas](#U2T12)
       13. [Modelos Matemáticos](#U2T13)
       14. [Modelos Matemáticos Lineales](#U2T14)
       15. [Modelos Matemáticos Exponenciales](#U2T15)
       16. [Modelos Matemáticos Trigonométricos](#U2T16)
2. [Unidad 2](#U2)
3. [Unidad 3](#U3)

# Unidad 1 <a name="U1"></a> <small>[:arrow_heading_up:](#index)</small>

## Númeroes Reales <a name="U1T1"></a> <small>[:arrow_heading_up:](#index)</small>

### Distintos tipos de números <a name="U1T1S1"></a> <small>[:arrow_heading_up:](#index)</small>

Todos estos conjuntos de números pertenecen a los **Reales** $(\Bbb{R})$:  

+ $\Large{\text{Naturales } (\Bbb{N}) \text{: } \{1, 2, 3, 4, 5, ...\}}$
+ $\Large{\text{Enteros } (\Bbb{Z}) \text{: } \{..., -3, -2, -1, 0, 1, 2, 3, ...\}}$
+ $\Large{\text{Racionales } (\Bbb{Q}) \text{: } \{..., {1 \over 3}, -{3 \over 4}, {21 \over 47}, 8, -{9 \over 2}, -3, ...\}}$
+ $\Large{\text{Irracionales } (\Bbb{I}) \text{: } \{\pi, e, \sqrt{2}, -\sqrt{3}, ...\}}$

> $\Bbb{N} \subset \Bbb{Z} \subset \Bbb{Q}$

### Los números reales <a name="U1T1S2"></a> <small>[:arrow_heading_up:](#index)</small>

Debemos de tener cuidado al escribir los números reales.

+ **Expresiones Indefinidas**
   + ${3 \over 0}$
   + $\sqrt{-5}$
   + $0^{0}$
   + $(-1)^{3 / 4}$

+ **Expresiones Correctas**
   + ${0 \over 3}$ es correcto y es igual a $0$.
   + $\sqrt{0}$ es correcto y es igual a $0$.
   + $\sqrt{8}$ es correcto y es igual a $2.8284$.
   + $\sqrt[3]{-7}$ es correcto y es igual a $-1.9129$.

+ **Expresiones Incorrectas**
   + $\sqrt{2 + 3} = \sqrt{2} + \sqrt{3}$
   + $\sqrt{9} = \pm 3$
   + ${2 + \textcolor{red}{\cancel{\textcolor{white}{3}}} \over 5 + \textcolor{red}{\cancel{\textcolor{white}{3}}}} = {2 \over 5}$
   + $-2^{2} = 4$

+ **Expresiones con las que hay que tener cuidado**
   + $-x^{2} \textcolor{red}{\text{ no es lo mismo que }(-x)^{2}}$
   + ${5\textcolor{red}{\cancel{\textcolor{white}{x}}} \over \textcolor{red}{\cancel{\textcolor{white}{x}}}} = 5 \textcolor{red}{\text{ si } x = 0 \text{ la expresión es incorrecta}}$
   + $\sqrt{x^{2}} = 2 \textcolor{red}{\text{ si } x \text{ es negatival a expresión es incorrecta}}$

### Axiomas y propiedades de los números reales <a name="U1T1S3"></a> <small>[:arrow_heading_up:](#index)</small>

Existen propiedades o leyes que cumplen los números reales. 

Para que una propiedad o ley sea válida, requiere demostrarse; aunque también existen algunas *propiedades tan fundamentales que solamente se toman como ciertas*.

> Un **axioma** es una ley que es cierta por sí misma, es decir, no necesita demostración. Por ejemplo: *El axioma de la conmutatividad de la suma*:

$$
3 + 5 = 5 + 3
$$

> Un **teorema o propiedad** es una ley cuya veracidad ya ha sido demostrada. Por ejemplo: *Las leyes de los signos*:

$$
(-)(-) = (+) \\
(-)(+) = (-) \\
(+)(-) = (-) \\
(+)(+) = (+)
$$

```mermaid
graph LR
  Axiomas --> Propieades --> Teoremas
```

### Axiomas de los números reales <a name="U1T1S4"></a> <small>[:arrow_heading_up:](#index)</small>


+ **Para la suma:**
  + *Cerradura*
  Si $a \in \Bbb{R}$ entonces $a + b \in \Bbb{R}$
  + *Asociativa*
  $(a+b)+c = a+(b+c)$
  + *Neutro*
  $a + 0 = a$
  + *Inverso*
  $a - a = 0$
  + *Conmutativa*
  $a + b = b + a$

+ **Para la multiplicación:**
  + *Cerradura*
  Si $a \in \Bbb{R}$ entonces $ab \in \Bbb{R}$
  + *Asociativa*
  $(ab)c = a(bc)$
  + *Neutro*
  $a(1) = a$
  + *Inverso*
  $a({1 \over a}) = 1$
  + *Conmutativa*
  $ab = ba$
 
### Propiedades de los exponentes <a name="U1T1S5"></a> <small>[:arrow_heading_up:](#index)</small>

**Definición:** Si $a \in \Bbb{R}$ y $n \in \Bbb{N}$ entonces:

$$
a^{n} = \underbrace{(a)(a)(a)\dots(a)}_{n \text{ veces}}
$$

+ **Propiedades**
  1. $a^{0} = 1$ <small>, si $a \not = 0$</small>
  2. $a^{-n} = {1 \over a^{n}}$ y también $a^{n} = {1 \over a^{-n}}$
  3. $a^{m}a^{n} = a^{m+n}$
  4. ${a^{m} \over a^{n}} = a^{m-n} = {1 \over a^{n-m}}$
  5. $(a^{m})^{n} = a^{mn}$
  6. $(ab)^{n} = a^{n}b^{n}$
  7. $({a \over b})^{n} = {a^{n} \over b^{n}}$
  8. $({a \over b})^{-n} = ({b \over a})^{n} = {b^{n} \over a^{n}}$
  9. ${a^{-m} \over b^{-n}} = {b^{n} \over a^{m}}$

### Errores comunes <a name="U1T1S6"></a> <small>[:arrow_heading_up:](#index)</small>

### Intervalos <a name="U1T1S7"></a> <small>[:arrow_heading_up:](#index)</small>

### Tipos de intervalos <a name="U1T1S8"></a> <small>[:arrow_heading_up:](#index)</small>

### Unión e intersección de conjuntos <a name="U1T1S9"></a> <small>[:arrow_heading_up:](#index)</small>

### Resta y complemento de conjuntos <a name="U1T1S10"></a> <small>[:arrow_heading_up:](#index)</small>

### Inecuaciones (Desigualdades) <a name="U1T1S11"></a> <small>[:arrow_heading_up:](#index)</small>

### Inecuaciones Lineales <a name="U1T1S12"></a> <small>[:arrow_heading_up:](#index)</small>

### Inecuaciones Cuadráticas <a name="U1T1S13"></a> <small>[:arrow_heading_up:](#index)</small>

### Inecuaciones Racionales <a name="U1T1S14"></a> <small>[:arrow_heading_up:](#index)</small>

### Inecuaciones con valor absoluto <a name="U1T1S15"></a> <small>[:arrow_heading_up:](#index)</small>

## Funciones <a name="U1T2"></a> <small>[:arrow_heading_up:](#index)</small>

### Clasificación de las funciones <a name="U1T2S1"></a> <small>[:arrow_heading_up:](#index)</small>

### Dominio de funciones <a name="U1T2S2"></a> <small>[:arrow_heading_up:](#index)</small>

### Gráficas de funciones <a name="U1T2S3"></a> <small>[:arrow_heading_up:](#index)</small>

### Gráficas y ecuaciones <a name="U1T2S4"></a> <small>[:arrow_heading_up:](#index)</small>

### Gráficas importantes en cálculo <a name="U1T2S5"></a> <small>[:arrow_heading_up:](#index)</small>

### Funciones definidas por partes <a name="U1T2S6"></a> <small>[:arrow_heading_up:](#index)</small>

### Simetría <a name="U1T2S7"></a> <small>[:arrow_heading_up:](#index)</small>

### Funciones crecientes o decrecientes <a name="U1T2S8"></a> <small>[:arrow_heading_up:](#index)</small>

### Traslación de funciones <a name="U1T2S9"></a> <small>[:arrow_heading_up:](#index)</small>

### Operaciones con funciones <a name="U1T2S10"></a> <small>[:arrow_heading_up:](#index)</small>

### Composición de funciones <a name="U1T2S11"></a> <small>[:arrow_heading_up:](#index)</small>

### Funciones inversas <a name="U1T2S12"></a> <small>[:arrow_heading_up:](#index)</small>

### Modelos Matemáticos <a name="U1T2S13"></a> <small>[:arrow_heading_up:](#index)</small>

### Modelos Matemáticos Lineales <a name="U1T2S14"></a> <small>[:arrow_heading_up:](#index)</small>

### Modelos Matemáticos Exponenciales <a name="U1T2S15"></a> <small>[:arrow_heading_up:](#index)</small>

### Modelos Matemáticos Trigonométricos <a name="U1T2S16"></a> <small>[:arrow_heading_up:](#index)</small>

# Unidad 2 <a name="U2"></a> <small>[:arrow_heading_up:](#index)</small>

# Unidad 3 <a name="U3"></a> <small>[:arrow_heading_up:](#index)</small>

## Definición de la derivada

>La **derivada** de una función es un número, que resulta de la aplicación de cierto límite.

&nbsp;

Si $f(x)$ es una función, entonces la *derivada* de $f(x)$ en el punto $a$ se define así:

$$
f'(a) = \lim\limits_{h \to 0} \frac{f(a+h)-f(a)}{h} 
$$

O así:

$$
f'(a) = \lim\limits_{t \to a} \frac{f(t)-f(a)}{t-a}
$$

&nbsp;

Si $f(x)=x^2$ y $a=4$.

| $f'(a) = \lim\limits_{h \to 0} \frac{f(a+h)-f(a)}{h}$ | $f'(a) = \lim\limits_{t \to a} \frac{f(t)-f(a)}{t-a}$ |
| :--- | :--- |
| $f'(4) = \lim\limits_{h \to 0} \frac{f(4+h)-f(4)}{h}$ |$f'(4) = \lim\limits_{t \to 4} \frac{f(t)-f(4)}{t-4}$ |
| $= \lim\limits_{h \to 0} \frac{(4+h)^2-16}{h}$ | $= \lim\limits_{t \to 4} \frac{t^2-16}{t-4}$ |
| $= \lim\limits_{h \to 0} \frac{\cancel{16}+8h+h^2-\cancel{16}}{h}$ | $= \lim\limits_{t \to 4} \frac{(t+4)\cancel{(t-4)}}{\cancel{(t-4)}}$ |
| $= \lim\limits_{h \to 0} \frac{\cancel{h}(8+h)}{\cancel{h}}$ | $= \lim\limits_{t \to 4} (t+4) = 8$ |
| $= \lim\limits_{h \to 0}(8+h)=8$ | |


&nbsp;

## Fórmulas de Derivación

Las fórmulas de derivación nos servirá para poder calcular las derivadas sin tener que resolver los límites.

| **Función** | **Derivada** |
| :---: | :---:|
| $f(x) = c$ | $f'(x) = 0$ |
| $f(x) = x$ | $f'(x) = 1$ |
| $f(x) = x^n$ | $f'(x) = nx^{n-1}$ |
| $f(x) = \sqrt{x}$ | $f'(x) = \frac{1}{2\sqrt{x}}$ |
| $f(x) = sen(x)$ | $f'(x) = cos(x)$ |
| $f(x) = cos(x)$ | $f'(x) = -sen(x)$|
| $f(x) = tan(x)$ | $f'(x) = sec^{2}(x)$|
| $f(x) = e^{x}$ | $f'(x) = e^{x}$|
| $f(x) = ln(x)$ | $f'(x) = \frac{1}{x}$|

## Reglas de Derivación

Las fórmulas anteriores son importantes, pero no son suficientes pues no podríamos conocer las derivadas de funciones un poco más complejas. 

En este momento introducimos una nueva notación para la derivada: 

$$
f' =\frac{df}{dx} \text{ o equivalentemente } f'(x)=\frac{df}{dx}(x) 
$$

Usamos esta notación nueva para expresar las siguientes *Reglas de Derivación*:

| $\frac{d}{dx}[cf] = c(\frac{df}{dx})$ | --- |
| :---: | :---: |


## Ejercicios de Derivadas

- a) $\textcolor{gold}{f(x) = 4x^5 - 3x^4 - 6x^3 + 8x^2 + x - 4}$
  1. $20x^{4} - 12x^{3} - 18x^{2} + 16x + 1 - \cancel{0}$
- b) $\textcolor{gold}{f(x) = \sqrt{2}e^{3}}$
  1. $0$
- c) $\textcolor{gold}{f(x) = cos(t) + y^{3}}$
  1. $0$
- d) $\textcolor{gold}{f(x) = 4ln(x) - 3 \sqrt{x}}$
  1. $4(\frac{1}{x}) - 3(\frac{1}{2\sqrt{x}})$
  2. $\frac{4}{x} - \frac{3}{2\sqrt{x}}$
- e) $\textcolor{gold}{f(x) = \frac{5}{x^{2}}}$
  1. $\frac{(0)(x^{2})-(2x)(5)}{(x^{2})^{2}}$
  2. $\frac{\cancel{(0)(x^{2})}-(10x)}{x^{4}}$
  3. $\frac{-10x}{x^{4}}$
  4. $-10x^{-3}$
- f) $\textcolor{gold}{\sqrt[3]{x^{2}}}$
  1. $x^{\frac{2}{3}}$
  2. $\frac{2}{3}x^{-\frac{1}{3}}$
- g) $\textcolor{gold}{x^{3}e^{x}}$
  1. $3x^{2}e^{x} + x^{3}e^{x}$

## La Derivada como pendiente de recta tangente


