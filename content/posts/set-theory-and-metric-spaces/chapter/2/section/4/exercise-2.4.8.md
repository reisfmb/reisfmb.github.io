---
weight: 248
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.4.8
description: Chap. 1 Exercise 2.4.8
date: 2022-04-30
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
If $f: X \rightarrow Y$ is continuous at $x_0$, and $g: Y \rightarrow Z$ is continuous at $f(x_0)$, prove that $gf: X \rightarrow Z$ is continuous at $x_0$.

### Solução
Sejam $y_0 = f(x_0)$ e $z_0 = g(y_0)$.

Seja $x_0$ \in X$ e $\epsilon > 0$. Da continuidade de $g$ segue que existe $\delta_1 > 0$ tal que $D(y,y_0) < \delta_1 \implies D(g(y),z_0) < \epsilon$. Da continuidade da $f$ segue que existe $\delta_2 > 0$ tal que $D(x,x_0) < \delta_2 \implies D(f(x),y_0) < \delta_1$. Sendo assim:

$$
D(x,x_0) < \delta_2 \implies D(gf(x), gf(x_0)) < \epislon
$$