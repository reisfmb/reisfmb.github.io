---
weight: 118
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.1.8
description: Chap. 1 Exercise 1.1.8
date: 2022-04-02
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Set Theory
  - Combinatorics
---
### Pergunta
Let A be a finite set. Prove that 
$\bigg| \lbrace x \mid x \subset A \rbrace \bigg| = 2^{|A|}$.

### Solução
Queremos provar que o conjunto dos conjuntos potência de $A$ tem cardinalidade igual a $2^{|A|}$.

Uma maneira bem interessante de se pensar nesse problema é perceber que para cada conjunto potência de $A$ existe uma sequência binária que o identifica. Vamos em busca de encontrar tais sequências.

Considere o caso $A=\lbrace a,b,c \rbrace$. Sabemos que devemos ter $2^{|A|} = 2^3 = 8$ conjuntos potência. Vamos identificá-los:

$$
\emptyset, \lbrace a \rbrace, \lbrace b \rbrace, \lbrace c \rbrace, \lbrace a,b \rbrace, \lbrace a,c \rbrace, \lbrace b,c \rbrace, \lbrace a,b,c \rbrace
$$

Podemos então fazer a seguinte correspondência um a um:
$$
\begin{align*}
    \emptyset &\longleftrightarrow (0,0,0) \newline 
    \lbrace a \rbrace &\longleftrightarrow (1,0,0) \newline
    \lbrace b \rbrace &\longleftrightarrow (0,1,0) \newline
    \lbrace c \rbrace &\longleftrightarrow (0,0,1) \newline
    \lbrace a,b \rbrace &\longleftrightarrow (1,1,0) \newline
    \lbrace a,c \rbrace &\longleftrightarrow (1,0,1) \newline
    \lbrace b,c \rbrace &\longleftrightarrow (0,1,1) \newline
    \lbrace a,b,c \rbrace &\longleftrightarrow (1,1,1) \newline
\end{align*}
$$

A construção de tal correspondência fica evidente pelo exemplo acima, e pode ser feita para qualquer conjunto finito desde que se mantenha uma ordem inicial dos elementos, o que sempre pode ser feito através de uma bijeção ordenadora dado que os conjuntos são finitos.

Além disso, o exemplo acima também deixa claro a seguinte igualdade combinatória:

$$
\sum_{k=0}^n {n \choose k}  = 2^n
$$

Dado que:
- ${n \choose 0}$ contabiliza o subconjunto $\emptyset$ ou a sequência $(0,0,0)$
- ${n \choose 1}$ contabiliza os subconjuntos de cardinalidade $1$ ou as sequências que contém somente um $1$
- ${n \choose 2}$ contabiliza os subconjuntos de cardinalidade $2$ ou as sequências que contém somente dois $1$
- &nbsp;$\vdots$
- ${n \choose n}$ contabiliza o subconjunto $A$ ou a sequência $(1,1,1)$
