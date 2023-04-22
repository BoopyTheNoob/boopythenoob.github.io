---
layout: default
title: Second Order Differential Equations
parent: MH1811 - Mathematics 2
nav_order: 12
---

# Second Order Differential Equations

{: .highlight}
Find the general solution of the following ordinary differential equation:
$$y''-16y=4x\cos x.$$

**Solution.** The associated homogeneous equation and its characteristic equation are

$$y''-16y=0,\,\lambda^2-16=0.$$

The characteristic equation has roots of
$$\lambda=4$$
and
$$\lambda=-4,$$
therefore the homogeneous equation's solution (with $$C_1$$ and $$C_2$$ are arbitrary constants) is

$$y_h(x)=C_1e^{4x}+C_2e^{-4x}.$$

Using undetermined coefficients, we guess the particular solution of this equation will have the form

$$y_p(x)=(Ax+B)\cos x+(Cx+D)\sin x.$$

Then its first- and second-order differential are

$$\begin{align*}
y_p'&=(A+Cx+D)\cos x+(C-Ax-B)\sin x\\
y_p''&=(2C-Ax-B)\cos x+(-2A-Cx-D)\sin x
\end{align*}$$

Substituting these to the original equation gives

$$\begin{align*}
&(2C-Ax-B-16(Ax+B))\cos x&\\
&+(-2A-Cx-D-16(Cx+D))\sin x=4x\cos x.\\
\Leftrightarrow&(-17A)x\cos x+(2C-17B)\cos x\\
&+(-17C)x\sin x+(-2A-17D)\sin x=4x\cos x.
\end{align*}$$

Therefore
$$\begin{cases}-17A=4\\2C-17B=0\\-17C=0\\-2A-17D=0\end{cases}\Leftrightarrow\begin{cases}A=-\dfrac{4}{17}\\B=0\\C=0\\D=\dfrac{8}{289}.\end{cases}$$

The general solution for the specified differential equation is therefore

$$y(x)=y_h(x)+y_p(x)=C_1e^{4x}+C_2e^{-4x}-\dfrac{4}{17}x\cos x+\dfrac{8}{289}\sin x.$$