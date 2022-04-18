---
weight: 2111
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.1.11
description: Chap. 1 Exercise 2.1.11
date: 2022-04-17
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $D_1$ and $D_2$ be metrics on a single space $M$. Which of the following are metrics on $M$: $D_1 + D_2$, $\max(D_1,D_2)$, $\min(D_1,D_2)$?

### Solução

#### $D_1 + D_2$ é métrica em $M$
$(D_1 + D_2)(a,a) = D_1(a,a) + D_2(a,a) = 0 + 0 = 0$

$(D_1 + D_2)(a,b) = D_1(a,b) + D_2(a,b) > 0$

$(D_1 + D_2)(a,b) = D_1(a,b) + D_2(a,b) = D_1(b,a) + D_2(b,a) = (D_1 + D_2)(b,a)$

$$
\begin{align*}
(D_1 + D_2)(a,c) &= D_1(a,c) + D_2(a,c) \newline
&\leq (D_1(a,b) + D_1(b,c)) + (D_2(a,b) + D_2(b,c)) \newline
&= (D_1(a,b) + D_2(a,b)) + (D_1(b,c) + D_2(b,c)) \newline
&= (D_1 + D_2)(a,b) + (D_1 + D_2)(b,c)
\end{align*}
$$

Logo é métrica em $M$.

---

#### $\max(D_1,D_2)$ é metrica em $M$

$\max(D_1,D_2)(a,a) = \max(D_1(a,a),D_2(a,a)) = \max(0,0) = 0$

$\max(D_1,D_2)(a,b) = \max(D_1(a,b),D_2(a,b)) > 0$

$\max(D_1,D_2)(a,b) = \max(D_1(a,b),D_2(a,b)) = \max(D_1(b,a),D_2(b,a)) = \max(D_1,D_2)(b,a)$

Para provar a desigualdade triangular, relembre que:

$$
D_1(a,c) \leq D_1(a,b) + D_1(b,c) \newline
D_2(a,c) \leq D_2(a,b) + D_2(b,c)
$$

logo

$$
\max(D_1(a,c),D_2(a,c)) = D_1(a,b) + D_1(b,c)
$$

ou 

$$
\max(D_1(a,c),D_2(a,c)) = D_2(a,b) + D_2(b,c)
$$

e como temos que $D_1(a,b) \leq \max(D_1,D_2)(a,b)$ e $D_2(a,b) \leq \max(D_1,D_2)(a,b)$ para todo $a,b \in M$, segue que

$$
\max(D_1,D_2)(a,c) \leq \max(D_1,D_2)(a,b) + \max(D_1,D_2)(b,c)
$$

---

#### $\max(D_1,D_2)$ não é metrica em $M$

$\min(D_1,D_2)(a,a) = \min(D_1(a,a),D_2(a,a)) = \min(0,0) = 0$

$\min(D_1,D_2)(a,b) = \min(D_1(a,b),D_2(a,b)) > 0$

$\min(D_1,D_2)(a,b) = \min(D_1(a,b),D_2(a,b)) = \min(D_1(b,a),D_2(b,a)) = \min(D_1,D_2)(b,a)$

E claramente existem contra exemplos para o caso da desigualdade triangular considerando o mínimo como métrica.