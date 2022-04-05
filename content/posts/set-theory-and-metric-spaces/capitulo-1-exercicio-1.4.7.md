---
weight: 147
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.7
description: Chap. 1 Exercise 1.4.7
date: 2022-04-04
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
  - Periodic function
---
### Pergunta
Given a function $f: A \rightarrow A$, we write $f^n$ for the function on $A$ obtained by taking the composite of $f$ with itself $n$ times. Suppose that $f^n$ equals the identity function for some $n$ (one says that $f$ is periodic). Prove that $f$ is one-to-one and onto.

### Solução
Sejam $y \in A$. Em busca de sobrejetividade, vamos mostrar que existe $x \in A$ tal que $f(x) = y$.

- Se $n = 1$, então basta tomar $x = y$.
- Se $n > 1$, então basta tomar $x = f^{n - 1}(y)$, pois então $f(x) = y$.

Seja $a,b \in A$ tais que $f(a) = f(b)$. Em busca de injetividade, vamos mostrar que $a = b$. 

- Se $n = 1$, então é imediato, pois $f(a)=f(b) \implies a = b$.
- Se $n > 1$, então $f(a) = f(b) \implies (f^{n-1}f)(a) = (f^{n-1}f)(b) \implies a = b$.