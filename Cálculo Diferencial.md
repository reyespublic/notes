---
tags: [School]
title: Cálculo Diferencial
created: '2020-02-16T06:42:49.001Z'
modified: '2020-02-17T16:06:35.192Z'
---

# Cálculo Diferencial

Libreta para la materia de *Cálculo Diferencial*.

# Unidad 3:

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
