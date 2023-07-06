---
layout: post
title: Solución Cap$:$ 1, Ejercicio$:$ 1
subtitle: Machine Learning - A Bayesian and Optimization Perspective  | Sergios Theodoridis  | 2nd Edición | Ingles
gh-repo: rull3r/Solucionario-BayesianOptimizationPerspective-Sergios
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,calculo,integral,derivada, probabilidad, bayes,media,varianza,distribucion,binomial,uniforme]
full-width: true
comments: true
---

<div class="box-note">
	Deriva la media y la varianza para la distribución binomial
</div>

### Solucion

Una variable aleatoria $x$ se dice que sigue una distribucion binomial con parametros $n$, $p$ lo que escribimos como $x\sim$Bin($x\|n,p$), si $\mathcal{X}=$\{$ 0,1,\dots,n $\} y

$$p(x=k) :=\text{Bin}(k|n,p) = \binom{n}{k} p^k(1-p)^{n-k}, \quad\quad k = 0,1,\dots,n$$

sabiendo que 

$$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

Para calcular la media usamos la esperanza, en un punto de la demostracion nos apoyaremos en el [Teorema del Binomio](https://es.wikipedia.org/wiki/Teorema_del_binomio)

$$\begin{align}
\mathbb{E}(x)&=\sum_{k=0}^n kP(k) \\
&=\sum_{k=0}^n kP(k) \\
&=\sum_{k=0}^n k\binom{n}{k} p^k(1-p)^{n-k} \\
&=\sum_{k=0}^n k\frac{n!}{k!(n-k)!} p^k(1-p)^{n-k}\quad \text{(el primer elemento es 0)} \\ 
&=\sum_{k=1}^n k\frac{n!}{k!(n-k)!} p^k(1-p)^{n-k} \\
&= \frac{n!}{(n-1)!} p(1-p)^{n-1}+2\frac{n!}{2!(n-2)!} p^2(1-p)^{n-2}+3\frac{n!}{3!(n-3)!} p^3(1-p)^{n-3}+\cdots+ n\frac{n!}{n!(n-n)!} p^n(1-p)^{n-n}\\
&\text{Primero simplificamos los factoriales}\\
&= np(1-p)^{n-1}+\frac{n(n-1)}{1!} p^2(1-p)^{n-2}+\frac{n(n-1)(n-2)}{2!} p^3(1-p)^{n-3}+\cdots+ np^n\\
&\text{sacamos factor comun $np$}\\
&= np\left((1-p)^{n-1}+\frac{(n-1)}{1!} p(1-p)^{n-2}+\frac{(n-1)(n-2)}{2!} p^2(1-p)^{n-3}+\cdots+ p^{n-1}\right)\\
&\text{finalmente usamos el Teorema del Binomio}\\
&= np\left((1-p)+p\right)^{n-1}\\
\mathbb{E}(x)&= np\\
\end{align}$$

Para calcular la varianza usamos la esperanza calculada anteriormente,

$$\begin{align}
\sigma_X^2&=\mathbb{E}(x^2) - \mathbb{E}(x)^2 \\
&=\mathbb{E}(x^2) - (np)^2 \\
&=\sum_{k=0}^n k^2P(k) - (np)^2 \\
&=\sum_{k=0}^n k^2\binom{n}{k} p^k(1-p)^{n-k} - (np)^2 \\
&=\sum_{k=0}^n k^2\frac{n!}{k!(n-k)!} p^k(1-p)^{n-k} - (np)^2\quad \text{(el primer elemento es 0)} \\ 
&=\sum_{k=1}^n k^2\frac{n!}{k!(n-k)!} p^k(1-p)^{n-k} - (np)^2 \\
&\text{sacando factor comun $np$ mas directamente y simplificar $k$ }\\
&= np\left(\sum_{k=1}^n(k)\frac{(n-1)!}{(k-1)!(n-k)!}p^{k-1}(1-p)^{n-k}\right) - (np)^2\\
&= \frac{n!}{(n-1)!} p(1-p)^{n-1}+2^2\frac{n!}{2!(n-2)!} p^2(1-p)^{n-2}+3^2\frac{n!}{3!(n-3)!} p^3(1-p)^{n-3}+\cdots+ n^2\frac{n!}{n!(n-n)!} p^n(1-p)^{n-n} - (np)^2\\
&\text{Primero simplificamos los factoriales}\\
&= np(1-p)^{n-1}+2\frac{n(n-1)}{1!} p^2(1-p)^{n-2}+3\frac{n(n-1)(n-2)}{2!} p^3(1-p)^{n-3}+\cdots+ n^2p^n  - (np)^2 \\
&= np\left((1-p)^{n-1}+2\frac{(n-1)}{1!} p(1-p)^{n-2}+3\frac{(n-1)(n-2)}{2!} p^2(1-p)^{n-3}+\cdots+ np^{n-1}\right) - (np)^2\\
&= np\left(\sum_{k=1}^n(k)\frac{(n-1)!}{(k-1)!(n-k)!}p^{k-1}(1-p)^{n-k}\right) - (np)^2\\
\end{align}$$