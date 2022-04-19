---
weight: 224
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.2.4
description: Chap. 1 Exercise 2.2.4
date: 2022-04-18
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Open Sets
---
### Pergunta
Prove que o exemplo 4 na seção 4.1 é discreto.

### Solução
O exemplo 4 diz o seguinte:

Seja $M$ qualquer conjunto e defina $D(a,a) = 0$ e $D(a,b) = 1$ para $a \neq b$ em $M$.

Vamos provar que tal conjunto é discreto, o que é equivalente a provar que todo ponto é isolado, ou seja, que todo $\lbrace x \rbrace \subset M$ é aberto.

Seja $x \in M$ e $B_r(x) = \lbrace m \in M \mid D(x,m) < r\rbrace$. 

Perceba que se definirmos $r = \frac{1}{2}$ então teremos $B_{\frac{1}{2}}(x) = \left\lbrace m \in M \mid D(x,m) < \frac{1}{2} \right\rbrace$, tal que $B_{\frac{1}{2}}(x) \subset \lbrace x \rbrace$, logo $\lbrace x \rbrace$ é aberto.