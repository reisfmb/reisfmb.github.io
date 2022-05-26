---
weight: 1
author: Bruno Reis
title: R is complete
description: Full proof for completeness of R
date: 2022-05-08
categories:
  - Articles
tags:
  - Metric Spaces
---
### Lema 1
Seja $M$ um espaço métrico e $\lbrace x_n \rbrace \subset M$ uma sequência de Cauchy. Se existe uma subsequência dessa sequência tal que a subsequência converge para $x \in M$ então $\lbrace x_n \rbrace \rightarrow x$.

Seja $\lbrace x_{n_k} \rbrace$ uma subsequência de $\lbrace x_n \rbrace$ tal que $\lbrace x_{n_k} \rbrace \rightarrow x$. Mostraremos que $\lbrace x_n \rbrace \rightarrow x$.

Seja $\epsilon_1 > 0$. Pela convergência da subsequência, existe $N_1$ tal que para todo $k > N_1$ tem-se $D(x_{n_k},x) < \epsilon_1$.

Perceba então que 
$$
D(x_n,x) \leq D(x_n,x_{n_k}) + D(x_{n_k},x) < D(x_n,x_{n_k}) < \epsilon_1
$$

Porém $\lbrace x_n \rbrace$ é de Cauchy, logo para $\epsilon_2 > 0$ existe $N_2$ tal que para todo $n,m > N_2$ tem-se $D(x_n,x_m) < \epsilon_2$.

Tome então $\epsilon > 0$, $\epsilon_1 = \frac{\epsilon}{2}$, $\epsilon_2 = \frac{\epsilon}{2}$ e $N = \max(N_1,N_2)$. Segue então que para $n,n_k > N$ tem-se
$$
D(x_n,x) \leq D(x_n,x_{n_k}) + D(x_{n_k},x) < \frac{\epsilon}{2} + \frac{\epsilon}{2} < \epsilon
$$

Logo $\lbrace x_n \rbrace \rightarrow x$. $\blacksquare$


### Lema 2
Seja $\lbrace x_n \rbrace$ uma seuqência de Cauchy em $\mathbb{R}$. Segue então que $\lbrace x_n \rbrace$ é limitada.

Fixe $r_1 > 0$. Como a sequência é de Cauchy, então existe $N_1$ tal que $\forall n,m > N_1$ tem-se $D(x_n,x_m) < r_1$.

Mostraremos que existe $R \in \mathbb{R}$ tal que $D(x_i,x_{N_1}) < R$ para todo $i \in \mathbb{Z}^+$, ou seja, $\lbrace x_n \rbrace \subset B_R(x_{N_1})$.

Defina:

$$
r_2 = \max \lbrace D(x_i,x_{N_1})\rbrace_{i \leq N_1}
$$

Perceba que $r_2$ existe pois existem finitos termos da sequência com índices menores que $N_1$.

Perceba agora que:

- $\forall i \leq N_1$ temos $D(x_i,x_{N_1}) \leq r_2$. 
- $\forall i > N_1$ temos que $D(x_i,x_{N_1}) \leq D(x_i, x_{N_1+1}) + D(x_{N_1+1},x_{N_1}) \leq r_1 + D(x_{N_1+1},x_{N_1})$

Logo $\forall i \in \mathbb{Z}^+$ segue que

$$
D(x_i,x_{N_1}) < \underbrace{r_2 + r_1 + D(x_{N_1+1},x_{N_1})}_{R}
$$

Portanto $\lbrace x_n \rbrace \subset B_R(x_{N_1})$ onde $R = r_1 + r_2 + D(x_{N_1+1},x_{N_1})$. $\blacksquare$

### Lema 3
Seja $\lbrace x_n \rbrace$ uma sequência monótona e limitada em $\mathbb{R}$. Então $\lbrace x_n \rbrace$ é convergente.

Suponha sem perder generalidade que $\lbrace x_n \rbrace$ seja monótona crescente. Mostraremos que $\lbrace x_n \rbrace$ converge para $S = \sup \lbrace x_n \rbrace$.

Primeiramente perceba que $S$ existe pois $\lbrace x_n \rbrace$ é limitado superiormente.

Seja então $\epsilon > 0$. Afirmo que existe $N$ tal que $x_N > S - \epsilon$, pois caso contrário, $\lbrace x_n \rbrace < S - \epsilon$, e $S - \epsilon < S$, o que contraria o fato que $S$ é o supremo.

Sendo assim, para $n > N$ tem-se:
$$
S - \epsilon < x_N \leq x_n \leq S < S + \epsilon \implies |x_n - S| < \epsilon
$$ 

onde, da esquerda para a direita, a segunda desiguldade vem do fato que a sequência é monótona crescente e a terceira vem do fato que $S$ é supremo para a sequência.

Ou seja, para arbitrário $\epsilon > 0$, conseguimos mostrar que existe $N$ tal que $n > N$ implica que $|x_N - S| < \epsilon$, logo $\lbrace x_n \rbrace \rightarrow \sup\lbrace x_n \rbrace $. $\blacksquare$


### Lema 4
Se $\lbrace x_n \rbrace$ é uma sequência em $\mathbb{R}$ então existe $\lbrace x_{n_k} \rbrace$ subsequência monótona.

[ESCREVER A PROVA](https://math.stackexchange.com/questions/716461/proof-verification-every-sequence-in-bbb-r-contains-a-monotone-sub-sequence)

$\blacksquare$

---
### Definição de espaço completo
Um espaço métrico $M$ é dito completo se toda sequência de Cauchy em $M$ for convergente.

### $\mathbb{R}$ é completo
Seja $\lbrace x_n \rbrace$ uma sequência de Cauchy nos reais.

- Pelo lema 4, segue que existe uma subsequência $\lbrace x_{n_k} \rbrace$ de $\lbrace x_n \rbrace$ que é monótona;
- Pelo lema 2, $\lbrace x_n \rbrace$ é limitada e portanto $\lbrace x_{n_k} \rbrace$ também é;
- Pelo lema 3, segue que $\lbrace x_{n_k} \rbrace$ é convergente, pois pelo que foi contestado anteriormente garante que $\lbrace x_{n_k} \rbrace$ é monótona e limitada;
- Pelo lema 1, segue que $\lbrace x_n \rbrace$ é convergente.

Logo $\lbrace x_n \rbrace$ converge nos reais. $\blacksquare$