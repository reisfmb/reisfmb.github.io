---
weight: 1410
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.10
description: Chap. 1 Exercise 1.4.10
date: 2022-04-05
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
---
### Pergunta
Given a function $f: A \rightarrow B$, subsets $S_1, S_2$ of $A$ and subsets $T_1, T_2$ of $B$, prove the following:

a) $f(S_1 \cup S_2) = f(S_1) \cup f(S_2)$

b) $f^{-1}(T_1 \cup T_2) = f^{-1}(T_1) \cup f^{-1}(T_2)$

c) $f(S_1 \cap S_2) \subset f(S_1) \cap f(S_2)$

d) $f^{-1}(T_1 \cap T_2) = f^{-1}(T_1) \cap f^{-1}(T_2)$

In part (c) show that equality holds for all $S_1$ and $S_2$ if and only if $f$ is one-to-one.

### Solução

#### a
Seja $y \in f(S_1 \cup S_2)$, logo existe $x \in S_1 \cup S_2$ tal que $f(x) = y$. Como $x \in S_1$ então $y \in f(S_1) \subset (S_1) \cup f(S_2)$.

Seja $y \in f(S_1) \cup f(S_2)$, logo $y \in f(S_1)$ ou $y \in f(S_2)$. Se $y \in f(S_1)$ então existe $x \in S_1 \subset S_1 \cup S_2$ tal que $f(x) = y$, logo $y \in f(S_1 \cup S_2)$. Similarmente para $y \in f(S_2)$. Logo $y \in f(S_1 \cup S_2)$.

#### b
Seja $x \in f^{-1}(T_1 \cup T_2)$, logo $f(x) \in T_1 \cup T_2$, ou seja $f(x) \in T_1$ ou $f(x) \in T_2$. Se $f(x) \in T_1$ então $x \in f^{-1}(T_1) \subset f^{-1}(T_1) \cup f^{-1}(T_2)$. Se $f(x) \in T_2$ então $x \in f^{-1}(T_2) \subset f^{-1}(T_1) \cup f^{-1}(T_2)$. Logo $x \in f^{-1}(T_1) \cup f^{-1}(T_2)$.

Seja $x \in f^{-1}(T_1) \cup f^{-1}(T_2)$, logo $x \in f^{-1}(T_1)$ ou $x \in f^{-1}(T_2)$. se $x \in f^{-1}(T_1)$ então $f(x) \in T_1 \subset T_1 \cup T_2$, ou seja $x \in f^{-1}(T_1 \cup T_2)$. Similarmente para $x \in f^{-1}(T_2)$. Logo $x \in f^{-1}(T_1 \cup T_2)$.

#### c
Seja $y \in f(S_1 \cap S_2)$, logo existe $x \in S_1 \cap S_2$ tal que $f(x) = y$. Como $x \in S_1$ então $y \in f(S_1)$. Como $x \in S_2$ então $y \in f(S_2)$, logo $y \in f(S_1) \cap f(S_2)$.

Suponha então que $f$ seja injetora. Mostraremos que $f(S_1) \cap f(S_2) \subset f(S_1 \cap S_2)$.

Seja $y \in f(S_1) \cap f(S_2)$, logo $y \in f(S_1)$ e $y \in f(S_2)$, ou seja, existe $x_1 \in S_1$ e $x_2 \in S_2$ tais que $f(x_1) = y$ e $f(x_2) = y$. Como $f$ é injetora, então $f(x_1) = y = f(x_2) \implies x_1 = x_2 \in S_1 \cap S_2$. Logo $y \in f(S_1 \cap S_2)$.

#### d
Seja $x \in f^{-1}(T_1 \cap T_2)$, logo $f(x) \in T_1 \cap T_2$, ou seja, $f(x) \in T_1$ e $f(x) \in T_2$. Como $f(x) \in T_1$ segue que $x \in f^{-1}(T_1)$. Similarmente $x \in f^{-1}(T_2)$, logo $x \in f^{-1}(T_1) \cap f^{-1}(T_2)$.

Seja $x \in f^{-1}(T_1) \cap f^{-1}(T_2)$, logo $x \in f^{-1}(T_1)$ e $x \in f^{-1}(T_2)$. Como $x \in f^{-1}(T_1)$ então $f(x) \in T_1$. Como $x \in f^{-1}(T_2)$ então $f(x) \in T_2$.
Logo $f(x) \in T_1 \cap T_2$, ou seja, $x \in f^{-1}(T_1 \cap T_2)$.

