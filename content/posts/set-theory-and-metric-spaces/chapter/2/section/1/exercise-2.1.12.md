---
weight: 2112
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.1.12
description: Chap. 1 Exercise 2.1.12
date: 2022-04-10
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $M$ be the metric space of all real numbers, and let $x_0 \in M$. Prove that there exist exactly two isometries of $M$ that leave $x_0$ fixed.

### Solução
Seja $f$ uma isometria tal que $f(x_0) = x_0$. Como $f$ é isometria para qualquer métrica $D$, em particular $f$ é isometria na métrica $D(x,y) = |x - y|$, ou seja $|x - y| = |f(x) - f(y)|$, e tomando $y = x_0$ tem-se:

$$
|f(x) - x_0| = |x - x_0| 
$$

da onde segue que $f(x) = x$ ou $f(x) = 2x_0 - x$.
