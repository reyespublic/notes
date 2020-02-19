---
pinned: true
tags: [Notebook, School]
title: Matemáticas Discretas – Notebook
created: '2020-02-16T06:42:59.547Z'
modified: '2020-02-19T22:32:18.555Z'
---

# Matemáticas Discretas – Notebook

Libreta para la materia de *Matemáticas Discretas*

## Relación de Recurrencias (R.R) 

1. Queremos contar el número de listas de longitud $n \ge 1$, formadas de $0$'s y $1$'s.

$$
a_{1} = 2 \\
a_{2} = 4 \\ 
a_{3} = 8 \\
\vdots \\
\underbrace{a_{n} = 2*a_{n-1}}_{\text{Relación de Recurrencia}}
$$

&nbsp;

2. Llamemos $a_{n}$ al número de regiones del plano que determinan $n$ rectas. Las rectas son tales que por cualquier punto del plano pasan a lo más desde ellas y ninguna de ellas es paralela a ninguna otra.

$$
\begin{aligned}
a_{n} &= a_{n-1} + n\\
a_{1} &= 2 \\
a{2} &= a_{n-1} + n \to 4 + 3 = 7 
\end{aligned}
$$

&nbsp;

3. Expresa el número de movimientos para resolver las *Torres de Hanoi* con $n$ discos.

$$
H_{n} = 2H_{n-1} + 1
$$

&nbsp;

4. Julián invierte 100 pesos en una cuenta que le paga un interés compuesto $i$ de manera anual. ¿Cuánto tendrá después de 30 años?

$$
a_{n} = a_{n-1} + ia_{n-1} = (1+i)a_{n-1}
$$

&nbsp;

$$
\begin{aligned}
a_{n} &= (1+i)a_{n-1} \\
&= (1+i)[(1+i)a_{n-2}] = (1+i)^{2} a_{n-2} \\
&= (1+i)^{2}[(1+i)a_{n-3}] = (1+i)^{3} a_{n-3} \\
&= (1+i)^{3}[(1+i)a_{n-4}] = (1+i)^{4} a_{n-4} \\
\end{aligned} \\
\vdots \\
\begin{aligned}
&= (1+i)^{n} a_{n-n} \\
&= (1+i)^{n} a_{0} \\
&= (1+i)^{n} 100 \\
a_{30} &= (1+i)^{n}100 \gets \text{Solución}
\end{aligned}
$$

&nbsp;

5. Encuentre una relación de recurrencia para el número de cadenas de bits de longitud $n$ que no tienen 2 ceros consecutivos.

| **Longitud de la cadena** | **Cadena(s)** |
| :---: | --- |
| 1 | 2 = ($\textcolor{lightgreen}{0}, \textcolor{lightgreen}{1}$) |
| 2 | 3 = ($\cancel{00}, \textcolor{lightgreen}{01}, \textcolor{lightgreen}{10}, \textcolor{lightgreen}{11}$)|
| 3 | 5 = ($\cancel{000}, \cancel{001}, \textcolor{lightgreen}{010}, \textcolor{lightgreen}{011}, \cancel{100}, \textcolor{lightgreen}{101}, \textcolor{lightgreen}{110}, \textcolor{lightgreen}{111}$) |

$$
\overbrace{a_{n} = a_{n-1} + a_{n-2}}^{\text{Solución}} \\
a_{1} = 2, a_{2} = 3
$$

&nbsp;

6. Tenemos una escalera con $n$ peldaños; a cada paso se permite subir 1 o 2 escalones. ¿De cuántas formas diferentes se puede subir? (Encontrar una R.R.)

$$
a_{n} = a_{n-1} + a_{n-2} \\
a_{1} = 1 \\
a_{2} = 2 
$$

&nbsp;

7. Encuentre la **relación de recurrencia (R.R)** para el número de bolitas en una piramide, donde la base de $a_{n}$ es de $n$ bolitas y se van reduciendo el número, hasta llegar a la punta, dónde sólo es $1$ bolita.

$$
a_{1} = 1 \\
a_{2} = 3 \\
a_{3} = 6 \\
a_{4} = 10 \\
a_{5} = 15 \\
\vdots \\
\boxed{a_{n} = n + a_{n-1}}
$$

&nbsp;

$$
\underbrace{\sum_{i=1}^{n}={n(n+1) \over 2}}_{\text{Forma cerrada}}
$$

&nbsp;

8. Sea $a_{n}$ el número de formas diferentes de pagar $n$ dolares.


|   Valor   | Tipo  |
|   :---:   |  :-:  |
| 1 dolar   |  $m$  |
| 2 dolares |  $m$  |
| 5 dolares | $m,b$ | 

> Donde $m$ es $'moneda'$ y $b$ es $'billete'$.

$$
a_{n} = a_{n-1} + a_{n-2} + a_{n-5} + a_{n-5}
$$



