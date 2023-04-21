---
layout: default
title: Power Series
parent: MH1811
nav_order: 9
---

# Power series
**1.** Compute the infinite series
$$\displaystyle\sum_{n=1}^{+\infty}\dfrac{n}{5^n}.$$

**Solution.** Note that
$$\displaystyle\dfrac{1}{1-x}=\sum_{n=0}^{+\infty}x^n,$$
differentiating term-by-term gives

$$\left(\dfrac{1}{1-x}\right)'_x=\sum_{n=0}^{+\infty}\left(x^n\right)'_x\Leftrightarrow\dfrac{1}{(1-x)^2}=\sum_{n=1}^{+\infty}nx^{n-1}=\sum_{n=0}^{+\infty}(n+1)x^n.$$

(the sum starts from $$n=1$$ to handle unexpected behaviour of the term). 

Subtracting
$$\displaystyle\dfrac{1}{1-x}=\sum_{n=0}^{+\infty}x^n$$
from both sides give

$$\dfrac{1}{(1-x)^2}-\dfrac{1}{1-x}=\sum_{n=0}^{+\infty}nx^n\Leftrightarrow\sum_{n=0}^{+\infty}nx^n=\dfrac{x}{(1-x)^2}.$$

When
$$x=\dfrac{1}{5},$$
we have
$$\displaystyle\sum_{n=0}^{+\infty}\dfrac{n}{5^n}=\sum_{n=1}^{+\infty}\dfrac{n}{5^n}=\dfrac{1}{5\left(1-\dfrac{1}{5}\right)^2}=\dfrac{5}{16}$$
as the desired result (since the first term of
$$\dfrac{n}{5^n}$$
is actually equal to
$$0$$
when
$$n=0$$
).