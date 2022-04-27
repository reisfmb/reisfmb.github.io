---
weight: 236
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.3.6
description: Chap. 1 Exercise 2.3.6
date: 2022-04-26
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Convergence
  - Closed Annalus
---
### Pergunta
a) Prove that a closed ball in a metric space is a closed set.

b) The ***sphere*** with radius $r$ and center $x$ is the set of all $y$ with $D(x,y) = r$. Prove that a sphere is a closed set.

c) Given a point $x$ in a metric space $M$, and positive numbers $r,s$ with $r < s$, prove that the set of all $y \in M$ satisfying $r \leq D(x,y) \leq s$ is closed.

### Solução

#### a
Seja $C_r(c) = \lbrace m \in M \mid D(c,m) \leq r\rbrace$ uma bola centrada em $c \in M$ e $x_i \rightarrow y$ uma sequência convergente em $M$ tal que $x_i \in C_r(c)$. Provaremos que $y \in C_r(c)$.

Suponha que $y \notin C_r(c)$, ou seja, $D(c,y) > r$. Tome $\epsilon = D(c,y) - r$, logo para $i$ suficientemente grande temos $D(x_i,y) < D(c,y) - r$. Pela desigualdade triangular, tem-se 

$$
D(c,y) \leq D(c,x_i) + D(x_i,y) < D(c,x_i) + D(c,y) - r
$$

o que implica

$$
r = D(c,y) - D(c,y) + r < D(c,x_i) 
$$

da onde segue que $x_i \notin C_r(c)$, absurdo, logo $y \in C_r(c)$.

#### b
Seja $S_r(x) = \lbrace m \in M \mid D(x,m) = r \rbrace$ e $C_r(x)$ como definido anteriormente. Repare então que 

$$
S_r(x) = C_r(x) \cap (B_r(x))^c
$$

$B_r(x)$ é aberto, logo $(B_r(x))^c$ é fechado. Como visto anteriormente, $C_r(x)$ também é fechado. Segue então que $S_r(x)$ é fechado.

#### c
Seja $A_{r,s}(x) = \lbrace m \in M \mid r \leq D(x,y) \leq M \rbrace$. Repare então que

$$
A_{r,s}(x) = C_s(x) \setminus B_r(x) = C_s(x) \cap B_r(x)^c
$$

E como $C_s(x)$ e $B_r(x)^c$ são fechados, segue que $A_{r,s}(x)$ também será.