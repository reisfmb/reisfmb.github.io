---
weight: 1412
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.4.12
description: Chap. 1 Exercise 1.4.12
date: 2022-04-05
categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Functions
---
### Pergunta
Let $f: A \rightarrow B$ be a given function. Complements are taken within $A$ for subsets of $A$, and within $B$ for subsets of $B$.

a)

b) 

c) Prove that $f(S') \subset f(S)'$ for any $S \subset A$ if and only if $f$ is one-to-one

### Solução

#### a

#### b

#### c
Primeiramente perceba que $f(S') \subset f(S)'$ implica que $f(S') \cap f(S) = \emptyset$ pois caso o contrário existiria $b \in f(S') \cap f(S)$ logo $b \in f(S')$ mas $b \notin f(S)'$, absurdo. Logo, assumindo $f(S') \subset f(S)'$ obtemos que $f(S') \cap f(S) = \emptyset$ para todo $S \subset A$. 

Suponha então que $f(S') \subset f(S)'$ e em busca de contradição assuma $f$ não injetiva. Logo existem $a_1,a_2 \in A$ tais que $a_1 \neq a_2$ e $f(a_1) = f(a_2)$, ou seja, $f(\lbrace a_1 \rbrace) \cap f(\lbrace a_1 \rbrace') \neq \emptyset$ ou seja, existe $b$ tal que $b \in f(\lbrace a_1 \rbrace')$ mas $b \notin f(\lbrace a_1 \rbrace)'$, logo $f(\lbrace a_1 \rbrace')$ não é subconjunto de $f(\lbrace a_1 \rbrace)'$. Absurdo. Logo $f$ é injetiva.

Assuma então $f$ injetiva e em busca de contradição assuma que para algum subconjunto $S \subset A$ tenha-se que $f(S')$ não seja subconjunto de $f(S)'$, ou seja, $\exists b \in B$ tal que $b \in f(S')$ mas $b \notin f(S)'$. Do fato que $b \notin f(S)'$ segue que $b \in f(S)$, ou seja, $b \in f(S')$ e também $b \in f(S)$, ou seja, existe $a_1 \in S'$ tal que $f(a_1) = b$ e $a_2 \in S$ tal que $f(a_2) = b$. Claramente $a_1 \neq a_2$ pois percetencem a conjuntos disjuntos, nomeadamente $S'$ e $S$. Logo $f$ não pode ser injetiva, o que é uma contradição, da onde segue que todo subconjunto $S$ de $A$ deve satisfazer $f(S') \subset f(S)'$ se $f$ for injetora.