---
layout: default
title: Assignment
parent: MH3600 - Topology and Manifolds
nav_order: 1
---

# Take-home Assignment

{: .highlight }
> **Problem 1.**
>
> (i) Let $$Y$$ be a topological space. Show that $$Y$$ is Hausdorff if and only if the diagonal
>
> $$\Delta_Y=\{(y,y)|y\in Y\}\subset Y\times Y$$
> 
> is a closed subset of $$Y\times Y$$ with the Cartesian product topology.
> 
> (ii) Let $$X$$ and $$Y$$ be two topological spaces with $$Y$$ Hausdorff, and consider two continuous functions $$f, g\colon X\to Y$$. Show that $$Z\subset X$$ defined by
>
> $$Z=\{x\in X|f(x)=g(x)\}$$
>
> is closed in $$X$$.

_Solution._

(i) _For the first part_, assume $$Y$$ is Hausdorff and we want to show that the diagonal $\Delta_Y$ is closed with respect to $$Y\times Y$$.

Let $$(x,y)\in Y\times Y\setminus\Delta_Y$$, then $$x\ne y$$ by definition of the diagonal. As $$Y$$ is Hausdorff, there exists two neighboorhoods $$U$$ and $$V$$ of $$x$$ and $$y$$, respectively, that are disjoint. Therefore $$(x, y)\in U\times V\subset Y\times Y$$.

As $$U$$ and $$V$$ are open in $$Y$$, their Cartesian product $$U\times V$$ is a basis element of $$Y\times Y$$ and is open in this product topology as well.

Assume that $$(v, w)$$ is an intersection point in both $$U\times V$$ and $$\Delta_Y$$. Then:
* $$(v, w)\in U\times V$$ implies that $$v\in U$$ and $$w\in V$$; and since $$U$$ and $$V$$ are disjoint sets we must have $$v\ne w$$.
* $$(v, w)\in\Delta_Y$$ so $$v=w$$.

A contradiction arises ($$v\ne w$$ and $$v=w$$ at the same time), so therefore $$(v, w)$$ cannot be in both $$U\times V$$ and $$\Delta_Y$$. This implies that $$U\times V$$ and $$\Delta_Y$$ are disjoint.

As we have found a neighborhood of $$(x, y)$$ that does not intersect $$\Delta_Y$$ (at some point other than $$(x, y)$$), $$(x,y)$$ cannot be a limit point of $$\Delta_Y$$. But $$(x, y)$$ is arbitrary in $$Y\times Y\setminus\Delta_Y$$, this implies that no points outside of $$\Delta_Y$$ can be a limit point of $$\Delta_Y$$. This is equivalent to saying that all limit points of $$\Delta_Y$$ is in $$\Delta_Y$$, or $$\Delta_Y$$ contains all of its limit points. Therefore $$\Delta_Y$$ is closed according to the collorary on Chapter 2, Slide 99.

_For the second part_, assume $$\Delta_Y$$ is closed with respect to $$Y\times Y$$ and we want to show that $$Y$$ is Hausdorff.

Let $$x$$ and $$y$$ be two distinct elements in $$Y$$, then $$(x, y)\in Y\times Y\setminus\Delta_Y$$ be an arbitrary point outside of $$\Delta_Y$$. Since $$\Delta_Y$$ is closed, it contains all of its limit point and $$(x,y)$$ cannot be a limit point of $$\Delta_Y$$. Therefore, there exists a neighborhood $$T$$ of $$(x, y)$$ that does not intersect $$\Delta_Y$$.

By the construction of the product topology $$Y\times Y$$ from its basis, there exists a basis element $$U\times V$$ of $$T$$ such that $$(x, y)\in U\times V\subset T$$ where $$U$$ and $$V$$ are open in $$Y$$. Then $$x\in U$$ and $$y\in V$$.

Assume that $$z\in Y$$ is within the intersection $$U\cap V$$, then:
* as $$(z,z)\in U\times V$$. As $$U\times V\subset T$$ and $$T$$ does not intersect $$\Delta_Y$$, we must have that $$(z,z)\not\in \Delta_Y$$;
* as $$z=z$$, $$(z,z)\in \Delta_Y$$.

A contradiction arises ($$(z,z)$$ both not in $$\Delta_Y$$ and in $$\Delta_Y$$ at the same time), so therefore $$U\cap V$$ must be empty or $$U$$ and $$V$$ are disjoint. Since we are able to determine open neighborhoods $$U$$ and $$V$$ of $$x$$ and $$y$$ respectively that are disjoint, and that $$x$$ and $$y$$ are arbitrary distinct elements in $$Y$$, the topological space $$Y$$ must therefore be Hausdorff.

(ii) Let $$x\in X\setminus Z$$, then by definition of $$Z$$ we have $$f(x)\ne g(x)$$. Let $$y_1=f(x)$$ and $$y_2=g(x)$$ be the resulting distinct elements in $$Y$$. As $$Y$$ is Hausdorff, there exists neighborhoods $$V_1$$ and $$V_2$$ of $$y_1$$ and $$y_2$$, respectively, that are disjoint.

Since $$f$$ and $$g$$ are continuous functions, the preimages $$U_1=f^{-1}(V_1)$$ and $$U_2=g^{-1}(V_2)$$, of $$V_1$$ and $$V_2$$ respectively, are open in $$X$$. As $$f(x)=y_1\in V_1$$ and $$g(x)=y_2\in V_2$$, we have that $$x\in U_1$$ and $$x\in U_2$$, or equivalently $$x\in U_1\cap U_2$$. Note that $$U_1\cap U_2$$ is open in $$X$$ as $$U_1$$ and $$U_2$$ are open in $$X$$ and finite intersections of open sets are also open.

Assume that there exists some element $$z\in Z$$ that is also in $$U_1\cap U_2$$. Then:
* as $$f(z)\in V_1$$ and $$g(z)\in V_2$$, and that $$V_1\cap V_2=\empty$$ ($$V_1$$ are $$V_2$$ are disjoint open sets) so therefore $$f(z)\ne g(z)$$;
* as $$z\in Z$$ so $$f(z)=g(z)$$ by definition.

A contradiction arises ($$f(z)\ne g(z)$$ and $$f(z)=g(z)$$ at the same time), so therefore the intersection between $$U_1\cap U_2$$ and $$Z$$ must be empty. As we are able to point out a neighborhood $$U_1\cap U_2$$ of $$x$$ that does not intersect $$Z$$ (at another point), $$x$$ is not a limit point of $$Z$$. As $$x$$ is arbitrary among $$X\setminus Z$$, any limit point of $$Z$$ cannot lie outside $$Z$$. Hence all limit points of $$Z$$ lie in $$Z$$, and therefore the set $$Z$$ is closed.

{: .highlight }
> **Problem 2.**
> Let $$X$$ be a topological space.
>
> (i) Show that if a subset $$A$$ of $$X$$ is open if $$B$$ is a subset of $$X$$ with $$A\cap B=\emptyset$$, then $$A\cap\overline{B}=\emptyset$$, but $$\overline{A}\cap\overline{B}$$ is not necessarily empty.
>
> (ii) Show that
> * $$A\subset B$$ implies $$\mathrm{int}(\overline{A})\subset\mathrm{int}(\overline{B})$$ and $$\overline{\mathrm{int}(A)}\subset\overline{\mathrm{int}(B)}$$.
> * $$A$$ open implies $$A\subset\mathrm{int}(\overline{A})$$
> * $$A$$ closed implies $$\overline{\mathrm{int}(A)}\subset A$$.
>
> (iii) Find $$A\subset\mathbb{R}$$ such that $$A$$, $$\overline{A}$$, $$\mathrm{int}(A)$$, $$\mathrm{int}(\overline{A})$$, $$\overline{\mathrm{int}(A)}$$ are all distinct.

_Solution._

(i) Let $$x\in A$$. In order for $$x\in\overline{B}$$, all open subsets containing $$x$$ must intersect $$B$$. However, since $$A$$ is a valid neighborhood of $$x$$ and $$A\cap B=\emptyset$$, it must be that $$x\not\in\overline{B}$$. Therefore $$A\cap\overline{B}=\emptyset$$.

To show that $$\overline{A}\cap\overline{B}$$ may not be empty, we use the following counterexample.

Let $$X=\mathbb{R}$$ be equipped with the usual topology, $$A=(0,1)$$ and $$B=(1,2)$$. Then $$\overline{A}=[0,1]$$ and $$\overline{B}=[1,2]$$ are the closures of $$A$$ and $$B$$, and $$\overline{A}\cap\overline{B}=\{1\}\ne\emptyset$$.

(ii)
* We first prove that if $$A\subset B$$, then $$\mathrm{int}(A)\subset\mathrm{int}(B)$$. Let $$x\in\mathrm{int}(A)$$, then by definition $$x$$ belongs to an open subset $$C$$ such that $$x\in C\subset A$$. But since $$A\subset B$$, this subset $$C$$ is also contained in $$B$$. Hence, $$x\in\mathrm{int}(B)$$ by the definition of the interior, and $$\mathrm{int}(A)\subset\mathrm{int}(B)$$ as desired.
    * Tutorial 3.1.a states that if $$A\subset B$$ then $$\overline{A}\subset\overline{B}$$. Applying this with the above-proved result yields $$\mathrm{int}(\overline{A})\subset\mathrm{int}(\overline{B})$$.  
    * Since $$\mathrm{int}(A)\subset\mathrm{int}(B)$$, applying the result of tutorial 3.1.a yields $$\overline{\mathrm{int}(A)}\subset\overline{\mathrm{int}(B)}$$.
* Let $$x\in A$$, then since $$A\subset\overline{A}$$ we have $$x\in\overline{A}$$ as well. Furthermore, as $$A$$ is an open set contained in $$\overline{A}$$ and $$x\in A$$, $$x$$ must belong to the interior of $$\overline{A}$$. Hence $$A\subset\mathrm{int}(\overline{A})$$.
* As $$\mathrm{int}(A)\subset A$$, we apply the result of tutorial 3.1.a to get $$\overline{\mathrm{int}(A)}\subset\overline{A}$$. But $$A$$ is given to be closed, so $$\overline{A}=A$$ and we get the desired result of $$\overline{\mathrm{int}(A)}\subset A$$.

(iii) Let $$A=[0,1)\cup(1,2]\cup\{3\}\subset\mathbb{R}$$, then:
* $$\overline{A}=[0,2]\cup{3}$$,
* $$\mathrm{int}(A)=(0,1)\cup(1,2)$$,
* $$\mathrm{int}(\overline{A})=(0,2)$$,
* $$\overline{\mathrm{int}(A)}=[0,2]$$.

This is one such example where $$A$$, $$\overline{A}$$, $$\mathrm{int}(A)$$, $$\mathrm{int}(\overline{A})$$ and $$\overline{\mathrm{int}(A)}$$ are all distinct.

{: .highlight}
> **Problem 3.**
> Given a subset $$A\subset\mathbb{R}$$, we consider the associated subbasis
>
> $$\mathcal{S}_A=\{(-\infty, a)|a\in A\}\cup\{(a,\infty)|a\in A\},$$
>
> and we denote by $$\mathcal{T}_A$$ the topology generated by $$\mathcal{S}_A$$.
>
> (i) Describe explicitly a basis for the topology $$\mathcal{T}_A$$.
>
> (ii) Show that $$\mathcal{T}_A$$ is always contained in the usual topology $$\mathcal{T}_{\mathrm{usual}}$$ on $$\mathbb{R}$$, i.e. $$\mathcal{T}_A\subseteq \mathcal{T}_{\mathrm{usual}}$$.
>
> (iii) Determine necessary and sufficient conditions on $$A$$ for $$\mathcal{T}_A$$ to coincide with the usual topology $$\mathcal{T}_{\mathrm{usual}}$$ on $$\mathbb{R}$$, i.e. $$\mathcal{T}_A=\mathcal{T}_{\mathrm{usual}}$$.
>
> (iv) For which $$A$$ is $$\mathcal{T}_A$$ Hausdorff?
>
> (v) Let
>
> $$A=\mathbb{Z}\cup\left\{\frac{1}{n}\middle|n\in\mathbb{N}\right\}\subset\mathbb{R}.$$
>
> * Describe explicitly the topology $$\mathcal{T}_A$$ as well as a basis for it.
>
> * Study the convergence of the sequence $$x_n=\frac{1}{n}$$ in this topology.
>
> * Study the convergence of the sequence $$x_n=-\frac{1}{n}$$ in this topology.

_Solution._