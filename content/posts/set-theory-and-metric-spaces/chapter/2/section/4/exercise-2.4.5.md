---
weight: 245
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.4.5
description: Chap. 1 Exercise 2.4.5
date: 2022-04-30
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $X$ and $Y$ be metric spaces, $f$ a function from $X$ to $Y$.

a) If $X$ is a union of open sets $U_i$ on each which $f$ is continuous, prove that $f$ is continuous on $X$.

### Solução

#### a
Seja $V$ um aberto em $Y$. Provaremos que $f^{-1}(V) é um aberto$, o que implica que $f$ é contínua.

$$
\begin{align*}
f^{-1}(V) &= f^{-1}(V) \cap X = f^{-1}(V) \cap (\bigcup_{i}^\infty U_i) \newline
&= \bigcup_{i}^\infty (f^{-1}(V) \cap U_i) \newline
&= \bigcup_{i}^\infty (f|_{U_i}^{-1}(V))
\end{align*}
$$

E como $f$ é contínua em cada $U_i$ então $f|_{U_i}^{-1}(V)$ é aberto. União de abertos e aberta, logo $f^{-1}(V)$ será aberto.