---
weight: 111
author: Bruno Reis
title: (Probabilidade) Capítulo 1, exercício 1.11
description: Chap. 1 Exercise 1.11
date: 2022-04-13
categories:
  - Probabilidade
tags:
  - Probability
  - Stars and bars
---
### Pergunta
Inspirado pelo exercício anterior, mostre que o número de soluções inteiras não-negativas da equação $x_1 + \cdots + x_n = k$ é dada por ${n - 1 + k \choose k}$

### Solução
Cada solução pode ser identificada como uma sequência de símbolos que contém $n-1$ barras "|" e $k$ pontos ".". Exemplo de algumas soluções para $n = 3$ e $k = 10$:

- ..|......|.. $x_1 = 2, x_2 = 6, x_3 = 2$
- |.|........ $x_1 = 0, x_2 = 1, x_3 = 9$
- ....|..|.... $x_1 = 4, x_2 = 2, x_3 = 4$

Perceba então que para identificar cada palavra, basta que se defina as posições das $n-1$ barras dentre as $n - 1 + k$ possíveis posições e complete o restante com ".".

Por exemplo, a primeira solução exemplificada acima é definida por uma barra na posição $3$ e outra na posição $10$. Já a segunda solução é definida por uma barra na posição $1$ e outra barra na posição $3$.

Assim sendo, para contabilizar todas as soluções, basta que sejam escolhidas $n - 1$ das $n - 1 + k$ posições, ou seja:

$$
{n - 1 + k \choose n-1} = {n - 1 + k \choose k}
$$
