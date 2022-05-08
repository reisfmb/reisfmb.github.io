---
weight: 243
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.4.3
description: Chap. 1 Exercise 2.4.3
date: 2022-04-30
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $A$ be a fixed subset of a metric space $M$. The function $f(x) = D(A,x)$ maps $M$ into the real numbers - see [Exercise 4.3.10](../3/exercise-2.3.10). Prove that $f$ is continuous.

### Solução
Seja $x_0 \in M$ e $\epsilon$ um numero real positivo. Mostraremos que existe $\delta$ real positivo tal que $D(x,x_0) < \delta \implies D(f(x),f(x_0)) < \epsilon$.

$$
D(f(x),f(x_0)) = |D(A,x) - D(A,x_0)|
$$

onde $D(A,x) = \inf \lbrace D(a,x) \mid a \in A \rbrace$.

Da desigualdade triangular segue que para $z \in M$, tem-se:

$$
D(a,x) \leq D(a,z) + D(z,x)
$$

Como $D(A,x) \leq D(a,x)$ para todo $a \in A$, segue:

$$
D(A,x) \leq D(a,z) + D(z,x) \implies D(A,x) - D(z,x) \leq D(a,z)
$$

Mas como $D(A,z)$ é o ínfimo, então

$$
D(A,x) - D(z,x) \leq D(A,z) \implies D(A,x) - D(A,z) \leq D(z,x)
$$

Tomando $z = x_0$ temos que 

$$
D(A,x) - D(A,x_0) \leq D(x_0,x)
$$

E trocando $x$ por $x_0$:

$$
D(A,x_0) - D(A,x) \leq D(x,x_0)
$$

Logo 
$$
|D(A,x) - D(A,x_0)| \leq D(x,x_0) < \delta
$$

Portanto basta tomar $\delta = \epsilon$.
