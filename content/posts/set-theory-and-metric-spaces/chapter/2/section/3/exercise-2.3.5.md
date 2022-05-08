---
weight: 235
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.3.5
description: Chap. 1 Exercise 2.3.5
date: 2022-04-26
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Limit Point
---
### Pergunta
Let $A$ be a subset and $x$ a point in a metric space. Prove that $x$ is a limit point of $A$ if and only if there exist a sequence $\lbrace x_i \rbrace$ of elements of $A$ converging to $x$, with all $x_i \neq x$. Prove further that the $x_i$'s can be selected so that the numbers $D(x_i,x)$ decrease strictly monotonically, i.e.,
$$
D(x_1,x) > D(x_2,x) > D(x_3,x) > \cdots
$$

### Solução
Suponha que $x$ seja um ponto limite de $A$, ou seja, $x \in \overline{A \setminus \lbrace x \rbrace}$, isto é, $x$ pertence a todos os fechados que contém $A \setminus \lbrace x \rbrace$.
