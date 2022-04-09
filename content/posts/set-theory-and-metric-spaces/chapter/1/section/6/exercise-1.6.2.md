---
weight: 162
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.6.2
description: Chap. 1 Exercise 1.6.2
date: 2022-04-08
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Countable sets
---
### Pergunta
Prove that the cartesian product of two countable sets is countable. Generalize to the cartesian product of a finite number of sets.

### Solução
Sejam $A$ e $B$ conjuntos contáveis, ou seja, podemos ver $A$ e $B$ da seguinte forma:

$$
A = \lbrace a_1, a_2, \cdots \rbrace
\newline
B = \lbrace b_1, b_2, \cdots \rbrace
$$

Sendo assim, por definição $A \times B$ é o conjunto

$$
(a_1,b_1), (a_2,b_1), (a_3,b_1), \cdots \newline
(a_1,b_2), (a_2,b_2), (a_3,b_2), \cdots \newline
(a_1,b_3), (a_2,b_3), (a_3,b_3), \cdots \newline
\vdots \quad\quad \vdots \quad\quad \vdots \quad \ddots
$$

Faça a contagem via diagonal de cantor e acabou!

Para o produto cartesiano de um numero finito $N$ de conjuntos contáveis, basta aplicar indução.