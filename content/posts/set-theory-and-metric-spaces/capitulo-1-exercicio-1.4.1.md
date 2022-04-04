---
weight: 141
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.1
description: Chap. 1 Exercise 1.4.1
date: 2022-04-03
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
---
### Pergunta
Let $f: A \rightarrow B$ and $g: B \rightarrow C$ be given functions.

a) If $f$ and $g$ are one-to-one, prove that $gf$ is one-to-one.

b) If $gf$ is one-to-one, prove that $f$ is one-to-one.

c) If $f$ is onto and $gf$ is one-to-one, prove that $g$ is one-to-one.

d) Give an example where $gf$ is one-to-one, but $g$ is not.

### Solução

#### a
$(gf)(a) = (gf)(b) \iff g(f(a)) = g(f(b)) \implies f(a) = f(b) \implies a = b$

#### b
Em busca de contradição, suponha que $f$ não seja injetora, ou seja, $\exists a,b \in A$ tais que $f(a) = f(b)$ mas $a \neq b$. Sendo assim $(gf)(a) = (gf)(b)$ mas $a \neq b$. Contradição, logo $f$ é injetora.

#### c
Considere $b_1, b_2 \in B$ tais que $g(b_1) = g(b_2)$. Como $f$ é sobrejetora, segue que existem $a_1, a_2 \in A$ tais que $b_1 = f(a_1)$ e $b_2 = f(a_2)$. Logo $g(f(a_1)) = g(f(a_2))$. Como $gf$ é injetora, segue que $a_1 = a_2$, ou seja, $b_1 = f(a_1) = f(a_2) = b_2$, logo $g$ é sobrejetora.

#### d
Considere os seguintes conjuntos:

$$
A = \lbrace a_1,a_2 \rbrace \newline
B = \lbrace b_1,b_2,b_3 \rbrace \newline
C = \lbrace c_1,c_2 \rbrace \newline
$$

Defina $f: A \rightarrow B$ e $g: B \rightarrow C$ da seguinte forma:

$$
f(a_1) = b_1, f(a_2) = b_2 \newline
g(b_1) = c_1, g(b_2) = c_2, g(b_3) = c_1 \newline
$$