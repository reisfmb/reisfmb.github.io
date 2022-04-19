---
weight: 226
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.2.6
description: Chap. 1 Exercise 2.2.6
date: 2022-04-18
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Open Sets
---
### Pergunta
Let $A$ be a finite open subset of a metric space $M$. Prove that every point in $A$ is an isolated point of $M$.

### Solução
Como $A$ é finito, então o analisaremos como $A = \lbrace a_1, a_1, a_2, \cdots, a_n\rbrace$.

Fixe $k \in \lbrace 1, \cdots, n \rbrace$ e tome $a_k \in A$. Segue que:

$$
\lbrace a_k \rbrace = A \cap (M \setminus (A \setminus \lbrace a_k \rbrace))
$$

Já sabemos que $A$ é aberto e que a interseção finita de abertos é aberta, logo resta mostrar que $(M \setminus (A \setminus \lbrace a_k \rbrace))$ é aberto.


O conjunto $(M \setminus (A \setminus \lbrace a_k \rbrace))$ é o mesmo que $X = M \setminus \lbrace a_1 \rbrace \setminus \lbrace a_2 \rbrace \setminus \cdots \setminus \lbrace a_n \rbrace \cup \lbrace a_k \rbrace$.

Mostraremos então que $X$ é aberto. Para isso, defina

$$
f(x) = \frac{1}{2} \min \bigg \lbrace D(x,a_i) \mid a_i \in A \setminus \lbrace a_k \rbrace \bigg \rbrace
$$

Seja então $x \in X$. Provaremos que $B_{f(x)}(x) \subset X$.

Por definição, $B_{f(x)}(x) = \lbrace y \in X \mid D(x,y) < f(x) \rbrace$. Perceba então que para que $B_{f(x)}(x) \subset X$ nenhum $a_i$ com $i \in \lbrace 1, 2, \cdots, n \rbrace \setminus \lbrace k \rbrace$ pode estar em $B_{f(x)}(x)$. Provaremos isso a seguir.

Suponha que exista $i \in \lbrace 1, 2, \cdots, n \rbrace \setminus \lbrace k \rbrace$ tal que $a_i \in B_{f(x)}(x)$. Logo $D(x,a_i) < f(x)$, o que é um absurdo, pois por definição $f(x) < D(x,a_i)$ para todo $i \in \lbrace 1, 2, \cdots, n \rbrace \setminus \lbrace k \rbrace$, logo $a_i \notin B_{f(x)}(x)$ o que implica que $B_{f(x)}(x) \subset X$, da onde segue que $X$ é aberto.
