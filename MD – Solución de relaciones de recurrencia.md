---
tags: [Notebook]
title: MD – Solución de relaciones de recurrencia
created: '2020-02-19T22:29:28.359Z'
modified: '2020-03-01T18:51:09.305Z'
---

# MD – Solución de relaciones de recurrencia

1. $a_{n} = e^{3}a_{n-1}$ con $a_{o} = e^{6}$

$$
\begin{aligned}
a_{3} &= e^{3}(a_{2}) \\
&= e^{3}(e^{3}(a_{1})) \\
&= e^{3}(e^{3}(e^{3}(e^{6}))) \\
\end{aligned} \\
\vdots \\
\boxed{a_{n} = a^{6} \cdot (e^{3})^{n}}
$$

2. $a_{n} - (\sqrt{A})a_{n-1} = 0$ con $a_{1} = 1$ y $A$ un entero positivo

Para $a_{2}$:

$$
\begin{aligned}
a_{2} - (\sqrt{A}(1)) &= 0 \\
a_{2} - \sqrt{A} &= 0 \\
a_{2} &= \sqrt{A}
\end{aligned}
$$

Para $a_{3}$:

$$
\begin{aligned}
a_{3} - (\sqrt{A})(a_{2}) &= 0 \\
a_{3} - (\sqrt{A})(\sqrt{A}) &= 0 \\
a_{3} - (A) &= 0 \\
a_{3} &= A
\end{aligned}
$$

Para $a_{4}$:

$$
\begin{aligned}
a_{4} - (\sqrt{A})(a_{3}) &= 0 \\
a_{4} - (\sqrt{A})(A) &= 0 \\
a_{4} &= A\sqrt{A}
\end{aligned}
$$

Para $a_{5}$:

$$
\begin{aligned}
a_{5} - (\sqrt{A})(a_{4}) &= 0 \\
a_{5} - (\sqrt{A})(A\sqrt{A}) &= 0 \\
a_{5} - (A^{2}) &= 0 \\
a_{5} &= A^{2}
\end{aligned}
$$

Para $a_{n}$:

$$
a_{n} = (\sqrt{A})^{n-1} - (\sqrt{A})^{n-1}
$$

3. $a_{n} = e^{n-1}a_{n-1}$ con $a_{1} = e^{2}$

Para $a_{2}$:

$$
\begin{aligned}
a_{2} &= e^{1}a_{1} \\ 
a_{2} &= e \cdot e^{2} \\
a_{2} &= e^{3}
\end{aligned}
$$

Para $a_{3}$:

$$
\begin{aligned}
a_{3} &= e^{2}a_{2} \\
a_{3} &= e^{2} \cdot e^{3} \\
a_{3} &= e^{5}
\end{aligned}
$$

Para $a_{4}$:

$$
\begin{aligned}
a_{4} &= e^{3}a_{3} \\
a_{4} &= e^{3} \cdot e^{5} \\
a_{4} &= e^{8}
\end{aligned}
$$

Para $a_{n}$:

$$
a_{4} = e^{3} \cdot (e^{2} \cdot (e^{1} \cdot e^{2})) \\
\vdots \\
\boxed{a_{n} = e^{(n-1)!} \cdot e^{2}}
$$

4. $a_{n} = (n^{2} - n)a_{n-1}$ con $a_{0} = 2$

$$
\begin{aligned}
a_{3} &= (3^{2} - 3) \cdot a_{2} \\ 
a_{3} &= (3^{2} - 3) \cdot ((2^{2} - 2) \cdot a_{1}) \\
a_{3} &= (3^{2} - 3) \cdot ((2^{2} - 2) \cdot ((1^{2} - 1) \cdot a_{0})) \\
a_{3} &= (3^{2} - 3) \cdot ((2^{2} - 2) \cdot ((1^{2} - 1) \cdot 2)) \\
a_{3} &= (3^{2} - 3) \cdot ((2^{2} - 2) \cdot ((0) \cdot 2)) \\
a_{3} &= (3^{2} - 3) \cdot ((2^{2} - 2) \cdot (0)) \\
a_{3} &= (3^{2} - 3) \cdot (0) \\
a_{3} &= 0 \\
\end{aligned} \\
\vdots \\
a_{n} = 0
$$

5. 
