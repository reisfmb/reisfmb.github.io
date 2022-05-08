---
weight: 242
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.4.2
description: Chap. 1 Exercise 2.4.2
date: 2022-04-30
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $u$ be a fixed point of a metric space $M$. The function $f(x) = D(u,x)$ maps $M$ into the real numbers. Prove that $f$ is continuous.

### Solução
Seja $x_0 \in M$ e $\epsilon$ um numero real positivo. Mostraremos que existe $\delta$ real positivo tal que $D(x,x_0) < \delta \implies D(f(x),f(x_0)) < \epsilon$.

Basta tomar $\delta = \epsilon$.

$$
\begin{align*}
D(f(x),f(x_0)) &= D(D(u,x), D(u,x_0)) \newline
&\leq ||u-x| - |(u-x_0)|| \newline
&\leq |u - x - u + x_0| \newline
&\leq |x_0 - x| \newline
&= D(x,x_0) \newline
&= \delta \newline
&= \epsilon
\end{align*}
$$

