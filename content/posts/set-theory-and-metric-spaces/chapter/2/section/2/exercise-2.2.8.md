---
weight: 228
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.2.8
description: Chap. 1 Exercise 2.2.8
date: 2022-04-19
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Open Sets
---
### Pergunta
Let $x$ be a point of a metric space $M$. Prove that the following two statements are equivalent:

a) $x$ is not isolated; 

b) every neighborhood of $x$ contains an infinite number of points of $M$.

### Solução

#### a -> b
Seja $x \in M$ tal que $x$ não seja isolado, isso é, para todo $r \in \mathbb{R}^+$, tem-se $|B_r(x)| \not\subset \lbrace x \rbrace$. 

Em particular, na verdade o que se tem é que $|B_r(x)| = \infty$, pois caso fosse finito, então todos seus pontos seriam isolados (tal demonstração está contida no [exercício 2.2.6](../exercise-2.2.6)).

Seja então $N \subset M$ uma vizinhança de $x \in M$ e $O \subset N$ o aberto da vizinhança que contém $x$. Segue então que existe $r \in \mathbb{R}^+$ t.q $B_r(x) \subset O \subset N$. Como $B_r(x)$ contém infinitos elementos pelo que foi apontado anteriormente, segue que $|N| = \infty$.

#### b -> a
Seja $x \in M$ e suponha que toda vizinhança de $x$ contenha uma infinidade de pontos de $M$.

Por contradição, assuma que $x$ seja isolado.

Do fato que $x$ é isolado, segue que existe um $r \in \mathbb{R}^+$ tal que $B_r(x) \subset \lbrace x \rbrace$. Perceba então que $B_r(x)$ é uma vizinhança de $x$ pois é um subconjunto de $M$ e além disso possui um subconjunto aberto (ele próprio) que contém $x$, entretanto, $|B_r(x)| = 1$, o que é um absurdo, logo $x$ não é isolado.