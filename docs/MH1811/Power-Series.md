---
layout: default
title: Power Series
parent: MH1811 - Mathematics 2
nav_order: 9
---

# Power series

{: .highlight}
Find the interval of convergence of the power series
$$\displaystyle\sum_{n=1}^{+\infty}\dfrac{2^n-3^n}{4^n+1}x^n$$
.

**Solution.** Center of convergence is $$x=0$$.

Let
$$a_n=\dfrac{2^n-3^n}{4^n+1}x^n$$
, then its term ratio will be

$$\left|\dfrac{a_{n+1}}{a_n}\right|=\left|\dfrac{\left(2^{n+1}-3^{n+1}\right)x^{n+1}\left(4^{n}+1\right)}{\left(2^{n}-3^{n}\right)x^{n}\left(4^{n+1}+1\right)}\right|=\left|x\times\dfrac{2\times 8^n-3\times 12^n+2\times 2^n-3\times 3^n}{4\times 8^n+2^n-4\times 12^n-3^n}\right|.$$

By Ratio Test, the series converges when
$$\lim_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|<1.$$
We have that

$$
\begin{align*}
&\lim_{n\to\infty}x\times\dfrac{2\times 8^n-3\times 12^n+2\times 2^n-3\times 3^n}{4\times 8^n+2^n-4\times 12^n-3^n}\\
=&\lim_{n\to\infty}x\times\dfrac{2\times\left(\dfrac{8}{12}\right)^n-3+2\times\left(\dfrac{2}{12}\right)^n-3\times\left(\dfrac{3}{12}\right)^n}{4\times\left(\dfrac{8}{12}\right)^n+\left(\dfrac{2}{12}\right)^n-4-\left(\dfrac{3}{12}\right)^n}\\
=&x\times\dfrac{0-3+0+0}{0+0-4+0}=\dfrac{3x}{4}.
\end{align*}
$$

Therefore the series converges when

$$\lim_{n\to\infty}\left|\dfrac{a_{n+1}}{a_n}\right|<1\Leftrightarrow\left|\dfrac{3x}{4}\right|<1\Leftrightarrow |x|<\dfrac{4}{3}\Leftrightarrow -\dfrac{4}{3}<x<\dfrac{4}{3}.$$

And the series diverges when $$x>\dfrac{4}{3}$$ or $$x<-\dfrac{4}{3}$$. The series' radius of convergence is therefore $$R=\dfrac{4}{3}$$.

* At $x=2$ 

{: .highlight }
Compute the infinite series
$$\displaystyle\sum_{n=1}^{+\infty}\dfrac{n}{5^n}.$$

**Solution.** Note that
$$\displaystyle\dfrac{1}{1-x}=\sum_{n=0}^{+\infty}x^n,$$
differentiating term-by-term gives

$$\left(\dfrac{1}{1-x}\right)'_x=\sum_{n=0}^{+\infty}\left(x^n\right)'_x\Leftrightarrow\dfrac{1}{(1-x)^2}=\sum_{n=1}^{+\infty}nx^{n-1}=\sum_{n=0}^{+\infty}(n+1)x^n.$$

(the sum starts from
$$n=1$$
to handle unexpected behaviour of the term). 

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
is actually equal to $$0$$ when $$n=0$$).