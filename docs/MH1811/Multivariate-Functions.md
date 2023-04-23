---
layout: default
title: Functions of Several Variables
parent: MH1811 - Mathematics 2
nav_order: 1
---

# Functions of Several Variables

{: .highlight}
Does the limit
$$\displaystyle\lim_{(x,y)\to(0,0)}\dfrac{x^2\sin(xy^2)}{x^4+9y^4}$$
exists? If it does, what is the limit? Justify your answer.

**Solution.** We acknowledge these two results:

* $$\sin(x)\le x$$
for positive values of $$x$$.
* $$\dfrac{xy}{x^2+y^2}\le\dfrac{1}{2},$$
equality holds when $$x=y$$.

Applying the above results give

$$0\le\left|\dfrac{x^2\sin(xy^2)}{x^4+9y^4}\right|\le\left|\dfrac{x^2\times xy^2}{\left(x^2\right)^2+\left(3y^2\right)^2}\right|\le\left|\dfrac{x}{6}\right|.$$

Since
$$\displaystyle\lim_{(x,y)\to(0,0)}0=0,$$
and
$$\lim_{(x,y)\to(0,0)}\left|\dfrac{x}{6}\right|=0,$$
by Squeeze Theorem one must have

$$\displaystyle\lim_{(x,y)\to(0,0)}\left|\dfrac{x^2\sin(xy^2)}{x^4+9y^4}\right|=0.$$

Therefore
$$\displaystyle\lim_{(x,y)\to(0,0)}\dfrac{x^2\sin(xy^2)}{x^4+9y^4}=0,$$
as desired.