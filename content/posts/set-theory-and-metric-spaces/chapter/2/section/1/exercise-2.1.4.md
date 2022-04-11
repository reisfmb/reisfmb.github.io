---
weight: 214
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.1.4
description: Chap. 1 Exercise 2.1.4
date: 2022-04-10
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $M$ be a set with a real function $D$ satisfying $D(a,a) = 0$, $D(a,b) \neq 0$ for $a \neq b$, $D(a,b) + D(b,c) \geq D(c,a)$. Prove that $D$ makes $M$ a metric space.

### Solução
Perceba que

$$
\begin{align*}
D(a,b) + D(b,b) \geq D(b,a) &\implies D(a,b) \geq D(b,a) \newline
D(b,b) + D(b,a) \geq D(a,b) &\implies D(b,a) \geq D(a,b)
\end{align*}
$$

logo 

$$
D(a,b) = D(b,a)
$$

Além disso, segue que 

$$
D(c,b) + D(b,c) \geq D(c,c) \implies 2 D(b,c) \geq 0 \implies D(b,c) \geq 0
$$

Isso prova que $M$ é espaço métrico por $D$, dado que

- $D(a,a) = 0$, por definição de $D$
- $D(a,b) = D(b,a)$, como demonstrado acima
- $D(a,b) > 0$ se $a \neq b$, pois $D(a,b) \geq 0$ como demonstrado acima e $D(a,b) \neq 0$ por definição de $D$
- $D(a,c) \leq D(a,b) + D(b,c)$ por definição de $D$ e $D(a,b) = D(b,a)$ como demonstrado acima.
