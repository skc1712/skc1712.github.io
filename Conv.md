---
layout: default
title: Convergence
permalink: /Conv/
---
Convergence is a topic which starts to appear right from the beginning of a maths degree. A good way to understand this concept is to categorise it by what is converging:

# 1. numbers/sequences/series

A sequence $x_n$ converges to $x$ if for every $\epsilon$, there exists $N$ such that


$$
n \ge N \implies |x_n - x| < \epsilon
$$
.

### Example.
$$
x_n = \frac{1}{n} \to 0
$$
.

### Counterexample.

$$
x_n = (-1)^n
$$
,
does not converge.

## Cauchy convergence
A sequence $x_n$ is Cauchy if for every $\epsilon > 0$, there exists $N$ such that


$$
m, n \ge N \implies |x_n - x_m| < \epsilon
$$
.

### Example.
$$
x_n = \frac{1}{n} \to 0
$$
.

In fact, in $\mathbb{R}, \mathbb{C}$, Cauchy $\leftrightarrow$ convergent.


## Monotone convergence for sequences
If $x_n$ is monotone and bounded, then it converges.

### Example.
$$
x_n = 1-\frac{1}{n},
$$
is increasing and bounded above by 1, so $x_n \to 1$. 

# 2. For functions

Let $f_n: E \to \mathbb{R}$, f: E \to \mathbb{R}$. 

## Pointwise convergence

$$
f_n \to f  
$$
,
pointwise on $E$ means:

for every fixed $x \in E$, 

$$
f_n(x) \to f(x) 
$$
.

Equivalently,

$$
\forall x \in E, \forall \epsilon > 0, \exists N = N(x, \epsilon) \, \text{such that} \, n \ge N \implies |f_n(x) - f(x)| < \epsilon
$$
.
Example:
On $[0, 1], \, f_n(x)=x^n.$ Then

$$
f_n(x) \to f(x) =
\begin{cases}
0, \quad 0 \le x < 1 \\
1, \quad x = 1
\end{cases}
$$
.

# functions
# vectors in normed or topological spaces
# measurable functions / random variables

