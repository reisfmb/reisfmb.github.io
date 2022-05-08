---
weight: 210
author: Bruno Reis
title: (Probabilidade) Capítulo 2, exercício 2.10
description: Chap. 2 Exercise 2.10
date: 2022-05-03
categories:
  - Probabilidade
tags:
  - Probability
---
### Pergunta
Sejam $A$ e $B$ eventos tais que $P(A|B) = \frac{1}{4}$ e $P(B|A) = \frac{1}{2}$:

a) $A$ e $B$ podem ser independentes?

b) $A$ e $B$ são necessariamente independentes?

c) $A$ e $B$ podem ser disjuntos?

### Solução
#### a
Sim, basta que $P(A) = \frac{1}{4}$ e $P(B) = \frac{1}{4}$.

#### b
Não, basta tomar $P(A) = \frac{1}{8}$ e $P(B) = \frac{1}{4}$. Perceba que com isso temos que:

$$
P(A|B) = \frac{P(A \cap B)}{P(B)} = \frac{1}{4} \implies P(A \cap B) = \frac{P(B)}{4}\newline
P(B|A) = \frac{P(B \cap A)}{P(A)} = \frac{1}{2} \implies P(B \cap A) = \frac{P(A)}{2}\newline
$$

Segue que $P(A \cap B) = \frac{1}{16} \neq \frac{1}{32} = P(A)P(B)$.

#### c
Não, pois caso fossem, $P(A|B) = \frac{P(A\cap B)}{P(B)} = \frac{0}{P(B)} = 0 \neq \frac{1}{4}$
