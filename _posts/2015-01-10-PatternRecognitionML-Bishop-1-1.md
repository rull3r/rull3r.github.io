---
layout: post
title: Solución Cap$:$ 1, Ejercicio$:$ 1 ($\ast$)
subtitle: Pattern Recognition and Machine Learning |  Christopher M. Bishop | 1º Edición | Ingles
gh-repo: rull3r/Solucionario-PatternRecognitionML-Bishop
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, algebra lineal, estadistica, probabilidades, error, patrones, machine learning, deep learning]
full-width: true
comments: true
---

<div class="box-note">
Sea la siguiente funcion de error de suma de cuadrados:

$$ E(w) = \dfrac{1}{2}\sum^N_{n=1} \left( y(x_n,w) -t_n\right)^2$$

donde $y(x_n,w)$ viene dada por

$$ y(x_n,w) = w_0+w_1x+w_2x^2 + \cdots + w_Mx^M = \sum^M_{j=0}w_jx^j $$

Demuestre que los coeficientes $w = \{w_i\}$ que minimizan esta función de error vienen dados por la solución del siguiente conjunto de ecuaciones lineales

$$ \sum^M_{j=0}A_{ij}w_j = T_i$$

donde

$$ A_{ij} = \sum^N_{n=1} (x_n)^{i+j}, \quad\quad\quad T_i=\sum^N_{n=1} (x_n)^it_n$$   
</div>

### Solucion

Tenemos un problema de minimizacion asi que derivamos la funcion de error que depende de $w$ e igualamos a $0$:


$$
\begin{align}
E'(w)&=\left(\dfrac{1}{2}\sum^N_{n=1} \left( y(x_n,w) -t_n\right)^2\right)'\\
&=\sum^N_{n=1} \left( y(x_n,w) -t_n\right)x_n^i\\
&= \sum^N_{n=1} \left( y(x_n,w)x_n^i -t_nx_n^i\right)\\
0&= \sum^N_{n=1} \left( y(x_n,w)x_n^i -t_nx_n^i\right)
\end{align}
$$

Sustituimos ahora el polinimio $y(x_n,w)$ 

$$
\begin{align}
0&= \sum^N_{n=1} \left( \sum^M_{j=0}w_jx_n^jx_n^i -t_nx_n^i\right)\\
&=  \sum^N_{n=1} \left( \sum^M_{j=0}w_jx_n^{j+i} -t_nx_n^i\right)\\
&=  \sum^N_{n=1}\sum^M_{j=0}w_jx_n^{j+i} - \sum^N_{n=1}t_nx_n^i\\
\sum^N_{n=1}\sum^M_{j=0}w_jx_n^{j+i}&= \sum^N_{n=1}t_nx_n^i\\
\sum^M_{j=0}\sum^N_{n=1}x_n^{j+i}w_j&= \sum^N_{n=1}t_nx_n^i\\
\end{align}
$$

Veamos la segunda derivada de la funcion del error:

$$
\begin{align}
E''(w)&= \left(\sum^N_{n=1} \left( y(x_n,w)x_n^i -t_nx_n^i\right)\right)'\\
&= \sum^N_{n=1}  x_n^ix_n^i\\
&=\sum^N_{n=1}  \left(x_n^i\right)^2
\end{align}
$$

Notamos que la segunda derivada es siempre positiva, pero ademas, $E''(w)$ es constante (no depende de $w$) por lo tanto el valor critico o cualquiero otro cero de la primera derivada de la funcion de error sera siempre un minimo