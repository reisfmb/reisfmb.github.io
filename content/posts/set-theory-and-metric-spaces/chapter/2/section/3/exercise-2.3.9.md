---
weight: 239
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.3.9
description: Chap. 1 Exercise 2.3.9
date: 2022-04-30
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $A$ be a subset of a metric space $M$.

a) If $U$ is an open set in $M$, prove that $U \cap A$ is open in the metric space $A$.

b) If $F$ is a closed set in $M$, prove that $F \cap A$ is closed in $A$.

c) Prove that any open (resp. closed) set in $A$ is obtainable in this way from an open (resp. closed) set in $M$.

### Solução

#### a
Seja $x \in U \cap A$. Como $U$ é espaço métrico em $M$ então segue que existe $B_r(x) = \lbrace m \in M \mid D(x,m) < r \rbrace \subset U$. O conjunto $B_r(x) \cap A$ é uma bola aberta em $U \cap A$, logo $U \cap A$ é aberto.

#### b
Basta mostrar que $(F \cap A)^c$ é aberto. Perceba então que 

$$
(F \cap A)^c = F^c \cup A^c
$$

e como $F$ é fechado, então $F^c$ é aberto, logo caímos no mesmo caso a letra (a) e portanto $F^c \cup A^c$ é aberto, logo $F \cap A$ é fechado.

#### c
Seja $B \subset A$ um aberto. Basta tomar $U \in M$ aberto tal que $U \cap A = B$.
