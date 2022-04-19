---
weight: 221
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.2.1
description: Chap. 1 Exercise 2.2.1
date: 2022-04-18
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Open Sets
---
### Pergunta
a) Prove that in any metric space the complement of a point is open.

b) Prove that any set in a metric space is an intersection of open sets.

### Solução

#### a
Seja $p \in M$ e considere $U = M \setminus \lbrace p \rbrace$. Provaremos que $U$ é aberto, ou seja, para todo $x \in U$ existe $B_r(x) \subset U$ onde $B_r(x) = \lbrace m \mid m \in M \text{ e } D(x,m) < r \rbrace$. Repare então que se tomarmos $r = D(x,p)$ então segue que $p \notin B_r(x)$ pois $D(x,p) = D(x,p)$ e não estritamente menor, logo $B_{D(x,p)}(x) \subset U$.

#### b
Seja $U \subset M$. Pela letra (a) fica evidente a seguinte construção:

$$
U = \bigcap_{u \in U^c} M \setminus \lbrace u \rbrace
$$