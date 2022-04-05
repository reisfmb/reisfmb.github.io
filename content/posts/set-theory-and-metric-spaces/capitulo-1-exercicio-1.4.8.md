---
weight: 148
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.8
description: Chap. 1 Exercise 1.4.8
date: 2022-04-04
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
  - Periodic function
---
### Pergunta
As a generalization of periodic functions [see the preceding exercise](/posts/set-theory-and-metric-spaces/capitulo-1-exercicio-1.4.7/) we say that $f: A \rightarrow A$ is locally periodic if for every $x \in A$ there exists a positive integer $n(x)$, depending on $x$, such that $f^{n(x)}(x) = x$. Prove that a locally periodic function is one-to-one and onto

### Solução
Sejam $y \in A$. Em busca de sobrejetividade, vamos mostrar que existe $x \in A$ tal que $f(x) = y$.

Como $y \in A$, existe um inteiro $n(y)$ tal que $f^{n(y)}(y) = y$.
- Se $n(y) = 1$, então basta tomar $x = y$.
- Se $n(y) > 1$, então basta tomar $x = f^{n(y) - 1}(y)$, pois então $f(x) = y$.

Seja $a,b \in A$ tais que $f(a) = f(b)$. Em busca de injetividade, vamos mostrar que $a = b$. 

- Se $n(a) = n(b) = 1$, então segue diretamente que $a = b.
- Se $n(a) = n(b)$ e $n(a),n(b) > 1$, então segue diretamente que $a = b$ pois $(f^{n(a) - 1}f)(a) = (f^{n(b)-1}f)(b) \implies a = b$.
- Se $n(a) > n(b)$ e $n(a),n(b) > 1$, então

$$
\begin{align*}
  f(a) = f(b) & \implies (f^{n(a)n(b) - 1}f)(a) = (f^{n(a)n(b) - 1}f)(b) \newline
    & \implies (f^{n(a)n(b)})(a) = (f^{n(a)n(b)})(b) \newline
    & \implies a = b
\end{align*}
$$

Para ver a última passagem, basta perceber que

$
(f^{n(a)n(b)})(a) =
$

$
\underbrace{(f^{n(a)} \circ f^{n(a)} \circ \cdots \circ f^{n(a)})}_{n(b)\text{ vezes}}(a) = \newline
$

$
\underbrace{(f^{n(a)} \circ f^{n(a)} \circ \cdots \circ f^{n(a)})}_{n(b) - 1\text{ vezes}}\circ f^{n(a)}(a) 
$

$
\underbrace{(f^{n(a)} \circ f^{n(a)} \circ \cdots \circ f^{n(a)})}_{n(b) - 2\text{ vezes}}\circ f^{n(a)}(a) 
$

$
\vdots
$
