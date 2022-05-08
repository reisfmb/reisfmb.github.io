---
weight: 234
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 2, exercício 2.3.4
description: Chap. 1 Exercise 2.3.4
date: 2022-04-26
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Metric Spaces
  - Convergence
---
### Pergunta
Given two distinc points $x$ and $y$ in a metric space, prove that there exist open sets $U$ and $V$ such that $x \in U$, $y \in V$, and $\overline{U} \cap \overline{V}$ is empty. (Observe that this sharpens [this exercise](../../2/exercise-2.2.2))

### Solução
Do exercício em questão garantimos a existência dos abertos $U$ e $V$, que na verdade são bolas abertas disjuntas. Da letra a do [exercício 6](../exercise-2.3.6) segue que uma bola fechada é um conjunto fechado. Sendo assim, considere os fechados naturais, nomeadamente $F_U, F_V$ como extensão das bolas abertas $U$ e $V$. Tais fechados são disjuntos e portanto $\overline{U} \cap \overline{V} = \emptyset$. 

Para ver isso, considere que $\overline{U} \cap \overline{V} \neq \emptyset$ então existira elemento que $k$ pertencente ao fecho de $U$ e ao fecho de $V$, isso significa que $k$ pertence a todos os fechados que contém $U$ e todos os fechados que contém $V$. Ora, $F_U$ e $F_V$ são fechados que conteḿ $U$ e $V$ respectivamente, entretanto, por definição desses fechados, $F_U \cap F_V = \emptyset$, ou seja, tal $k$ não existe, logo a intercessão dos fechos é vazia.