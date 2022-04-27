---
weight: 231
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.3.1
description: Chap. 1 Exercise 2.3.1
date: 2022-04-26
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Convergence
---
### Pergunta
If in a metric space a sequence converges to both $x$ and $y$, prove that $x = y$.

### Solução
Seja $x_i$ uma sequência em um espaço métrico $M$ tal que $x_i \rightarrow x$ e $x_i \rightarrow y$, ou seja, para $\epsilon \in \mathbb{R}^+$ segue que existem $n_x, n_y \in \mathbb{Z}^+$ tais que para $i > \max(n_x,n_y)$, $D(x_i,x) < \epsilon$ e $D(x_i,y) < \epsilon$, ou seja:

$$
D(x,y) \leq D(x,x_i) + D(x_i,y) < 2\epsilon 
$$

Suponha então que $x \neq y$, logo $D(x,y) > d > 0$, ou seja, $d < 2\epsilon$.

Tome então $\epsilon = \frac{d}{4}$. Para $i$ suficientemente grande, teremos então que $d < 2\frac{d}{4} = \frac{d}{2}$. Absurdo, logo $x = y$.