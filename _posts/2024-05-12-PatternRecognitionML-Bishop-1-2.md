---
layout: post
title: Solución Cap$:$ 1, Ejercicio$:$ 2 ($\ast$)
subtitle: Pattern Recognition and Machine Learning |  Christopher M. Bishop | 1º Edición | Ingles
gh-repo: rull3r/Solucionario-PatternRecognitionML-Bishop
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, algebra lineal, estadistica, probabilidades, error, patrones, machine learning, deep learning]
full-width: true
comments: true
---

<div class="box-note">
Escriba el conjunto de ecuaciones lineales  análogas al <a href="https://rull3r.github.io/2015-01-10-PatternRecognitionML-Bishop-1-1/">ejercicio 1</a>, satisfechas por los coeficientes $w_i$ que minimizan la función de error de suma de cuadrados regularizada dada por:.

$$ E(w) = \dfrac{1}{2}\sum^N_{n=1} \left( y(x_n,w) -t_n\right)^2 + \dfrac{\lambda}{2}\lVert w \rVert^2$$  
</div>

### Solucion

Tenemos un problema de minimizacion asi que derivamos la funcion de error que depende de $w$ e igualamos a $0$:

$$
\begin{align}
E'(w)&=\left(\dfrac{1}{2}\sum^N_{n=1} \left( y(x_n,w) -t_n\right)^2 + \dfrac{\lambda}{2}\lVert w \rVert^2\right)'\\
&=\left(\dfrac{1}{2}\sum^N_{n=1} \left( y(x_n,w) -t_n\right)^2\right)' + \left(\dfrac{\lambda}{2}\lVert w \rVert^2\right)'\\
&=\sum^N_{n=1} \left( y(x_n,w) -t_n\right)x_n^i + \lambda \sum^M_{j=0} w_j\\
&= \sum^N_{n=1} \left( y(x_n,w)x_n^i -t_nx_n^i\right) + \lambda  \sum^M_{j=0} w_j\\ 
0&= \sum^N_{n=1} \left( y(x_n,w)x_n^i -t_nx_n^i\right) + \lambda \sum^M_{j=0} w_j
\end{align}
$$

Sustituimos ahora el polinimio $y(x_n,w)$ 

$$
\begin{align}
0&= \sum^N_{n=1} \left( \sum^M_{j=0}w_jx_n^jx_n^i -t_nx_n^i\right) + \lambda \sum^M_{j=0} w_j\\
&=  \sum^N_{n=1} \left( \sum^M_{j=0}w_jx_n^{j+i} -t_nx_n^i\right) + \lambda \sum^M_{j=0} w_j\\
&=  \sum^N_{n=1}\sum^M_{j=0}w_jx_n^{j+i} - \sum^N_{n=1}t_nx_n^i + \lambda \sum^M_{j=0} w_j\\
\sum^N_{n=1}\sum^M_{j=0}w_jx_n^{j+i} + \lambda \sum^M_{j=0} w_j &= \sum^N_{n=1}t_nx_n^i\\
\sum^M_{j=0}\sum^N_{n=1}x_n^{j+i}w_j + \lambda \sum^M_{j=0} w_j&= \sum^N_{n=1}t_nx_n^i\\
\sum^M_{j=0}\left(\sum^N_{n=1}\left(x_n^{j+i}w_j\right) + \lambda w_j\right)&= \sum^N_{n=1}t_nx_n^i
\end{align}
$$
