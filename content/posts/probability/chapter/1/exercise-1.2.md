---
weight: 12
author: Bruno Reis
title: (Probabilidade) Capítulo 1, exercício 1.2
description: Chap. 1 Exercise 1.2
date: 2022-04-13
categories:
  - Probabilidade
tags:
  - Probability
---
### Pergunta
a) De um baralho comum (52 cartas) são retiradas, sem reposição, uma amostra de 5 cartas. Qual evento é mais provável, sair uma quadra (4 cartas com o mesmo número) ou um flush (5 cartas do mesmo naipe, sem formar uma sequência de 5 números consecutivos)?

b) Repita o exercício anterior, supondo agora um baralho com apenas as cartas 7, 8, 9, 10, J, Q, K e A (32 cartas).

### Solução

#### a

Quadra:

$$
\frac{{13 \choose 1} 48}{52 \choose 5} = 
\frac{13 \times 48}{\frac{52 \times 51 \times 50 \times 49 \times 48}{5!}} =
\frac{13 \times 48 \times 5!}{52 \times 51 \times 50 \times 49 \times 48} =
\frac{13 \times 5!}{52 \times 51 \times 50 \times 49} \approx 0.00024
$$

Flush:

$$
\frac{4 * (13 * 12 * 11 * 10 * 9 - (5! * 9))}{(52 * 51 * 50 * 49 * 48)}
\approx 0.00197
$$

Quadra < Flush

#### b

Quadra:

$$
\frac{{8 \choose 1} 28}{32 \choose 5} = 
\frac{8 \times 28}{\frac{32 \times 31 \times 30 \times 29 \times 28}{5!}} =
\frac{8 \times 28 \times 5!}{32 \times 31 \times 30 \times 29 \times 28} =
\frac{8 \times 5!}{32 \times 31 \times 30 \times 29} \approx 0.0011
$$

Flush:
$$
\frac{4 * (8 * 7 * 6 * 5 * 4 - (5! * 4))}{(32 * 31 * 30 * 39 * 38)}
\approx 0.000566
$$

Flush < Quadra
