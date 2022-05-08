---
weight: 238
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.3.8
description: Chap. 1 Exercise 2.3.8
date: 2022-04-28
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Limit point
---
### Pergunta
Pove: The diameter of a set $A$ in a metric space is the same as the diameter of its closure.

### Solução
Seja $A \subset M$. Como $A \in \overline{A}$ segue que $\text{diam}(A) \leq \text{diam}(\overline{A})$.

Mostraremos então que $\text{diam}(\overline{A}) \leq \text{diam}(A)$.

Sejam $x,y \in \overline{A}$.

Se $x,y \in A$ então $d(x,y) < \text{diam}(A)$.

Se $x \in A$ e $y \notin A$ então $y$ é ponto limite de $A$ pois $y \in \overline{A \setminus \lbrace y \rbrace}$, logo para todo $r > 0$ segue que $B_r(y) \cap A \neq \emptyset$, ou seja, para todo $r > 0$ existe $z \in B_r(y) \cap A$ tal que $d(y,z) < r$, logo

$$
D(x,y) \leq D(x,z) + D(z,y) < \text{diam}(A) + r = \text{diam}(A) + \epsilon
$$

Suponha então que $x$ e $y$ não estejam em $A$, logo $x$ e $y$ são pontos limites, e pelo mesmo argumento anterior segue que para qualquer $r_1,r_2 > 0$ existem $z,w \in A$ tais que $D(x,z) < r_1$ e $D(y,w) < r_2$, logo

$$
D(x,y) \leq D(x,z) + D(z,w) + D(w,y) < r_1 + \text{diam}(A) + r_2 = \text{diam}(A) + \epsilon
$$

Ou seja, para qualquer $x,y \in \overline{A}$ concluimos que para $\epsilon$ arbitrário tem-se $\text{diam}(\overline{A}) < \text{diam}(A) + \epsilon$, o que implica que $\text{diam}(\overline{A}) \leq \text{diam}(A)$ pois caso contrário então teriamos $\text{diam}(\overline{A}) > \text{diam}(A)$, o que é aburdo pois basta tomar $\epsilon = \frac{\text{diam}(\overline{A}) - \text{diam}(A)}{2}$ que teriamos:

$$
\begin{align*}
\text{diam}(\overline{A}) &< \text{diam}(A) + \epsilon \newline
&< \text{diam}(A) +  \frac{\text{diam}(\overline{A}) - \text{diam}(A)}{2} \newline
&< \frac{\text{diam}(A) + \text{diam}(\overline{A})}{2} \newline
\text{diam}(\overline{A}) &< \text{diam}(A) \newline
\end{align*}
$$

logo

$$
\text{diam}(A) = \text{diam}(\overline{A})
$$

