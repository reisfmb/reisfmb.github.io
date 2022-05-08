---
weight: 2
author: Bruno Reis
title: Elementary probability definitions
description: Elementary probability definitions and basic results
date: 2022-04-23
categories:
  - Articles
tags:
  - Probability
---
### Espaço amostral
Se $\Omega$ é um conjunto não vazio formado com todos os possíveis resultados de um experimento, então chamamos $\Omega$ de espaço amostral.

### Evento aleatório
Seja $\Omega$ um espaço amostral. Qualquer subconjunto $A \subset \Omega$ é chamado de evento aleatório.

### Sigma álgebra ($\sigma$-álgebra)
Uma classe de subconjuntos de $\Omega$, nomeadamente $F$, é considerada uma $\sigma$-álgebra se:

1. $\Omega \in F$
2. Para todo $A \in F$ segue que $A^c \in F$
3. Se $A_1,A_2, \cdots \in F$ então $(\cup_{i=1}^\infty A_i) \in F$

#### Observações sobre uma $\sigma$-álgebra $F$
- Por 1 e 2, segue que $\emptyset \in F$;
- União finita está em $F$, pois basta tomar para certo $i > n$ todos os conjuntos como sendo o vazio dado a conclusão anterior;
- Por 2 e 3, segue que $(\cap_{i=1}^\infty A_i) \in F$ dado que $(\cup_{i=1}^\infty A_i^c)^c = (\cap_{i=1}^\infty A_i)$;
- Se $A, B \in F$ então $A \setminus B \in F$ pois $A \setminus B = A \cap B^c$.

### Medida de probabilidade
Seja $\Omega$ um espaço amostral e $F$ uma $\sigma$-álgebra de $\Omega$. Uma medida de probabilidade $P$ é uma função $P: F \rightarrow \mathbb{R}$ tais que:

1. $P(\Omega) = 1$
2. $P(A) \geq 0$ para todo $A \in F$
3. Se $(A_n)$ são eventos disjuntos, então $P(\cup_{i=1}^\infty A_i) = \sum_{i=1}^\infty P(A_i)$

#### Observações sobre uma medida de probabilidade
1. $P(\emptyset) = 0$
2. $P(A^c) = 1 - P(A)$
3. Se $A \subset B$ vale $P(B \setminus A) = P(B) - P(A)$
4. $0 \leq P(A) \leq 1$
5. $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
6. $P(\cup_{i=1}^\infty A_i) \leq \sum_{i=1}^\infty P(A_i)$

Prova de 1) $P(\Omega) = P(\Omega \cup \emptyset \cup \emptyset \cup \cdots) = P(\Omega) + P(\emptyset) = 1 + P(\emptyset) = 1 \implies P(\emptyset) = 0$.

Prova de 2) $P(\Omega) = P(A \cup A^c) = P(A) + P(A^c) = 1 \implies P(A^c) = 1 - P(A)$

Prova de 3) $P(B) = P(B \setminus A \cup A) = P(B \setminus A) + P(A) \implies P(B \setminus A) = P(B) - P(A) \implies P(B) \geq P(A)$

Prova de 4) $P(A) \leq 1$ pois $A \subset \Omega$ e $P(\Omega) = 1$. $P(A) \geq 0$ por definição.

Prova de 5) $P(A \cup B) = P(A \cup (B \setminus A)) = P(A) + P(B \setminus A)$, porém $P(B) = P(B \setminus A \cup (A \cap B)) = P(B \setminus A) + P(A \cap B)$ logo $P(A \cup B) = P(A) + P(B) - P(A \cap B)$.

Prova de 6) Segue diretamente de 5 e da propriedade 3 de uma medida de probabilidade
