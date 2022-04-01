---
author: Bruno Reis
title: (Spivak Calculus) Capítulo 1, exercício 22
description: Chap. 1 Exercise 22
date: 2022-04-01
categories:
  - Spivak - Calculus
tags:
  - Desigualdades
---
Primeiro é importante perceber que dizer que $x < \min(a,b)$ é o mesmo que dizer que:

- $x < a$ e também que
- $x < b$

Sendo assim, segue diretamente que:

$$
\begin{align}
    |y - y_0| &< \frac{|y_0|}{2}\newline
    |y - y_0| &< \frac{\epsilon|y_0|^2}{2}
\end{align}
$$

Perceba então a seguinte igualdade:

$$
\begin{align*}
   \frac{1}{y} - \frac{1}{y_0} &= 
   \frac{y_0}{y_0}\frac{1}{y} - \frac{y}{y}\frac{1}{y_0}\newline
   &=\frac{y_0 - y}{yy_0} 
\end{align*}
$$

Da onde segue que:

$$
\begin{align*}
   \left | \frac{1}{y} - \frac{1}{y_0} \right | &= \left | \frac{y_0 - y}{yy_0} \right |\newline
   &= \frac{|y_0 - y|}{\left | yy_0 \right |}\newline
   &= \frac{|y - y_0|}{|y||y_0|}
\end{align*}
$$

Utilizando essa conclusão, junto de (2) conclui-se que:

$$
\begin{align}
    \left | \frac{1}{y} - \frac{1}{y_0} \right | = \frac{|y - y_0|}{|y||y_0|} < \frac{\frac{\epsilon|y_0|^2}{2}}{|y||y_0|} = \frac{\epsilon|y_0|}{2|y|}
\end{align}
$$

Analisando a desigualdade (3) percebe-se que se provarmos que $|y_0| < 2|y|$ então obteremos a desigualdade desejada, uma vez que $\frac{\epsilon|y_0|}{2|y|} < \epsilon$ caso $|y_0| < 2|y|$.

Com tal finalidade, observe que pela desigualdade triangular, temos que:

$$
\begin{align*}
    |y_0| = |y_0-y+y| \leq |y_0-y| + |y| = |y-y_0| + |y|
\end{align*}
$$

Utilizando a desigualdade (1), tem-se:

$$
\begin{align*}
    |y_0| \leq |y-y_0| + |y| < \frac{|y_0|}{2} + |y|
    &\implies |y_0| - \frac{|y_0|}{2} < |y|\newline
    &\implies 2|y_0| - |y_0| < 2|y|\newline
    &\implies |y_0| < 2|y|
\end{align*}
$$

Como queríamos demonstrar. Dessa conclusão, juntamente de (3), segue que:

$$
\left|\frac{1}{y} - \frac{1}{y_0}\right| < \epsilon
$$
