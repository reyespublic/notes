---
title: MD – Solución de Relaciones de Recurrencia
created: '2020-03-10T15:07:26.297Z'
modified: '2020-03-11T05:05:41.125Z'
---

# MD – Solución de Relaciones de Recurrencia

### Jorge Vázquez, Jorge Reyes y Augusto Reyes

Marzo 6, 2020

---

1. $s_{n} = s_{n-1} + 5$ con $s_{1} = 5$

$$
s_{3} = s_{2} + 5 \\
s_{3} = (s_{1} + 5) + 5 \\
s_{3} = ((5) + 5) + 5 \\
s_{3} = 3n \\
\vdots \\
\textcolor{#69a847}{s_{n} = 5n}
$$

2. $b_{n} = 3b_{n-1}$ con $b_{1} = 5$

$$
\text{Dado el caso 1 que nos dice que: } a_{n} = Ca_{n-1} = C^{n-1} \cdot a_{1} \\
\space \\
\textcolor{#69a847}{b_{n} = 3^{n-1} \cdot 5}
$$

3. $f_{n} = nf_{n-1}$ con $f_{1} = 1$

$$
\text{Dado el caso 2 que nos dice que: } a_{n} = g(n)a_{n-1} = a_{1}\prod^{n}_{k=2}g(k)\\
f_{n} = 1\prod^{n}_{k=2}k \implies \textcolor{#69a847}{n!}
$$

4. $s_{n} = ns_{n-1} + n!$ con $s_{1} = 1$

$$
\text{Dado el caso 5 que nos dice que: } \\
a_{n} = a_{1} \prod^{n}_{k=2}g(k) + \Big(\sum^{n-1}_{k=2}f(k) \prod^{n}_{r=k+1}g(r)\Big) + f(n) \\
\space \\
s_{n} = (1) \prod^{n}_{k=2}k + (\sum^{n-1}_{k=2}(k! \prod^{n}_{r=k+1}r))+n! \\
\space \\
\Downarrow \\
\space \\
n! + (\sum^{n}_{k=2}(k! \prod^{n}_{r=k+1})) + n! \\
\space \\
n! (2 + \sum^{n}_{k=2}(k! {n! \over 2})) \\
\space \\
\textcolor{#69a847}{n! (2 +  {1 \over 2} \sum^{n}_{k=2}k!)}
$$

5. $P_{n} = 3^{n+1}P_{n-1} + n$ con $P_{1} = 2$

$$
2 \prod^{n}_{k=2}3^{k+1} + (\sum^{n-1}_{k=2}(k \prod^{n}_{r=k+1}3^{r+1})) + n \\
\space \\
\Downarrow \\
\space \\
\textcolor{#69a847}{2\cdot3 \prod^{n}_{k=2}3^{k} + (\sum^{n-1}_{k=2}(k \prod^{n}_{r=k+1}3^{r+1})) + n} \\
$$

6. Un email de tipo SPAM que contiene un virus se envia a $1000$ direcciones electrónicas. Después de un segundo, cada máquina receptora envía $10$ nuevos emails con el virus después de lo cual el virus se deshabilita a si mismo en la máquina receptora.

  + Escriba una relación de recurrencia para el número de e-mails enviados al inicio del $n$-esimo segundo.

   $$
   \textcolor{#69a847}{a_{n} = 10a_{n-1} \text{ con } a_{0} = 1000} 
   $$

   + Resuelva la relación de recurrencia

   $$
   \textcolor{#69a847}{10^{n} \cdot 1000 \to 10^{n+3}}
   $$

   + ¿Cuántos e-mails son enviados al final de 20 segundos?

   $$
   \textcolor{#69a847}{10^{23}}
   $$

7. A un crédito de $5000$ pesos se le carga una tasa del $12%$ de interés anual. UN pago de $80$ pesos se realiza una vez cada mes.

  + Escriba una relación de recurrencia para el saldo restante del crédito al comienzo del mes $n$.

   $$
   \textcolor{#69a847}{a_{n} = 1.01a_{n-1} - 80 \text{ con } a_{0} = 5000}
   $$

  + Resuelva la relación de recurrencia

   $$
   \textcolor{#69a847}{1.01^{n} \cdot 5000 - 80 \sum^{n-1}_{k=0}1.01^{k}}
   $$

  + ¿Cuál es el saldo restante al comienzo del mes $19$?

   $$
   \textcolor{#69a847}{1.01^{19} \cdot 5000 - 80 \sum^{18}_{k=0}1.01^{k}}
   $$

8. $S_{n} = S_{n-1} + 2S_{n-2}$ con $S_{1} = 4$ y $S_{2} = -2$

$$
x^{2} + x - 2 
\begin{cases}
x_{1} = 1 \\
x_{2} = -2
\end{cases} \\
\Downarrow \\
A(1)^{n} + B(-2)^{n}\\
\space \\
a_{1} = A - 2B = 4 \\
a_{2} = A + 4B = -2 \\
\space \\
A = 4 + 2B \\
\space \\
4 + 2B + 4B = -2 \implies 6B = -6 \implies \textcolor{gold}{B=-1} \\
A = 4 + 2(-1) \implies 4 - 2 \implies \textcolor{gold}{A = 2} \\
\space \\
\Downarrow \\
\space \\
\textcolor{#69a847}{a_{n} = 2(1)^{n} - 1(-2)^{n}}
$$

9. $S_{n} = -10S_{n-1} - 25S_{n-2}$ con $S_{1} = -10$ y $S_{2} = 40$

$$
x^{2} + 10 + 25 
\begin{cases}
x_{1} = -5\\
x_{2} = -5
\end{cases} \\
\Downarrow \\
A(-5)^{n} + Bn(-5)^{n} \\
\space \\
a_{1} = -5A  -5B = -10 \\
a_{2} = 25A + 50B = 40 \\
\space \\
A = {-10 + 5B \over -5} \\
\space \\
25({-10 + 5B \over -5}) + 50B = 40 \\
{-250 + 125B \over -5} + 50B = 40 \\
{-250 + 125B \over -5} = 40 - 50B \\
-250 + 125B = -5(40 - 50B) \\
-250 + 125B = -200 + 250B \\
-125B = 50 \\
\space \\
\textcolor{gold}{B = {50 \over -125} = -{2 \over 5}} \\
\space \\
A = {-10 + 5(-{2 \over 5}) \over -5} \\
\space \\
A = {-10 + -2 \over -5} \\
\space \\
\textcolor{gold}{A = {12 \over 5}}
$$

$$
\textcolor{69a847}{{12 \over 5}(-5)^{n} -{2 \over 5}n(-5)^{n}}
$$

10. $P_{n} = 2P_{n/2} + 3$ con $n = 2^{m}$ y $P_{1} = 1$

$$
P_{8} = 2P_{4} + 3 \\
P_{8} = 2(2P_{2} + 3) + 3 \\
P_{8} = 2(2(2P_{1}+3)+3)+3 \\
P_{8} = 2(2(2(1)+3)+3)+3 \\
\space \\
2^{3} + 3 \cdot 2^{2} + 3 \cdot 2^{1} \\
2^{n} + 3 \cdot 2^{n-1} + 3 \cdot 2^{n-2} + 3 \cdot 2^{n-3} \\
\space \\
\textcolor{69a847}{2^{m} + 3 \sum^{m-1}_{k=0}2^{k}} \text{ y } \textcolor{69a847}{m = log_{2}n}
$$

11. $4a_{n} = -4a_{n-2} + (n+1)2^{n}$

$$
4a_{n} = -4a_{n-2} + (n+1)2^{n} \\
4x^{2} = -4 \\
x^{2} = -1 \\
x = \pm \sqrt{-1} \\
x = \pm i \\
\space \\
Ai^{n} + B(-i)^{n} \\
\space \\
F(n) = (n+1)2^{n} \\
a_{n}^{(p)} = 2^{n}(Cn+D) \\
\space \\
4(2^{n}(Cn+D)) = -4(2^{n-2}(C(n-2) +D)) + (n+1)2^{n} \\
4(2^{n}(Cn+D)) = -4(2(Cn - 2c +D)) + (n+1)2^{n} \\
16Cn + 8Cn + 16C + 16D + 8D + 4n + 4 = 0\\
\space \\
n(16C + 8C + 4) = 0 \\
24C = -4 \\
\textcolor{gold}{C = -{1 \over 6}} \\
\space \\
16C + 24D + 4 = 0 \\
-{8 \over 3} + 24D = - 4 \\
D = - {4 \over 3 \cdot 24} = \textcolor{gold}{-{1 \over 18}} \\
\space \\
\textcolor{69a847}{A(0 + i)^{n} + B(0 - i)^{n} + 2^{n}(-{n \over 6} - {1 \over 18})}
$$

12. $a_{n+2} + 3a_{n+1} + 2a_{n} = 3^{n}$ con $a_{0}$ y $a_{1} = 1$

$$
a_{n} + 3a_{n-1} + 2a_{n-2} = 3^{n} \\
a_{n} = -3a_{n-1} - 2a_{n-2} + 3^{n} \\
x^{2} = -3x -2 \\
x^{2} + 3x + 2 \\
(x+2)(x+1) 
\begin{cases}
x_{1} = -2 \\
x_{2} = -1
\end{cases}\\
\space \\
A(-2)^{n} + B(-1)^{n} \\
\space \\
F(n) = 3^{n} \\
A_{n}^{(p)} =3^{n} C \\
\space \\
3^{n} C = -3(3^{n-1}C) -2(3^{n-2}) + 3^{n} \\
3^{2} C = -3(3C) - 2(C) + 3^{2} \\
20C = 9 \\
\textcolor{gold}{C = {9 \over 20}} \\
\space \\
A(-2)^{n} + B(-1)^{n} + {9 \over 20} \cdot 3^{n} \\
\space \\
A + B = - {9 \over 20} \\
-2A -B = - {7 \over 20} \\
\Downarrow \\
-A = - {16 \over 20} \\
\textcolor{gold}{A = {16 \over 20}} \\
\space \\
{16 \over 20} + B = - {9 \over 20} \\
\space \\
B = - {9 \over 20} - {16 \over 20} \\
\space \\
\textcolor{gold}{B = - {5 \over 4}} \\
\space \\
\textcolor{69a847}{{4 \over 5}(-2)^{n} - {5 \over 4}(-1)^{n} + {9 \over 20} \cdot 3^{n}}
$$

13. $a_{n} + 4a_{n-1} + 4a_{n-2} = 7n(-2)^{n}$ con $a_{0} = 1$ y $a_{1} = 2$


14. Determine la solución general de la relación de recurrencia $a_{n} = -5a_{n-1} - 6a_{n-2} + 42(4^{n})$

$$
x^{2} + 5x + 6 = 0 \\
(x+2)(x+3) = 0 
\begin{cases}
x_{1} = -2 \\
x_{2} = -3
\end{cases} \\
\space \\
A(-2)^{n} + B(-3)^{n} \\
\space \\
F(n) = 42(4^n) \\
a_{n}^{(p)} = C4^{n} \\
4^{n}C = -5(4^{n-1}) - 6(4^{n-2}) + 42(4^{n}) \\
4^{2}C = -5(4) - 6 + 42(4^{2}) \\
16C = -20 - 6 + 42(16) \\
16C = 646 \\
\textcolor{gold}{C ={646 \over 16} = {323 \over 8}} \\
\space \\
\textcolor{69a847}{A(-2)^{n} + B(-3)^{n} + {323 \over 8}(4^{n})}
$$

15. Escriba un problema que pueda ser planteado como una recurrencia lineal no homogénea con coeficientes constantes de segundo orden. Considere que la parte no homogénea es $f(n) = n(e^{n})$. Resuelva completamente la relación de recurrencia resultante tomando en cuenta que $a_{0} = 1$, $a_{1} = 2 + e$.

> Se anexan las fotos de los apuntes y procedimientos
