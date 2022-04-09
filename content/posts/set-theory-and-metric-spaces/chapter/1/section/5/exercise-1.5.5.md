---
weight: 155
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.5.5
description: Chap. 1 Exercise 1.5.5
date: 2022-04-08
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Relation
---
### Pergunta
Let $f$ be a map of a set $A$ into itself. Call a subset $B$ of $A$ invariant if $f(B) \subset B$. (More carefully, we ought to say invariant relative to $f$.) Call an invariant set *indecomposable* if it cannot be expressed as a union of disjoint nonvoid invariant sets. Prove that $A$ has a unique expression as a disjoint union of indecomposable invariant sets. (Hint: Try to define an appropriate equivalence relation.)

### Solução
Considere os seguintes conjuntos para $S \subset A$:
$$
B_x = \bigcap \lbrace B \subset S \mid x \in B \text{ e $B$ é invariante} \rbrace \newline
I_S = \lbrace B_x | x \in S \rbrace
$$

#### $B_x$ não é vazio. 

Primeiro perceba que sempre existe um invariante não vazio que contém $x$, nomedamente $A$ pois $f(A) \subset A$.

Perceba então que nenhum outro invariante que entra nas intercessões de $B_x$ é vazio pois assume-se que $x \in B$.

Logo $\forall x \in A$, tem-se $B_x \neq \emptyset$.

#### $B_x$'s são disjuntos

$$
???
$$