---
weight: 303
author: Bruno Reis
title: (Probabilidade) Capítulo 3, exercício 3.3
description: Chap. 3 Exercise 3.3
date: 2022-05-03
categories:
  - Probabilidade
tags:
  - Probability
---
### Pergunta
Sejam $X, Y, Z$ e $W$ variáveis aleatórias onde $X$ é uma variável qualquer, $Y = \max\lbrace 0,X \rbrace$, $Z = \max \lbrace 0, -X \rbrace$ e $W = |X|$. Escreva funções de distribuição $F_Y, F_Z$ e $F_W$ em termos da função de distribuição $F_X$.

### Solução
$$
\begin{align*}
F_X(t) &= P(\lbrace X \leq t \rbrace) \newline
F_Y(t) &= P(\lbrace 0 \leq X \leq t \rbrace) \newline
F_Z(t) &= P(\lbrace -t \leq X \leq 0 \rbrace) \newline
F_W(t) &= P(\lbrace -t \leq X \leq t \rbrace)
\end{align*}
$$