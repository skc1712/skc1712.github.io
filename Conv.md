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

So pointwise convergence holds.

Note that each $f_n(x) = x^n$ is continuous, but the limit $f$ is not continuous at 1. So pointwise convergence does not preserve continuity.

## Uniform convergence

$$
f_n \to f  
$$
,
uniform on $E$ means:


$$
\forall \epsilon > 0, \exists N = N(\epsilon) \, \text{such that} \, n \ge N \implies |f_n(x) - f(x)| < \epsilon, \, \forall x \in E
$$
.

Equivalent form:

$$
\sup_{x\in E} |f_n(x) \to f(x)| \to 0.  
$$
.

Example:

On $[0, 1], \, f_n(x)= \frac{x}{n}.$ Then

$$
\sup_{x\in[0, 1]} |f_n(x)| = \frac{1}{n} \to 0,
$$
so $f_n \to 0$, uniformly.

Standard counterexample:
$f_n(x) = x^n$ converges pointwise, but not uniformly, because
$$
\sup_{x\in[0, 1]} |x^n - f(x)| = 1, \quad \forall n
$$
.

Note that uniform convergence preserves continuity. 

## Locally uniform convergence


$$
f_n \to f  
$$
,
locally uniform on $U$, 

means uniform convergence on every compact subset $K \subset U$.

Example: 

$$
f_n(x) = \frac{x}{n}
$$
,

converges locally uniformly on $\mathbb{R}$, in fact, uniformly on every bounded interval.

Counterexample to global uniformity:

$$
f_n(x) = \frac{x}{n}, \quad x \in \mathbb{R}
$$
,
does not converge uniformly on all of $\mathbb{R}$, because

$$
\sup_{x\in\mathbb{R}} \left| \frac{x}{n} \right| = \infty
$$
.

# Convergence in a metric space

In a metric space $(X, d), x_n \to x$, means

$$
d(x_n, x) \to 0
$$
.

Example:

In $C([0, 1])$ with the sup metric

$$
d(f, g) = \sup_{x\in[0, 1]} |f(x) - g(x)|
$$
,

metric convergence is exactly uniform convergence.

In $L^p$, metric convergence is $L^p$-convergence. 

# Norm (Strong) convergence
In a normed space $(X, \|\cdot\|$,

$$
x_n \to x \quad \text{strongly (or in norm)}
$$

means,

$$
\| x_n - x\| \to 0
$$
.

Example:

- In $C([0, 1])$ 

$$
\|f_n - f\|_\infty \to 0
$$
is uniform convergence.

- In $l^2$, $e_n$ does not converge strongly to 0, because $\|e_n\|_2=1$.

# Weak convergence

Let $X$ be a normed space and $X^*$ be its dual. Then

$$
x_n \rightharpoonup x
$$
,
means:

for every continuous linear function $\varphi\in X^*$

$$
\varphi(x_n) \to \varphi(x)
$$
.

Example:
In a Hilbert space $l^2$, the standard basis $e_n \rightharpoonup 0$ weakly:

for any $y = (y_k) \in l^2$,  
$$
\langle y, e_n \rangle = y_n \to 0  
$$
.
But $e_n \not \to 0$, because $\| e_n \| = 1$. 

Note that convergence in norm implies weak convergence, but not vice versa in infinite-dimensional spaces. 

# Weak$-^*$ convergence

If $\varphi_n^*\in X^*$ then

$$
\varphi_n^* \rightharpoonup \varphi^*
$$
,
means

$\forall x \in X$, 

$$
\varphi_n^*(x) \to \varphi^*(x)
$$
.

Example:

In $l^\infty = (l^1)^*$, weak $-^*$ convergence means pointwise convergence on $l^1$-pairings.
