---
weight: 3
author: Bruno Reis
title: Complete metric space equivalence
description: Equivalence of the statement that a set is a complete metric space
date: 2022-05-08
categories:
  - Articles
tags:
  - Metric Spaces
---
### Theorem
For a metric space $M$ the following two statements are equivalent:

a) $M$ is complete.

b) For any descending sequence $A_1 \supset A_2 \supset A_3 \supset \cdots$ of nonempty closed sets with diameters approaching $0$, the intersection $\cap A_i$ is nonempty.

### $a \implies b$
Como cada $A_i$ é não vazio, tome $x_i \in A_i$ e considere a sequência formada por tais elementos. Mostraremos que tal sequência é de Cauchy. 

Seja $\epsilon > 0$. Como $\big\lbrace \text{diam}(A_n)\big\rbrace \rightarrow 0$ então existe $N$ tal que $\text{diam}(A_N) < \epsilon$, ou seja, para todo $i,j > N$ segue que $D(x_i,x_j) < \text{diam}(A_N) < \epsilon$, logo $\lbrace x_n \rbrace$ é de Cauchy. Como o espaço métrico $M$ é completo então essa sequência converge para um $x \in M$. Mostraremos que $x \in \cap A_i$.

Pelo fato que $A_1 \supset A_2 \supset A_3 \supset \cdots$ temos:

- $\lbrace x_n \rbrace \in A_1$
- $\lbrace x_n \rbrace \setminus \lbrace x_1 \rbrace \in A_2$
- $\lbrace x_n \rbrace \setminus \lbrace x_1,x_2 \rbrace \in A_3$
- $\cdots$

Como $\lbrace x_n \rbrace \rightarrow x$, toda subsequência convergente de uma sequência convergente converge pro mesmo limite e $A_i$ é fechado, então segue que $x \in A_i$ para todo $i$, logo $x \in \cap A_i$.

### $b \implies a$
Seja $\lbrace x_n \rbrace$ uma sequência de Cauchy em $M$. Mostraremos que tal sequência converge em $M$, o que por definição implica que $M$ é completo.

Defina a seguinte família de conjuntos $B_i = \lbrace x_j \mid j \geq i \rbrace$. Segue que $B_1 \supset B_2 \supset B_3 \supset \cdots$. Mostraremos que $\big\lbrace \text{diam}(B_i) \big\rbrace \rightarrow 0$. Seja $\epsilon > 0$. Como $\lbrace x_n \rbrace$ é de Cauchy, segue que existe $N$ tal que $\forall i,j > N$ tem-se $D(x_i,x_j) < \epsilon$, ou seja, $\text{diam}(B_{N+1}) < \epsilon$, logo $\big\lbrace \text{diam}(B_i) \big\rbrace \rightarrow 0$.

Defina os seguintes conjuntos $A_i = \overline{B_i}$. Claramente $A_1 \supset A_2 \supset A_3 \supset \cdots$ e $\big\lbrace \text{diam}(A_i) \big\rbrace \rightarrow 0$ uma vez que $\text{diam}(B_i) = \text{diam}(\overline{B_i}) = \text{diam}(A_i)$ (veja a [demonstração](../../set-theory-and-metric-spaces/chapter/2/section/3/exercise-2.3.8) desse fato).

Assim sendo, os $A_i$'s são fechados, não vazios, formam uma cadeia descendente e portanto tem intercessão não vazia, i.e, $x \in \cap A_i$. Mostraremos que $x$ é o ponto a qual a sequência de Cauchy converge.

Seja $\epsilon > 0$. Como $\big\lbrace \text{diam}(A_i) \big\rbrace \rightarrow 0$ segue que existe $N$ tal que $\text{diam}(A_N) < \epsilon$. Como $x \in \cap A_i$ então para todo $n > N$ tem-se

$$
D(x_n,x) \leq \text{diam}(A_N) < \epsilon
$$

logo $\lbrace x_n \rbrace \rightarrow x$. Como todos os $A_i$'s são subconjuntos de $M$, segue que $x \in M$ e portanto $M$ é fechado. $\blacksquare$