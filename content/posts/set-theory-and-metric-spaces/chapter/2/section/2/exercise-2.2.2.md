---
weight: 222
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.2.2
description: Chap. 1 Exercise 2.2.2
date: 2022-04-18
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Open Sets
---
### Pergunta
Let $x$ and $y$ be distinct points in a metric space $M$. Prove that there exist in $M$ disjoint open sets $U$ and $V$ with $x \in U$, $y \in V$.

### Solução
Como $x \neq y$ então $D(x,y) > 0$. Sendo assim considere os seguintes conjuntos:

$$
U = \left\lbrace m \in M \mid D(x,m) < \frac{D(x,y)}{2} \right\rbrace = B_{\frac{D(x,y)}{2}}(x) \newline
V = \left\lbrace m \in M \mid D(y,m) < \frac{D(x,y)}{2} \right\rbrace = B_{\frac{D(x,y)}{2}}(y)
$$

Claramente $U,V$ são abertos pois são bolas abertas por definição.

Provaremos que $x \in U$, $y \in V$ e $U \cap V = \emptyset$. 

$x \in U$ pois $D(x,x) = 0 < \frac{D(x,y)}{2}$, e similarmente $y \in V$.

Suponha $z \in U \cap V$, ou seja, $z$ satisfaz as seguintes desigualdades:

- $D(x,z) < \frac{D(x,y)}{2}$
- $D(y,z) < \frac{D(x,y)}{2}$

Porém, pela desigualdade triângular segue que

$$
D(x,y) \leq D(x,z) + D(z,y)
$$

Como cada uma das parcelas da soma acima é menor que $\frac{D(x,y)}{2}$ então tem-se

$$
D(x,y) < \frac{D(x,y)}{2} + \frac{D(x,y)}{2} = D(x,y)
$$

Absurdo, logo $U \cap V = \emptyset$.