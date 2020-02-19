---
pinned: true
tags: [Notebook, School]
title: Álgebra Superior – Notebook
created: '2020-02-16T06:42:21.402Z'
modified: '2020-02-19T22:32:14.039Z'
---

# Álgebra Superior – Notebook

Libreta para la clase de *Álgebra Superior*.

## Índice <a name="index"></a>

1. [Unidad 2](#U2)
   1. [Subconjuntos de conjuntos y conjunto potencia](#T1)
      1. [Subconjuntos](#T1S1)
      2. [Conjunto potencia](#T1S1)
   2. [Operaciones con conjuntos](#T2)
      1. [Unión](#T2S1)
      2. [Intersección](#T2S2)
      3. [Complemento](#T2S3)
      4. [Diferencia](#T2S4)
   3. [Demostraciones](#E1)

# Unidad 2 <a name="U2"></a> <small>[:arrow_heading_up:](#index)</small>

De manera intuitiva, un conjunto es una colección de objetos bien definidos de modo que dados un conjunto y un elemento se puede decir si el elemento pertenece o no al conjunto.

Es usual nombrar a los conjuntos por letras mayúsculas: $A, B, C, ...$ y representar los elementos de un conjunto por letras minúsculas: $a, b, c, ...$  generalmente se usan corchetes, $\{ \}$ para representar un conjunto.

Un conjunto se puede determinarde dos maneras: por extensión o por comprensión. Se dice que está dado por extensión si se dan en forma explícita sus elementos. Se dice que está dadopor comprensión si se da un criterio de pertenencia de sus elementos, es decir, cuando se enuncia la propiedad o propiedades que deben tener sus elementos.

> El conjunto vacio $\varnothing$ es un elemento que pertenece a cualquier conjunto.

## Subconjuntos de conjuntos y conjunto potencia <a name="T1"></a> <small>[:arrow_heading_up:](#index)</small>

### Subconjuntos <a name="T1S1"></a> <small>[:arrow_heading_up:](#index)</small>

Sean $A$ y $B$ conjuntos. Se dice que $A$ es subconjunto de $B$, lo cual se denota $A \subset B$, si todo elemento de $A$ también es elemento de $B$.

$$
A \subset B \iff (\forall x, x \in A \implies x \in B)
$$

**Propiedades:**
+ $A \subset A$
+ $\varnothing \subset A$
+ $A \subset B \land B \subset A \iff A = B$
+ $A \subset B \land B \subset C \rArr A \subset C$

### Conjunto potencia <a name="T1S2"></a> <small>[:arrow_heading_up:](#index)</small>

Sea $A$ un conjunto. Entonces el conjunto potencia de $A$ es el conjunto formado por todos los subconjuntos de $A$. Se denota $P(A)$ o $2^{A}$.

*Ejemplo:*

$$
\begin{aligned}
A &= \{a, b, c, d\} \\
P(A) &= \{\{a\}, \{b\}, \{c\}, \{d\}, \{a,b\}, \{a,c\}, \{a,d\}, \{b,c\}, \{b,d\}, \{c,d\}, \{a,b,c\}, \{a,b,d\}, \{a,c,d\}, \{b,c,d\}, \{a,b,c,d\}, \{\varnothing\}\}
\end{aligned}
$$

> En general si el número de elementos de $A$ es $n (n \in \Bbb N)$ entonces el número de elementos de $P(A)=2^{n}$.

## Operaciones con conjuntos <a name="T2"></a> <small>[:arrow_heading_up:](#index)</small>

### Unión <a name="T2S1"></a> <small>[:arrow_heading_up:](#index)</small>

Sean $A$ y $B$ subconjuntos de un conjunto universo $X$. Se define la unión de $A$ y $B$ como el conjunto.

$$
A \cup B = \{x \in X \space | \space x \in A \lor x \in B\}
$$

**Propiedades:**
+ $A \cup \varnothing = A$
+ $A \cup X = X$
+ $A \cup A = A$
+ $A \cup B = B \cup A \text{ (conmutativa)}$
+ $(A \cup B) \cup C = A \cup (B \cup C) \text{ (asociativa)}$
+ $A \subset A \cup B$

### Intersección <a name="T2S2"></a> <small>[:arrow_heading_up:](#index)</small>

Sean $A$ y $B$ subconjuntos de un conjunto universo $X$. Se define la intersección $A$ y $B$ como el conjunto. 

$$
A \cap B = \{x \in X \space | \space x \in A \land x \in B\}
$$

**Propiedades:**
+ $A \cap \varnothing = \varnothing$
+ $A \cap X = A$
+ $A \cap A = A$
+ $A \cap B = B \cap A \text{ (conmutativa)}$
+ $(A \cap B) \cap C = A \cap (B \cap C) \text{ (asociativa)}$
+ $A \cap B \subset C$
+ $A \cup (B \cap C) = (A \cup B) \cap (A \cup C) \text{ (distributiva)}$ 
+ $A \cap (B \cup C) = (A \cap B) \cup (A \cap C) \text{ (distributiva)}$ 

### Complemento <a name="T2S3"></a> <small>[:arrow_heading_up:](#index)</small>

Sea $X$ un conjunto universo. Sea $A \subset X$. Se define el complemento de $A$ como el conjunto de elementos en el universo $X$ que no pertenecen a $A$. Se denota $A^{c}$.

Así:

$$
A^{c} = \{x \in X \space | \space x \notin A\}
$$

**Propiedades:**
+ $A \cap A^{c} = \varnothing$
+ $A \cup A^{c} = X$
+ $(A^{c})^{c} = A$
+ $A \subset B \rArr B^{c} \subset A^{c}$
+ $(A \cup B)^{c} = A^{c} \cap B^{c}$
+ $(A \cap B)^{c} = A^{c} \cup B^{c}$

### Diferencia <a name="T2S4"></a> <small>[:arrow_heading_up:](#index)</small>

Sean $A$ y $B$ subconjuntos de un conjunto universo $X$. Entonces la diferencia de $A$ y $B$, denotado $A - B$, es el conjunto:

$$
A - B = \{x \in X \space | \space x \in A \land x \notin B\}
$$

**Propiedades:**
+ $A - A = \varnothing$
+ $X - A = A^{c}$
+ $A - B = A \cap B^{c}$
+ $B - (B - A) = A \cap B$
+ $A \subset B \rArr C - B \subset C - A$
+ $C - (A \cup B) = (C - A) \cap (C - B)$
+ $C - (A \cap B) = (C - A) \cup (C - B)$
+ $A \cap (B - C) = (A \cap B) - (A \cap C)$

---

## Demostraciones <a name="E1"></a>[:arrow_heading_up:](#index)</small>

1) $A \cap (B - C) = (A \cap B) - (A \cap C)$

$\text{Desmotración}$

$$
\begin{aligned}
(A \cap B) - (A \cap C) &= (A \cap B) \cap (A \cap C)^{c},\text{ prop. 3.} \\
&= (A \cap B) \cap (A^{c} \cup C^{c}), \text{ prop. DeMorgan} \\
&= [(A \cap B) \cap A^{c}] \cup [(A \cap B) \cap C^{c}], \text{ prop. distributiva} \\
&= [A \cap (B \cap A^{c})] \cup [A \cap (B \cap C^{c})], \text{ prop. asociativa} \\
&= [A \cap (A^{c} \cap B)] \cup [A \cap (B \cap C^{c})], \text{ prop. conmutativa} \\
&= [(A \cap A^{c}) \cap B]\cup[A \cap (B \cap C^{c})], \text{ prop. asociativa}\\ 
&= [\varnothing \cap B] \cup [A \cap (B \cap C^{c})], \text{ prop. complemento} \\
&= \varnothing \cup [A \cap (B \cap C^{c})], \text{ prop. } \varnothing \cap B = \varnothing \\
&= A \cap (B \cap C^{c}) \\ 
&= A \cap (B - C) \\
\therefore A \cap (B - C) &= (A \cap B) - (A \cap C). \\ \text{ y ya!}
\end{aligned} 
$$

2) Sea $X$ el conjunto unvierso y sean $A, B,$ y $C$ subconjuntos de $X$. Demuestra:

   + Si $A \subset B$ y $A \subset C$ entonces $A \subset B \cap C$

   $Demostración$

   $$
   \text{Por definición:} \\
   A \subset B \iff (\forall x, x \in A \rArr x \in B) \\
   \ \\
   \text{Entonces, si } A \subset B \text{ y } A \subset C \\
   \forall x \in A \space | \space x \in B \land x \in C \\
   \ \\
   \text{Por definición de Intersección: }\\
   A \cap B = \{x \in X \space | \space x \in A \land x \in B\} \\
   \ \\
   \therefore \space A \subset (B \cap C) \text{ y ya!} 
   $$

