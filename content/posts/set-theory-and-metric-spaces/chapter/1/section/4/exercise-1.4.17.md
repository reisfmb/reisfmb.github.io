---
weight: 1417
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.17
description: Chap. 1 Exercise 1.4.17
date: 2022-04-05
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
---
### Pergunta
Let $f$ be a map of the set $A$ to itself.

a) If $B$ and $C$ are subsets with $f(B) = B$ and $f(C) = C$, prove that $f(B \cup C) = B \cup C$.

b) Extend part a to any number of subsets.

c) Prove that there is a unique largest subset of $A$ which is carried onto itself by $f$.

d) If $B$ and $C$ are subsets with $f$ one-to-one on $B$ and $C$, is $f$ necessarily one-to-one on $B \cup C$ ?

### Solução

#### a
Segue direto do fato demonstrado [na letra (a)](/posts/set-theory-and-metric-spaces/capitulo-1-exercicio-1.4.10/) e das premissas $f(B) = B$ e $f(C) = C$.

#### b
Já foi mostrado a validade para o caso de $2$ subconjuntos $B$ e $C$ no item anterior. Tomemos esse como o caso base. Considere então válido para a união de $j \leq n$ subconjuntos de $A$, nomeadamente $S_1, S_2, \cdots, S_n$. Mostraremos ser válido para $\bigcup_{i=1}^{n+1} S_i$.

$$
\begin{align*}
  f(S_1 \cup S_2 \cup \cdots \cup S_n \cup S_{n+1})
  &= f(S_1 \cup S_2 \cup \cdots \cup (S_n \cup S_{n+1})) \newline
  &= f(S_1) \cup f(S_2) \cup \cdots \cup f(S_n \cup S_{n+1}) \newline
  &= f(S_1) \cup f(S_2) \cup \cdots \cup f(S_n) \cup f(S_{n+1}) \newline
  &= S_1 \cup S_2 \cup \cdots \cup S_n \cup S_{n+1}
\end{align*}
$$

#### c
Queremos mostrar que existe somente um maior subconjunto $S \subset A$ tal que $f(S)$ é sobrejetora.
  
Primeiro vamos garantir que tal subconjunto existe. 

Para ver isso, perceba que se $f(a) = a$ para algum $a \in A$ então $\lbrace a \rbrace$ é tal conjunto, uma vez que $\lbrace a \rbrace \subset A$ e $f(\lbrace a \rbrace) = \lbrace a \rbrace$.

Suponha então que $\forall a \in A$, $f(a) \neq a$.

$$
???
$$

Agora vamos mostrar a unicidade do maior subconjunto com tal propriedade.

Suponha que $B,C \subset A$ tais que $B \neq C$, $f(B) = B$ e $f(C) = C$. Segue que $f(B \cup C) = f(B) \cup f(C) = B \cup C$. Mas $B,C \subsetneq B \cup C$. Absurdo dado que assumimos que $B$ e $C$ são os maiores subconjuntos com tal priopriedade.

#### d
Não. Considere que $A = B \cup C$ tais que $B = \lbrace 1,2 \rbrace$ e $C = \lbrace 3,4 \rbrace$. Defina $f: A \rightarrow A$ da seguinte forma:

- $ f(1) = 3 $
- $ f(2) = 4 $
- $ f(3) = 3 $ 
- $ f(4) = 4 $

Repare que $f$ restrita à $B$, assim como $f$ restrita à $C$, é injetiva, mas $f$ restrita à $B \cup C$ não.
