---
weight: 1418
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.18
description: Chap. 1 Exercise 1.4.18
date: 2022-04-05
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
---
### Pergunta

a) Let $x_0$ be a fixed element in a set $X$. Let $f: X \rightarrow X$ be defined by $f(x) = x_0$ for all $x$. Prove that $fg = f$ for all $g: X \rightarrow X$.

b) Conversely assume that $f: X \rightarrow X$ satisfies $fg = f$ for all $g: X \rightarrow X$. Prove that, for a suitable $x_0$, $f$ is the map of part (a).

### Solução

#### a
$$
(fg)(x) = f(\underbrace{g(x)}_{\in X})= x_0 = f(x)
$$

#### b
Suponha $f$ não constante. Logo existem $(a,b) \in X^2$ tal que $f(a) \neq f(b)$. Perceba então que para toda $g:X \rightarrow X$ tal que $g(a) = b$ tem-se $fg(a) = f(b) \neq f(a)$. Absurdo, logo $f$ é constante.