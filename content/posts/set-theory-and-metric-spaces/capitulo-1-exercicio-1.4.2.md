---
weight: 142
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.2
description: Chap. 1 Exercise 1.4.2
date: 2022-04-03
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
---
### Pergunta
Let $f: A \rightarrow B$ and $g: B \rightarrow C$ be given functions.

a) If $f$ and $g$ are onto, prove that $gf$ is onto.

b) If $gf$ is onto, prove that $g$ is onto.

c) If $gf$ is onto and $g$ is one-to-one, prove that $f$ is onto.

d) Give an example where $gf$ is onto, but $f$ is not.

### Solução

#### a
Seja $c \in C$. Vamos mostrar que existe $a \in A$ tal que $(gf)(a) = c$. Do fato que $g$ é sobrejetora, segue que existe $b \in B$ tal que $c = g(b)$. Do fato que $f$ é sobrejetora, segue que existe $a \in A$ tal que $b = f(a)$. Logo $c = g(b) = g(f(a)) = (gf)(a)$.

#### b
Em busca de contradição, suponha que $g$ não seja sobrejetora, isso é, existe $c \in C$ tal que $\forall b \in B$. Segue que $g(b) \neq c$. Perceba em particular que se, se $b \in f(A)$, $g(b) \neq c$, logo $gf$ não pode ser sobrejetora. Contradição, logo $g$ é sobrejetora.

#### c
Seja $b \in B$. Vamos mostrar que existe $a \in A$ tal que $f(a) = b$. Seja $g(b) = c$. Como $gf$ é sobrejetora, segue que $\exists a \in A$ tal que $(gf)(a) = c$. Perceba então que $(gf)(a) = g(f(a)) = c = g(b)$. Como $g$ é injetora, segue que $f(a) = b$.

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
g(b_1) = c_1, g(b_2) = c_2, g(b_3) = c_2 \newline
$$