---
weight: 225
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.2.5
description: Chap. 1 Exercise 2.2.5
date: 2022-04-18
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Open Sets
---
### Pergunta
Prove that in the metric space of all real numbers there are no isolated points.

### Solução
Suponha que $x \in \mathbb{R}$ seja um ponto isolado, ou seja, $\exists r \in \mathbb{R}^+$ tal que $B_r(x) \subset \lbrace x \rbrace$. Segue então que 

$$
D(x,y) \geq r \quad \text{ para todo } y \neq x
$$

Tome $z,y \in \mathbb{R}$ tais que $z \neq y \neq x$. Pela desigualdade triangular segue que

$$
\begin{align*}
D(x,z) &\leq D(x,y) + D(y,z) \newline
&\leq r + D(y,z) \newline
&\implies D(x,z) - D(y,z) \leq r \newline
&\implies \frac{D(x,z) - D(y,z)}{2} < r
\end{align*}
$$

ou seja, $\frac{D(x,z) - D(y,z)}{2} \in B_r(x)$, da onde segue que $B_r(x)$ não está contido em $\lbrace x \rbrace$. Absurdo, logo $x$ não pode ser ponto isolado.