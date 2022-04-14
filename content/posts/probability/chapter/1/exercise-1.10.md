---
weight: 110
author: Bruno Reis
title: (Probabilidade) Capítulo 1, exercício 1.10
description: Chap. 1 Exercise 1.10
date: 2022-04-13
categories:
  - Probabilidade
tags:
  - Probability
  - Stars and bars
---
### Pergunta
No final da Seção 1.1.3, observamos que há 21 resultados possíveis no lançamento simultâneo de dois dados idênticos, correspondendo aos 21 pares não-ordenados de números entre 1 e 6. Um jogo de dominó para crianças, em que cada metade de peça pode ser pintada com uma de 7 cores do arco-íris, possui 28 peças, correspondendo aos 28 pares não-ordenados de cores do arco-íris. De forma mais geral, o número de pares não-ordenados de um conjunto com $n$ elementos é ${n+1 \choose 2}$. Prove este fato de quatro formas diferentes:

a) Por indução em n e usando propriedades do Triângulo de Pascal.

b) Decompondo a família de pares não-ordenados em pares de elementos distintos e pares de elementos iguais.

c) Descrevendo uma correspondência direta entre pares não-ordenados de {1, . . . , n} e subconjuntos de {*, 1, . . . , n} com dois elementos, de forma que o novo elemento * cumpra um papel especial.

d) Descrevendo uma correspondência direta entre pares não-ordenados de {1, . . . , n} e palavras compostas por n − 1 símbolos |” e 2 de seus símbolos “·”.

### Solução
Primeiro perceba que 
$$
{n+1 \choose 2} = \frac{(n+1)!}{2!(n-1)!} = \frac{(n+1)n(n-1)!}{2(n-1)!} = \frac{n^2+n}{2}
$$

#### a
Boring.

#### b
Seja $S$ um conjunto com $n$ elementos e vamos considerar todos os possíveis pares não ordenados.

Primeiramente perceba que existem $n$ pares não ordenados de elementos iguais. 

Para calcular os demais, basta contar os elementos da parte superior à diagonal principal de $S^2$, que possuirá $\frac{n^2 - n}{2}$ elementos.

Assim sendo, tem-se:
$$
n + \frac{n^2 - n}{2} = \frac{n^2+n}{2} = {n+1 \choose 2}
$$

#### c
Seja $PNO_n$ o conjunto de pares não ordenados de $\lbrace 1, \cdots, n \rbrace$.

Considere então as entradas de $PNO_n$ com elementos iguais e tome o seguinte mapeamento

$$
\lbrace i \rbrace \mapsto \lbrace *, i \rbrace
$$

Já para as anetradas de $PNO_n$ com elementos distintos, tome o seguinte mapeamento

$$
\lbrace i, j \rbrace \mapsto \lbrace i, j \rbrace
$$

Defina então $f:PNO_n \rightarrow \text{subconjuntos de $\lbrace *, 1, \cdots, n \rbrace$ com $2$ elementos}$ com os mapeamentos acima. Como evidentemente $f$ é bijeção, segue que:

$$
|PNO_n| = |\text{subconjuntos de $\lbrace *, 1, \cdots, n \rbrace$ com $2$ elementos}| = {n+1 \choose 2}
$$

#### d
É mais facil descrever um caso específico do que escrever uma demonstração formal de tal fato.

Com tal finalidade, considere $\lbrace 1,2,3 \rbrace$ e vamos considerar todos os pares não ordenados de tal conjunto:

- $\lbrace 1 \rbrace$
- $\lbrace 1,2 \rbrace$
- $\lbrace 1,3 \rbrace$
- $\lbrace 2 \rbrace$
- $\lbrace 2,3 \rbrace$
- $\lbrace 3 \rbrace$

Perceba que as palavas associadas utilizando os símbolos solicitados são respectivamente
- ..||
- .|.|
- .||.
- |..|
- .|.|.
- ||..