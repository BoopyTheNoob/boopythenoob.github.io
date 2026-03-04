---
layout: default
title: The Product Topology
parent: Topological Spaces and Continuous Functions
nav_order: 2
---

# The Product Topology

Consider the Cartesian products $$X_1\times\cdots\times X_n$$ and $$X_1\times X_2\times\cdots$$, where each $$X_i$$ is a topological space.

{: .new }
> Let $$J$$ be an index set. Given a set $$X$$, we define a **$$J$$-tuple** of elements of $$X$$ to be a function $$\mathbf{x}\colon J\to X$$.
> 
> If $$\alpha$$ is an element of $$J$$, we often denote the value of $$\mathbf{x}$$ at $$\alpha$$ by $$x_{\alpha}$$ rather than $$\mathbf{x}(\alpha)$$; we call it the $$\alpha$$th **coordinate of $$\mathbf{x}$$.
> 
> We denote the function $$\mathbf{x}$$ itself by the symbol $$(x_\alpha)_{\alpha\in J}$$.
>
> We denote the set of all $$J$$-tuples of elements of $$X$$ by $$X^J$$.

{: .new }
> Let $$\{A_{\alpha}\}_{\alpha\in J}$$ be an indexed family of sets; let $$\displaystyle X=\cup_{\alpha\in J}A_{\alpha}$$.
>
> The **cartesian product** of this indexed family, denoted by $$\displaystyle\prod_{\alpha\in J}A_{\alpha}$$, is defined to be the set of all $$J$$-tuples $$(x_\alpha)_{\alpha\in J}$$ of elements of $$X$$ such that $$x_{\alpha}\in A_{\alpha}$$ for each $$\alpha\in J$$.
>
> That is, it is the set of all functions $$\displaystyle\mathbf{x}\colon\cup_{\alpha\in J}A_{\alpha}$$ such that $$\mathbf{x}(\alpha)\in A_\alpha$$ for each $$\alpha\in J$$.