---
weight: 152
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.5.2
description: Chap. 1 Exercise 1.5.2
date: 2022-04-06
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Relation
---
### Pergunta
Suppose that on a set $A$ there is a given partition: an expression of $A$ as union of disjoint subets. For $a,b \in A$, define $a \sim b$ to mean $a$ and $b$ lie in the same subset. Prove that this defines an equivalence relation.

### Solução
$$
A = \dot\bigcup_{i \in I} S_i \quad \text{ tal que } \quad \forall i \in I, S_i \subset A
$$

#### Reflexividade
$a \sim a$ para todo $a \in A$ pois $a$ sempre estará no mesmo subconjunto $S_i$ de $A$.

#### Simetria
Se $a \sim b$ então $a,b \in S_j$, logo $b \sim a$.

#### Transitividade
Se $a \sim b$ e $b \sim c$ então $a,b \in S_j$ e $b,c \in S_k$. Como $S_j$ e $S_k$ são disjuntos, então $k=j$ e portanto $a,b,c \in S_j$ logo $a \sim c$.
