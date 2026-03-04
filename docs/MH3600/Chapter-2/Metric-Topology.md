---
layout: default
title: The Metric Topology
parent: Topological Spaces and Continuous Functions
nav_order: 3
---

# The Metric Topology

{: .new }
> A **metric** on a set $$X$$ is a function $$d\colon X\times X\to\mathbb{R}$$ having the following properties:
> 1. $$d(x, y)\ge 0$$ for all $$x, y\in X$$; equality holds if and only if $$x=y$$.
> 2. $$d(x, y)=d(y,x)$$ for all $$x, y\in X$$.
> 3. (Triangle inequality) $$d(x, y)+d(y,z)\ge d(x, z)$$ for all $$x, y, z\in X$$.

{: .new }
Given $$\varepsilon>0$$, the set $$B_d(x,\epsilon)=\{y\vert d(x,y)<\varepsilon\}$$ of all points $$y$$ whose distance from $$x$$ is less than $$\varepsilon$$ is called the **$$\varepsilon$$-ball centered at $$x$$**.

{: .new }
If $$d$$ is a metric on the set $$X$$, then the collection of all $$\varepsilon$$-balls $$B_d(x,\varepsilon)$$, for $$x\in X$$ and $$\varepsilon>0$$, is a basis for a topology on $$X$$, called the **metric topology** induced by $$d$$.

Equivalently, a set $$U$$ is open in the metric topology induced by $$d$$ if and only if for each $$y\in U$$, there is a $$\delta>0$$ such that $$B_d(y, \delta)\subset U$$.