---
weight: 227
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.2.7
description: Chap. 1 Exercise 2.2.7
date: 2022-04-19
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Open Sets
  - Open Annalus
---
### Pergunta
Given a point $x$ in a metric space $M$, and positive numbers $r$, $s$ with $r < s$, prove that the set of all $y \in M$ satisfying $r < D(x,y) < s$ is open. (A reasonable name for such set is "open ring" or "open annalus").

### Solução
Defina $A_x = \lbrace y \in M \mid r < D(x,y) < s \rbrace$. Vamos mostrar que $A_x$ é aberto.

Seja $a \in A_x$ e considere $B_d(a)$ tal que $d = \frac{\min \lbrace D(x,a) - r, s - D(a,x) \rbrace}{2} $. Mostraremos que $B_d(a) \subset A_x$, o que prova que $A_x$ é aberto.

Seja $b \in B_d(a)$. Pela desigualdade triangular segue que

$$
D(x,b) \leq D(x,a) + D(a,b)
$$

Como $D(a,b) \leq \frac{s - D(a,x)}{2} < s - D(a,x)$ segue que $D(x,b) < D(x,a) + s - D(a,x) = s$.

Suponha então que $D(x,b) \leq r$, logo pela desigualdade triangular segue que

$$
D(a,x) \leq D(a,b) + D(b,x) \implies D(a,x) \leq D(a,b) + r \implies D(a,x) - r \leq D(a,b)
$$

Porém $D(a,b) \leq \frac{D(x,a) - r}{2} < D(x,a) - r$. Absurdo, logo $r < D(x,b)$.

Conclusão

$$
r < D(x,b) < s \implies b \in A_x \implies B_d(a) \subset A_x
$$
