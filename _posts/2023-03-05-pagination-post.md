---
layout: post
title: "Extending The Lebesgue Measure"
author: "Vivaan Daga"
tags: Measure-theory, Set-theory
usemathjax: true


---
# Contents
{:.no_toc}

* Will be replaced with the ToC, excluding the "Contents" header
{:toc}

# Introduction
The problem of assigning measure(length, area, volume, hyper-volume) to subsets in $\mathbb{R}^d$  and its deep connection with the theory of integral has been examined by several mathematicians of the 19th century including Augustin Cauchy, Lejeune Dirichlet, Bernhard Riemann, Camille Jordan, Emile Borel, Henri Lebesgue, and Giuseppe Vitali. The ultimate dream was to find a measure $m:\mathcal{P}(\mathbb{R})\to[0,\infty]$ on all subsets of $\mathbb{R}^d$ satisfying the following properties:

- $$m([0,1]^d)=1$$.
- If $$E_n$$ is a countable collection of pairwise disjoint sets in $$\mathbb{R}^d$$, then $$m(\bigcup E_n)=\sum_{n=1}^{\infty} m(E_n)$$. (Countable Additivity)
- If $$\tau$$ is a rigid-motion from $$\mathbb{R}^d\to \mathbb{R}^d$$ and $$E$$ is a subset of $$\mathbb{R}^d$$ then $$m(E)=m(\tau(E))$$. (Invariance under rigid-motions)

Unfortunately, the dream was shattered by Giuesspe Vitali by his construction of the so-called "Vitali set". Indeed, Vitali proved that no such measure could exist on all subsets of $$\mathbb{R}^d$$. 
\newline
Not all hope was lost however, even though one can not have such a measure on all subsets of $$\mathbb{R}^d$$, one can still hope to have a measure on a "large" subset of $$\mathcal{P}(\mathbb{R}^d)$$ that suffices for all practical purposes, and this is exactly what the Lebesgue measure is, on the family of Lebesgue measurable sets. It turns out that the the family of Lebesgue measurable sets is large enough that for all practial purposes of analysis the measure problem is solved, however it is it remains an interesting question to ask "How much can we extend Lebesgue Measure" while trying to retian its properties. This shall be our aim for this blog, but to ask this question precsicely we need to set up several definitions.

# The set up

Here we see **Tale's** pagination feature in action. It is set to 5 posts per page by default. Feel free to change this number in the `_config.yml` file!

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

The following is a math block $x^2\sin(x)\cos(x)$
<script src="https://unpkg.com/@lyket/widget@latest/dist/lyket.js?apiKey=pt_66df15dfbc78920218145f5b7ee867"></script>
