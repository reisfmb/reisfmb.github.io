---
weight: 15
author: Bruno Reis
title: (Probabilidade) Capítulo 1, exercício 1.5
description: Chap. 1 Exercise 1.5
date: 2022-04-13
categories:
  - Probabilidade
tags:
  - Probability
---
### Pergunta
Mostre o Teorema das Colunas do Triângulo de Pascal: para todos n e k inteiros não-negativos,
$\sum_{j=0}^k {n+j \choose n} = {k+n+1 \choose n+1}$. *Dica: Mostre por indução em k para todo n.*

### Solução
Fixe n inteiro não negativo e seja $k = 1$, logo

$$
{n \choose n} + {n+1 \choose n} = 1 + {n+1 \choose n}
$$

Pela relação de Stifel, segue que

$$
{n+2 \choose n+1} = {n+1 \choose n} + {n+1 \choose n+1} = 1 + {n+1 \choose n}
$$

Logo, para $k = 1$ está provado que $\sum_{j=0}^k {n+j \choose n} = {k+n+1 \choose n+1}$.

Suponha então que a relação esteja demonstrada para $k$. Mostraremos que é válida para $k+1$.

$$
\sum_{j=0}^{k+1} {n+j \choose n} = \sum_{j=0}^k {n+j \choose n} + {k+n+1 \choose n}
$$

Porém, pela H.I, segue que 

$$
\sum_{j=0}^k {n+j \choose n} = {k+n+1 \choose n+1}
$$

logo

$$
\sum_{j=0}^{k+1} {n+j \choose n} = {k+n+1 \choose n+1} + {k+n+1 \choose n}
$$

porém, pela relação de Stifel

$$
{k+n+1 \choose n+1} + {k+n+1 \choose n} = {k+n+2 \choose n+1}
$$

portanto

$$
\sum_{j=0}^{k+1} {n+j \choose n} = {k+n+2 \choose n+1}
$$