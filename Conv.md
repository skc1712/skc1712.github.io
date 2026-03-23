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

# 2. For series


# functions
# vectors in normed or topological spaces
# measurable functions / random variables

