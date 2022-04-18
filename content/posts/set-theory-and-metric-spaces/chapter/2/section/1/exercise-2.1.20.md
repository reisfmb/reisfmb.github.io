---
weight: 2120
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.1.20
description: Chap. 1 Exercise 2.1.20
date: 2022-04-17
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
a) Suppose that a metric space $A$ is a union $B \cup C$ of two subsets of finite diameter. Show that $A$ has a finite diameter.

b) Generalize part (a) to the union of a finite number of subesets.

c) Suppose that, in part (a), $B \cap C$ is nonempty. Prove that $\text{diam($A$) $\leq$ diam($B$) + diam($C$)}$

### Solução
Primeiramente defina $d_B,d_C \in \mathbb{R}$ como sendo o diâmetro dos espaços métricos $B$ e $C$ respectivamente.

#### a
Claramente se $a,b$ \in $B$ ou $a,b \in C$ então $D(a,b) \leq d_B + d_C$. Considere então $b \in B$ e $c \in C$ e fixe $x \in B$ e $y \in C$. Segue que $D(b,c) \leq D(b,x) + D(x,c) \leq D(b,x) + D(x,y) + D(y,c) \leq d_B + D(x,y) + d_c$. Como $D(x,y) \in \mathbb{R}$ segue que $D(b,c)$ para quaisquer $b,c \in B \cup C$ é um valor finito, logo o diâmetro será finito.

#### b
O caso base para a união de dois conjuntos está provado na letra (a). Considere então provado para $k$ conjuntos. Provaremos que vale para $k+1$ conjuntos. 

Seja $A = S_1 \cup S_2 \cup \cdots \cup S_k \cup S_{k+1}$. Defina $B$ como $S_1 \cup S_2 \cup \cdots \cup S_k$, logo $A = B \cup S_{k+1}$. Como $B$ por hipótese de indução tem diâmetro finito e $S_{k+1}$ também, segue pela letra (a) que $A$ também terá. 

Sendo assim, **o conjunto definido pela união finita de espaços métricos de diâmetros finitos terá diâmetro finito**.

#### c
Seja $x \in B \cap C$, logo para $b,c \in B \cup C$ tem-se

$$
D(b,c) \leq D(b,x) + D(x,c)
$$

Porém $D(b,x) \leq d_B$ e $D(x,c) \leq d_C$, logo

$$
D(b,c) \leq d_B + d_C
$$