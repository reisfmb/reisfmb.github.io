---
weight: 128
author: Bruno Reis
title: (Irving Kaplansky - Set Theory And Metric Spaces) Capítulo 1, exercício 1.2.8
description: Chap. 1 Exercise 1.2.8
date: 2022-04-02

categories:
  - Irving Kaplansky - Set Theory And Metric Spaces
tags:
  - Teoria dos conjuntos
---
### Pergunta
With an arbitrary (possibly infinite) index set $I$, prove:

a) $A \cup ( \cap_{i} B_i ) = \cap_{i} ( A \cup B_i )$

b) $A \cap ( \cup_{i} B_i ) = \cup_{i} ( A \cap B_i )$

In (c) and (d) the complementation is taken relative to a fixed universal set $U$.

c) $( \cup_{i}A_i )^{'} = \cap_{i}A_i^{'}$

d) $( \cap_{i}A_i )^{'} = \cup_{i}A_i^{'}$

### Solução

#### a
Basta utilizar 
$A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$ 
iterativamente...

$$
\begin{align*}
  A \cup ( \cap_{i} B_i ) 
  &= A \cup (B_1 \cap (\cap_{i > 1} B_i) ) \newline
  &= (A \cup B_1) \cap (A \cup \cap_{i > 1} B_i) \newline
  &= (A \cup B_1) \cap (A \cup (B_2 \cap (\cap_{i > 2} B_i))) \newline
  &= (A \cup B_1) \cap (A \cup B_2) \cap (A \cap (\cap_{i > 2} B_i)) \newline
  &= \cdots \newline
  &= (A \cup B_1) \cap (A \cup B_2) \cap (A \cup B_3) \cap \cdots \newline
  &= \cap_{i}(A \cup B_i)
\end{align*}
$$

#### b
O procedimento é o mesmo que o anterior, entretanto deve-se utilizar o fato que 

$A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$

#### c
Basta utilizar 
$(A \cup B)^{'} = A^{'} \cap B^{'}$ 
iterativamente...

$$
\begin{align*}
  ( \cup_{i}A_i )^{'} 
  &= (A_1 \cup (\cup_{i>1}A_i))^{'} \newline
  &= A_1^{'} \cap (\cup_{i>1}A_i)^{'} \newline
  &= A_1^{'} \cap (A_2 \cup (\cup_{i>2}A_i))^{'} \newline
  &= A_1^{'} \cap A_2^{'} \cap (\cup_{i>2}A_i)^{'} \newline
  &= \cdots \newline
  &= A_1^{'} \cap A_2^{'} \cap A_3^{'} \cdots \newline
  &= \cap_{i}A_i^{'}
\end{align*}
$$

#### d

O procedimento é o mesmo que o anterior, entretanto deve-se utilizar o fato que 

$(A \cap B)^{'} = A^{'} \cup B^{'}$