---
weight: 153
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.5.3
description: Chap. 1 Exercise 1.5.3
date: 2022-04-06
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Relation
---
### Pergunta
Let $\sim$ be an equivalence relation on $A$. For $a \in A$ define $S_a$ to be the set of all $b \in A$ with $a \sim b$. Prove that two $S_a$'s are either disjoint or identical. Prove that the distinct $S_a$'s form a partition of $A$ (they are called the equivalence classes of the relation).

### Solução
Considere $S_a, S_b$ como descrito no enunciado. 

Mostraremos primeiro que se $S_a = S_b$, então $S_a = S_b$, logo ou são idênticos ou são disjuntos.

Seja $x \in S_a \cap S_b$, logo $x \sim a$ e $x \sim b$, da onde segue que $a \sim b$.

Como $a \sim b$ então se $y \sim a$, por simetria, $y \sim b$, logo $S_a \subset S_b$.

Como $a \sim b \implies b \sim a$, o raciocínio acima conclui também que $S_b \subset S_a$.

Logo $S_a = S_b$.

Mostraremos agora que $A = \bigcup_{a \in A} S_a$.

Seja $x \in A$. Por reflexividade $x \sim x$, logo $x \in S_x$ e portanto $x \in \bigcup_{a \in A} S_a$.

Seja $x \in \bigcup_{a \in A} S_a$. Logo, para algum $j \in A$, $x \in S_j$, ou seja, $x \in A$.

Como foi mostrado anteriormente, ou os $S_a$'s são idênticos ou disjuntos... Basta então escolher um único representante para os que são idênticos, obtendo assim

$$
A = \dot\bigcup_{k \in S \subset A}S_k
$$