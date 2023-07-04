---
layout: post
title: Solución Cap$:$ 1, Ejercicio$:$ 1
subtitle: Bayesian Statistical Methods | Brian J. Reich - Sujit K. Ghosh | 1st Edición | Ingles
gh-repo: rull3r/Solucionario-Bayesatistical-ReichGhosh
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,calculo,integral,derivada, probabilidad, bayes]
full-width: true
comments: true
---

<div class="box-note">
Si $X$ tiene como soporte $X \in S = [1,\infty]$, entonctrar el valor de la constante $c$ (como una funcion de $\theta$) que haga que $$f(x)=c e^\left(\frac{-x}{\theta}\right)$$

sea una función de densidad de probabilidad valida.
</div>


$$\begin{align}
1&=\int_{1}^{\infty} ce^{-\frac{x}{\theta}} \, dx \\ 
&= \lim_{a \to \infty}\left(	\int_{1}^{a} c \cdot e^{-\frac{1}{\theta} \cdot x} \, dx \right) \quad \text{(la $c$ sale de la integral y del limite)}\\
&= c\lim_{a \to \infty} \left(-\theta \cdot e^{-\frac{1}{\theta} \cdot x} \bigg|_{1}^{\infty}\right) \quad \text{(integramos y evaluamos en los extremos)} \\
&= c\lim_{a \to \infty} \left(-\theta \cdot \left(e^{-\frac{1}{\theta} \cdot a} - e^{-\frac{1}{\theta} \cdot 1}\right)\right)  \quad \text{(evaluamos el limite)} \\
&= -c\cdot\theta \cdot (0 - e^{-\frac{1}{\theta}}) \\
&= c\cdot\theta \cdot \left(e^{-\frac{1}{\theta}} - 0\right) \\
1&= c\cdot\theta \cdot e^{-\frac{1}{\theta}}
\end{align}$$

finalmente despejamos c de la ultima ecuacion y tendremos que el valor buscado es 

$$c= \dfrac{e^{\frac{1}{\theta}}}{\theta} $$

