---
weight: 215
author: Bruno Reis
title: (Probabilidade) Capítulo 2, exercício 2.15
description: Chap. 2 Exercise 2.15
date: 2022-05-03
categories:
  - Probabilidade
tags:
  - Probability
---
### Pergunta
Sejam $A$ e $(B_n)_n$ eventos tais que $A$ e $B_n$ são independentes para todo $n$. Mostre que, se os eventos $(B_n)_n$ são dois a dois disjuntos, então $A$ e $\cup_n B_n$ são independentes. Exiba um exemplo ilustrando que a hipótese de que os $(B_n)_n$ são disjuntos não pode ser omitida.

### Solução
$$
\begin{align*}
P(A \cap (\cup_n B_n)) &= P(\cup_n (A \cap B_n)) \newline
&=\sum_n P(A \cap B_n) \newline
&=\sum_n P(A)P(B_n) \newline
&=P(A) \sum_n P(B_n) \newline
&=P(A)P(\cup_n B_n)
\end{align*}
$$

Pensar no exemplo...