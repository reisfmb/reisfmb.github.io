---
weight: 161
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.6.1
description: Chap. 1 Exercise 1.6.1
date: 2022-04-07
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Countable sets
---
### Pergunta
Let $A$ be a countable set and suppose that there is a given function mapping $A$ onto a set $B$. Prove that $B$ is countable

### Solução
Como $A$ é contável, segue que existe bijeção $f: \mathbb{N} \rightarrow A$. Seja $g: A \rightarrow B$ a função sobrejetora do enunciado. 

Se $g$ for também injetora, então não há muito trabalho a fazer dado que $fg$ é a bijeção dos naturais ao conjunto $B$.

Suponha então $g$ não injetora.

Pelo fato de $A$ ser contável, segue que $A = \lbrace a_1, a_2, \cdots \rbrace$.

Para $S \subset A$ defina:

$$
I(S) = I(\lbrace a_{s1}, a_{s2}, \cdots \rbrace) = \lbrace s1, s2, \cdots \rbrace \subset \mathbb{N}
$$


Com tal definição, defina a seguinte função $h: B \rightarrow \mathbb{N}$

$$
h(b) = \min I(g^{-1}(\lbrace b \rbrace))
$$

Perceba então que é **suficiente mostrar que $h$ é injetiva**, pois caso seja, $h$ será bijeção com subconjunto de $\mathbb{N}$ e como todo subconjunto de um conjunto contável é contável, $B$ será contável.

Sejam $b_1, b_2 \in B$ tal que $h(b_1) = h(b_2)$, o que implica que:

$$
\min I(g^{-1}(\lbrace b_1 \rbrace)) = \min I(g^{-1}(\lbrace b_2 \rbrace))
$$

Para que os mínimos sejam iguais, é necessário então que exista ao menos um elemento em comum nos conjuntos $g^{-1}(\lbrace b_1 \rbrace)$ e $g^{-1}(\lbrace b_2 \rbrace)$. Tal suposição implica a existência de $a \in A$ tal que $g(a) = b_1$ e $g(a) = b_2$, logo, $b_1 = b_2$.
