---
weight: 2318
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.3.18
description: Chap. 1 Exercise 2.3.18
date: 2022-04-30
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $\lbrace x_i \rbrace$ be a sequence of distinct elements in a metric space, and suppose that $x_i \rightarrow x$. Let $f$ be a one-to-one map of the set of $x_i$'s into itself. Prove that $f(x_i) \rightarrow x$.

### Solução
Suponha que $f(x_i)$ não converta para $x$, ou seja, $\exists \epsilon_0 \in \mathbb{R}^+$ tal que para todo $N \in \mathbb{Z}^+$ vai existir $i > N$ tal que $D(f(x_i),x) \geq \epsilon_0$.

Do fato que $\lbrace x_i \rbrace \rightarrow x$ segue que $\exists N_{\epsilon_0}$ tal que $D(x_i,x) < \epsilon_0$ para todo $i > N_{\epsilon_0}$.

Suponha então que $f(x_i) = x_j$ e tome $N$ tal que $j > N_{\epsilon_0}$. 

Da negação de $f(x_i) \rightarrow x$ segue que $\exists i > N$, tal que

$$
D(f(x_i),x) = D(x_j,x) \geq \epsilon_0
$$

E como $j > N_{\epsilon_0}$, isso implica que $\lbrace x_i \rbrace$ não converte para $x$. Absurdo, logo $f(x_i) \rightarrow x$.
