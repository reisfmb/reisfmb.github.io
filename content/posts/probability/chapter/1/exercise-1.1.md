---
weight: 11
author: Bruno Reis
title: (Probabilidade) Capítulo 1, exercício 1.1
description: Chap. 1 Exercise 1.1
date: 2022-04-13
categories:
  - Probabilidade
tags:
  - Probability
---
### Pergunta
Considere o experimento resultante do lançamento de dois dados onde se observa o mínimo entre suas faces. Construa um modelo probabilístico associado.

### Solução

$$
\Omega = \lbrace 1,2,3,4,5,6 \rbrace^2
$$

Seja então $A_i$ tal que $i \in \lbrace 1,2,3,4,5,6 \rbrace$ os seguintes conjuntos

$$
A_i =
\lbrace (i,j) \mid i \leq j \text{ e } j \in \lbrace 1,2,3,4,5,6 \rbrace \rbrace 
\cup
\lbrace (j,i) \mid i \leq j \text{ e } j \in \lbrace 1,2,3,4,5,6 \rbrace \rbrace 
$$

Perceba então que podemos interpretar cada $A_i \subset \Omega$ como sendo o conjunto de todos os possiveis lançamentos de dois dados onde o menor número entre as duas faces para cima é $i$.

Considere então uma $\sigma$-álgebra $\mathcal{F}$ de subconjuntos de $\Omega$ tal que $A_i \in \mathcal{F}$.

Logo, associamos a seguinte função $P: \mathcal{F} \rightarrow \mathbb{R}$ todo $A \in \mathcal{F}$:

$$
P(A) = \frac{|A|}{|\Omega|} = \frac{|A|}{36}
$$

Sendo assim, teriamos as seguintes probabilidades para os eventos $A_i$:
$$
P(A_1) = 11 / 36 \newline
P(A_2) = 9 / 36 \newline
P(A_3) = 7 / 36 \newline
P(A_4) = 5 / 36 \newline
P(A_5) = 3 / 36 \newline
P(A_6) = 1 / 36 \newline
$$
