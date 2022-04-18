---
weight: 2119
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.1.19
description: Chap. 1 Exercise 2.1.19
date: 2022-04-17
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $M$ be a set with a distance function $D$ satisfying the postulates for a metric space, expect the axiom II (p. 68) is weakened to $D(a,b) \geq 0$ for all $a,b$. Define $a \sim b$ to mean $D(a,b) = 0$. Prove that $\sim$ is an equivalence relation. Make the set of equivalence classes into a metric space in a natural way.

### Solução
Para que $\sim$ seja uma relação de equivalência deve satisfazer:

- $a \sim a$ para todo $a \in M$.
- $a \sim b$ s.s.e $b \sim a$.
- $a \sim b$ e $b \sim c$ implica que $a \sim c$.

$D(a,a) = 0$ para todo $a \in M$, ja que $D$ é "quase" uma métrica, não atendendo somente o axioma II, logo $a \sim a$.

$a \sim b$ implica que $D(a,b) = 0$, mas $D(a,b) = D(b,a)$ pelo axioma III, logo $b \sim a$.

$D(a,c) \leq D(a,b) + D(b,c)$. Se $a \sim b$ e $b \sim c$ então $D(a,c) \leq 0$. Como $\underbrace{D(a,c) \geq 0}_{\text{weakened axiom II}}$ para todo $a,c \in M$, segue que $D(a,c) = 0$, portanto $a \sim c$.

Seja então 

$$
X = \bigg\lbrace C_m \mid m \in M \text{ e } C_m = \lbrace a \mid D(a,m) = 0 \rbrace \bigg\rbrace
$$

X é o conjunto das classes de equivalência da relação definida no enunciado. Mostraremos que a seguinte função

$$
\begin{align*}
F:X^2 &\rightarrow \mathbb{R} \newline
F(C_a, C_b) &=
  \begin{cases}
  0 && \text{se $a \sim b$} \newline
  1 && \text{se $a \nsim b$} \newline
  \end{cases}
\end{align*}
$$

é uma métrica em $X$ que o torna um espaço métrico.


- $F(C_a,C_a) = 0$ pois $a \sim a$
- $F(C_a,C_b) = 1 > 0$ pois se $C_a \neq C_b$ então $a \nsim b$.
- $F(C_a,C_b) = F(C_b,C_a)$ pois se $a \sim b \implies a \sim b$ e $b \nsim a \implies a \nsim b$.
- $F(C_a,C_c) \leq F(C_a,C_b) + F(C_b,C_c)$ pois se $a \sim c$ então $0 \leq$ a soma de duas imagens de $F$ que são sempre não negativas. Se $a \nsim c$ então $a \nsim b$ ou $b \nsim c$, logo tem-se $1 \leq 1$ ou $1 \leq 2$.
