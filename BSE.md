---
layout: default
title: Black--Scholes equation
permalink: /BSE/

---
<script>
  window.MathJax = {
    tex: { inlineMath: [['\\(','\\)']], displayMath: [['$$','$$']] }
  };
</script>
<script defer src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script>

# Black--Scholes equation

The function \( u(x,t) \) satisfies the heat equation.
$$
\frac{\partial u}{\partial t}
= \alpha \left(
  \frac{\partial^2 u}{\partial x^2}
  + \frac{\partial^2 u}{\partial y^2}
\right),
\quad (x,y)\in \Omega,\; t>0
$$

