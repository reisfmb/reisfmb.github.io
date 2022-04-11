---
weight: 212
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.1.2
description: Chap. 1 Exercise 2.1.2
date: 2022-04-09
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $M$ be a set with three elements $a,b$ and $c$. Define $D$ so that $D(x,x) = 0$ for all $x$, $D(x,y) = D(y,x) = $ a positive real number for $x \neq y$. Say $D(a,b) = r, D(a,c) = s, D(b,c) = t$ with $r \leq s \leq t$. Prove that $D$ makes $M$ a metric space if and only if $t \leq r + s$.

### Solução
$D(x,x) = 0$ para todo $x \in M$, $D(x,y) = D(y,x)$ e $D(x,y) > 0$ se $x \neq y$ são claras pela definição de $D$.

Suponha então que $D$ torne $M$ um espaço métrico, logo $D(x,y) = D(y,x)$ e além disso vale a desigualdade triangular, logo:

$$
D(b,c) \leq D(b,a) + D(a,c) \implies t \leq r + s
$$

Suponha agora que $t \leq r + s$. Vamos provar que $D(x,z) \leq D(x,y) + D(y,z)$

$$
t \leq r + s \implies D(b,c) \leq D(b,a) + D(a,c) \newline
r \leq s \leq t \implies r \leq s + t \implies D(a,b) \leq D(a,c) + D(c,b) \newline
r \leq s \leq t \implies s \leq r + t \implies D(a,c) \leq D(a,b) + D(b,c) \newline
$$