---
weight: 149
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.9
description: Chap. 1 Exercise 1.4.9
date: 2022-04-04
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
  - Periodic function
---
### Pergunta
Let $f: A \rightarrow B$ be a given function

a) If $S$ and $T$ are subsets of $A$ with $S \subset T$, prove that $f(S) \subset f(T)$.

b) If $S$ and $T$ are subsets of $B$ with $S \subset T$, prove that $f^{-1}(S) \subset f^{-1}(T)$

c) Prove that $ff^{-1}$ is the identity on $P(B)$ if $f$ is onto and that $f^{-1}f$ is the identity on $P(A)$ if $f$ is one-to-one

### Solução

#### a
Seja $y \in f(S)$, logo, por definição, $\exists s \in S$ tal que $y = f(s)$. Como $s \in T$ segue que $y \in f(T)$.

#### b
Seja $x \in f^{-1}(S)$, logo, por definição, $f(x) \in S$. Como $S \subset T$ então $f(x) \in T$ logo $x \in f^{-1}(T)$.


#### c
Queremos mostrar que $ff^{-1}$ é a relação identidade no cartesiano $P(B) \times P(B)$, ou seja, que $f(f^{-1}(S)) = S$ para todo $S \subset B$.

Primeiro vamos mostrar que $f(f^{-1}(S)) \subset S$.

Seja $y \in f(f^{-1}(S))$ logo existe $x \in f^{-1}(S)$ tal que $f(x) = y$. Como $x \in f^{-1}(S)$ então $f(x) \in S$, ou seja, $y \in S$, logo $f(f^{-1}(S)) \subset S$.

Agora vamos mostrar que com $f$ sobrejetora, $S \subset f(f^{-1}(S))$. 

Seja $y \in S$. Como $f$ é sobrejetora, então existe $x \in A$ tal que $f(x) = y$. Como $y \in S$ segue que na verdade $x \in f^{-1}(S) \subset A$. Logo $y \in f(f^{-1}(S))$ e portanto $S \subset f(f^{-1}(S))$.

Conclusão: sob tais condições $f(f^{-1}(S)) = S$.