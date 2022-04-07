---
weight: 143
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.3
description: Chap. 1 Exercise 1.4.3
date: 2022-04-04
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
---
### Pergunta
Prove that a function $f: A \rightarrow B$ is one-to-one and onto if and only if there exists $g: B \rightarrow A$ with $gf = I_A$ and $fg = I_B$.

### Solução
Suponha que $f: A \rightarrow B$ seja uma bijeção. Segue diretamente que existe $f^{-1}: B \rightarrow A$, logo:

- $f \circ f^{-1} = I_A$
- $f^{-1} \circ f = I_B$

Suponha que exista $f: A \rightarrow B$ e $g: B \rightarrow A$ tal que $gf = I_A$ e $fg = I_B$. Vamos mostrar que $f$ é bijeção.

Seja $b \in B$. Em busca da sobrejetividade, vamos mostrar que $\exists a \in A$ tal que $f(a) = b$.

$$
g(b) = a \implies fg(b) = f(a) \implies b = f(a)
$$

Agora sejam $a_1, a_2 \in A$ tais que $f(a_1) = f(a_2)$. Em busca da injetividade vamos mostrar que $a_1 = a_2$.

$$
f(a_1) = f(a_2) \implies gf(a_1) = gf(a_2) \implies a_1 = a_2
$$
