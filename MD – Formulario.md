---
title: MD – Formulario
created: '2020-03-11T18:10:29.228Z'
modified: '2020-03-11T21:32:11.242Z'
---

# MD – Formulario

## **Iteración**

$$
a_{n} = a_{n-1} + 5 \\
\space \\
\Downarrow\\
\space \\
a_{3} = a_{2} + 5 \\
a_{3} = (a_{1} + 5 ) + 5 \\
a_{3} = ((a_{0} + 5) + 5) + 5 \\
$$

## **Suma Telescópica**

$$
a_{3} - \cancel{a_{2}} = 3 \\
\cancel{a_{2}} - \cancel{a_{1}} = 2 \\
\cancel{a_{1}} - a_{0} = 1
$$

## **Caso 1**

La recurrencia:

$$
a_{n} = Ca_{n-1}
$$

Tiene la solución:

$$
a_{n} = C^{n-1}a_{1}
$$

## **Caso 2**

La recurrencia:

$$
a_{n} = g(n)a_{n-1}
$$

Tiene la solución: 

$$
a_{n} = a_{1} \prod^{n}_{k=2}g(k)
$$

## **Caso 3**

La recurrencia:

$$
a_{n} = a_{n-1} + f(n)
$$

Tiene la solución:

$$
a_{n} = a_{1} + \sum^{n}_{k=2}f(k)
$$

## **Caso 4**

La recurrencia:

$$
a_{n} = Ca_{n-1} + f(n)
$$

Tiene la solución:

$$
a_{n} = C^{n-1}a_{1} + \sum^{n}_{k=2}C^{n-k}f(k)
$$

## **Caso 5**

La recurrencia:

$$
a_{n} = g(n)a_{n-1} + f(n)
$$

Tiene la solución:

$$
a_{n} = a_{1} \prod^{n}_{k=2}g(k) + \Big( \sum^{n-1}_{k=2} f(k) \prod^{n}_{r=k+1} g(r) \Big) + f(n)
$$

# Métodos de la ecuación Caracterísitca

## **Grado 1**

La recurrencia: 

$$
a_{n} = Ca_{n-1}
$$

Tiene como ecuación caracterísitca:

$$
r - C = 0
$$

y como raíz característica a $C$, por lo tanto la solución de la recurrencia está dada por:

$$
a_{n} = aC^{n}
$$

## **Grado 2**

1. $x^{2} - c_{1}x - c_{2} = 0$

2. $a_{n} = Ar_{1}^{n} + Br_{2}^{n}$

> Si las raíces son iguales entonces: $a_{n} = Ar^{n} + Bnr^{n}$

# Relaciones de recurrencia lineales no homogéneas con coeficientes constantes

| Forma de $F(n)$ | Ejemplo $F(n)$ | Forma de $a_{n}^{p}$ |
| :-------------: | :------------: | :------------------: |
| c, una constante|       $5$       |   $A$, una constante   |
|        $n$        |       $2n$      |        $An + B$      |
|        $n^{2}$   |    $3n^{2}$     |     $An^{2} + Bn + C$ |
| $n^{t}, t \in Z^{+}$ | $3n^{5} + 2$ | $A_{t}n^{t} + A_{t-1}n^{t-1} + ... + A_{1}n + A_{0}$ |
| $r^{n}, r \in R$ | $7^{n}$ | $Ar^{n}$ |
| $n^{t}r^{n}$ | $3^{n}(n^{3} - 2)$ | $r^{n}(A_{t}n^{t} + A_{t-1}n^{t-1} + ... + A_{1}n + A_{0}$) 

# Formulas de Sumatorias

$$
\sum^{n}_{k=0}ar^{k} (r \not = 0) = 
\boxed{{ar^{n+1} - a \over r - 1}, r \not = 1}
$$

$$
\sum^{n}_{k=1}k = 
\boxed{{n(n+1) \over 2}}
$$

$$
\sum^{n}_{k=1}k^{2} =
\boxed{{n(n+1)(2n+1) \over 6}}
$$

$$
\sum^{n}_{k=1}k^{3} =
\boxed{{n^{2}(n+1)^{2} \over 4}}
$$

$$
\sum^{\infin}_{k=0}x^{k}, |x| < 1 =
\boxed{{1 \over 1 - x}}
$$

$$
\sum^{\infin}_{k=1}kx^{k-1}, |x| < 1 = \boxed {{1 \over (1-x)^{2}}}
$$
