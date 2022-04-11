---
weight: 213
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.1.3
description: Chap. 1 Exercise 2.1.3
date: 2022-04-09
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
On an arbitrary set $M$ suppose that $D(x,x) = 0$, and for $x \neq y$, $D(x,y) = D(y,x)$ is a number between $1$ and $2$ (the end points $1$ and $2$ are permitted). Prove that $M$ is a metric space.

### Solução
As condições enunciadas já garantem 3 das 4 verificações. 

Resta mostrar que $D(x,z) \leq D(x,y) + D(y,z)$ para todo $x,y,z \in M$.

Repare então que

$$
1 \leq D(x,z) \leq 2 \newline
2 \leq D(x,y) + D(y,z) \leq 4 \newline
$$

Logo

$$
D(x,z) \leq D(x,y) + D(y,z)
$$