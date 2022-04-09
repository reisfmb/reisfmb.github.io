---
weight: 163
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.6.3
description: Chap. 1 Exercise 1.6.3
date: 2022-04-08
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Countable sets
---
### Pergunta
Prove that the set of all finite subsets of a coutable set is countable. *(Hint: Use exercises 1 and 2.)*

### Solução
Seja $A$ um conjunto contável. Defina então:

$$
S = \lbrace B \subset A \mid \text{$B$ é finito} \rbrace
$$

Perceba então que

$$
S = \bigcup_{n \in \mathbb{N}} S_n
$$

onde

$$
S_n = \lbrace B \subset A \mid \text{$B$ é finito e $|B| = n$} \rbrace
$$

ou seja, $S$ é uma união contável de conjuntos. Se provarmos que $S_n$ é contável para cada $n \in \mathbb{N}$ então $S$ será contável.

Seja então $n \in \mathbb{N}$. definimos a seguinte função

$$
\begin{align*}
  f_n: \mathbb{N}^n &\rightarrow S_n \newline
  (m_1, m_2, \cdots, m_n) &\mapsto X \quad \text{ t.q } \quad a_{m_1}, a_{m_2}, \cdots, a_{m_n}\in X \subset A
\end{align*}
$$

Perceba que $f_n$ é bem definida como função.

É suficiente provar que $f_n$ é sobrejeção, [ver exercício 1.6.1](../exercise-1.6.1), dado que $\mathbb{N}^n$ é contável [ver exercício 1.6.2](../exercise-1.6.2)

Seja $X \in S_n$, ou seja, $X \subset A$ e $|X| = n$, logo 

$$
X = \lbrace a_{k_1}, a_{k_2}, \cdots, a_{k_n} \rbrace \implies f_n(k_1, k_2, \cdots, k_n) = X
$$

Assim sendo, $S_n$ é contável, o que implica que $S$ é contável.