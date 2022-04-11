---
weight: 211
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.1.1
description: Chap. 1 Exercise 2.1.1
date: 2022-04-09
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
---
### Pergunta
Let $M$ be a set with two numbers $a$ and $b$. Define $D(a,a) = D(b,b) = 0$ and $D(a,b) = D(b,a) = r$, where $r$ is a positive real number. Prove that $M$ is a metric space relative to the function $D$.

### Solução
Basta verificar se $D$ satisfaz as 4 propriedades que definem, junto de $M$, um espaço métrico:

#### 1) $D(x,x) = 0$ para todo $x \in M$
Verdade pois $M = \lbrace a,b \rbrace$ e $D(a,a) = D(b,b) = 0$.

#### 2) $D(x,y) > 0$ se $x \neq y$
Verdade pois $D(a,b) = D(b,a) = r > 0$.

#### 3) $D(x,y) = D(y,x)$ para todo $x,y \in M$
Verdade pois $D$ foi definida dessa forma... $D(a,b) = D(b,a) = r$.

#### 4) $D(x,z) \leq D(x,y) + D(y,z)$ (desigualdade triangular)
Verdade pois $D(a,b) \leq D(a,b) + D(b,a) = 2D(a,b)$.