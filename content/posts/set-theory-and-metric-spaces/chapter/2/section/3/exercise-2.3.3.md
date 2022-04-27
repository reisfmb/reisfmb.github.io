---
weight: 233
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.3.3
description: Chap. 1 Exercise 2.3.3
date: 2022-04-26
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Convergence
---
### Pergunta
Prove: In a metric space $x_i \rightarrow x$ if and only if $D(x_i,x) \rightarrow 0$.

### Solução
Defina $D_i = D(x_i,x)$.

Suponha que $D_i \rightarrow d > 0$. Mostraremos que isso gera uma contradição com o fato que $x_i \rightarrow x$.

Tome $\epsilon_1 > d$, logo para todo $i > N_{\epsilon_1}$ segue que $|D_i - d| < \epsilon_1$ da onde segue que $\epsilon_1 - d < D_i$.

Tome $\epsilon_2 < \frac{\epsilon_1 - d}{2}$, logo para todo $i > N_{\epsilon_2}$ segue que $D_i < \frac{\epsilon_1 - d}{2}$.

Segue então que para $i > \max(N_{\epsilon_1}, N_{\epsilon_2})$ tem-se $\epsilon_1 - d< D_i < \frac{\epsilon_1 - d}{2}$ o que implica que $\epsilon_1 - d < \frac{\epsilon_1 - d}{2}$, absurdo, logo $d = 0$.

Suponha agora que $D_i \rightarrow 0$, logo para todo $\epsilon$ segue que $|D_i| < \epsilon$ para $i$ suficientemente grande. 

Como por definição $D_i \geq 0$, segue que $D(x_i,x) < \epsilon$ para $i$ suficientemente grande, que é justamente a definição de $x_i \rightarrow x$.