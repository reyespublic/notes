---
title: MD – Aplicación de las Relaciones de Recurrencia
created: '2020-03-05T19:19:47.186Z'
modified: '2020-03-07T02:16:13.604Z'
---

# MD – Aplicación de las Relaciones de Recurrencia

## Sucesión de Fibonacci

La sucesión comienza con os números de $0$ y $1$, a partir de estos, cada término es la suma de los dos anteriores. 

La relación de recurrencia es:

$$
a_{n} = a_{n-1} + a_{n-2}
$$

Con los casos iniciales $a_{0} = 0$ y $a_{1} = 1$

Nos podemos dar cuenta que la relación de recurrencia es de órden $2$, por lo que podemos usar la fórmula de la ecuación característica. 

1. Primero planteamos la ecuación:

$$
x^{2} - x - 1 = 0
$$

2. Conseguimos las raíces usando la fórmula general:

$$
x = {1 \pm \sqrt{5} \over 2} 
\begin{cases}
x_{1} = {1 + \sqrt{5} \over 2} \\
x_{2} = {1 - \sqrt{5} \over 2} 
\end{cases}
$$

3. Sustituímos los valores de las raíces en la fórmula. (Se usa esta fórmula ya que las raíces son diferentes)

$$
\def\rU{{1 + \sqrt{5} \over 2}}
\def\rD{{1 - \sqrt{5} \over 2}}

a_{n} = Ar^{n} + Br^{n} \\
\Downarrow \\
a_{n} = A(\rU)^{n} + B(\rD)^{n}
$$

4. Conseguimos dos ecuaciones con los casos base dados:

$$
\def\ru{{1 + \sqrt{5} \over 2}}
\def\rd{{1 - \sqrt{5} \over 2}}

a_{0} = 0 = A(\ru)^{0} + B(\rd)^{0} \\
\Downarrow \\
\boxed{a_{0} = 0 = A + B}
\space \\
\space \\
a_{1} = 1 = A(\ru)^{1} + B(\rd)^{1} \\
\Downarrow \\
\boxed{a_{1} = 1 = A(\ru) + B(\rd)}
$$

5. Conseguimos los valores de $A$ y $B$

$$
\def\ru{{1 + \sqrt{5} \over 2}}
\def\rd{{1 - \sqrt{5} \over 2}}
\def\A{-({1 \over -(\ru) + (\rd)})}
\def\B{{1 \over -(\ru) + (\rd)}}

\begin{aligned}
A + B &= 0 \\
A(\ru) + B(\rd) &= 1
\end{aligned} \\
\vdots \\
A = -B \\
\space \\
\space \\
-B(\ru) + B(\rd) = 1 \\
B(-(\ru) + (\rd)) = 1 \\
B = \B \\
A = \A
$$

6. Por lo que la fórmula general nos queda:

$$
\def\ru{{1 + \sqrt{5} \over 2}}
\def\rd{{1 - \sqrt{5} \over 2}}
\def\A{-({1 \over -(\ru) + (\rd)})}
\def\B{{1 \over -(\ru) + (\rd)}}

a_{n} = \A(\ru)^{n} + \B(\rd)^{n} \\
\Downarrow \\
a_{n} = \B(-(\ru)^{n} + (\rd)^{n}) \\
\Downarrow \\
\boxed{a_{n} = {-(\ru)^{n} + (\rd)^{n} \over -(\ru) + (\rd)}}
$$

De esta forma damos con la fórmula cerrada de la relación de recurrencia.

En conclusión podemos ver como en este ejercicio para encontrar la relación de recurrencia de la sucesión de Fibonacci logramos tanto encontrar su **R.R** como su **Fórmula cerrada**. Para llegar a ese resultado de una forma óptima usamos las fórmulas establecidas (como el método de la ecuación característica).

