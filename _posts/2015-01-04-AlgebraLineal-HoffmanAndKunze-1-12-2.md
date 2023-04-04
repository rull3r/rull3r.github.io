---
layout: post
title: Solución Cap$:$ 1, Sec$:$1.2, Ejercicio$:$ 2
subtitle: Algebra Lineal | Hoffman - Kunze | 2º Edición | Español
gh-repo: rull3r/Solucionario-AlgebraLineal-HoffmanAndKunze
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, algebra lineal,cuerpo, numeros complejos]
comments: true
---

<div class="box-note">
  Sea $F$ el cuerpo de los números complejos. ¿Son equivalentes los dos sistemas de ecuaciones lineales siguiente? Si es así. expresar cada ecuación de cada sistema como combinación lineal del otro.

$$\begin{align}
\left\lbrace\begin{aligned}
x_1-x_2=0 \\
2x_1+x_2=0
\end{aligned}\right.
\quad\quad
\left\lbrace\begin{aligned}
3x_1+x_2=0 \\
x_1+x_2=0
\end{aligned}\right.
\end{align}$$
</div>

### Solucion


Para la ecuación 1 del sistema 1 hacemos $x_1-x_2=a(3x_1+x_2)+b(x_1+x_2)$

$$\begin{align}
\begin{aligned}
1&= 3a+b \\
-1&=a+b
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&= 1 \\
b&= -2
\end{aligned}
\end{align}$$

de modo que $x_1-x_2=1(3x_1+x_2)-2(x_1+x_2)$

<hr>
Para la ecuación 2 del sistema 1 hacemos $2x_1+x_2=a(3x_1+x_2)+b(x_1+x_2)$

$$\begin{align}
\begin{aligned}
2&= 3a+b \\
1&=a+b
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&=\frac{1}{2} \\
b&= \frac{1}{2}
\end{aligned}
\end{align}$$

de modo que $2x_1+x_2=\frac{1}{2}(3x_1+x_2)+\frac{1}{2}(x_1+x_2)$
<hr>
Para la ecuación 1 del sistema 2 hacemos $3x_1+x_2=a(x_1-x_2)+b(2x_1+x_2)$

$$\begin{align}
\begin{aligned}
3&= a+2b \\
1&=-a+b
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&=\frac{1}{3} \\
b&= \frac{4}{3}
\end{aligned}
\end{align}$$

de modo que $3x_1+x_2=\frac{1}{3}(x_1-x_2)+\frac{4}{3}(2x_1+x_2)$
<hr>
Para la ecuación 2 del sistema 2 hacemos $x_1+x_2=a(x_1-x_2)+b(2x_1+x_2)$

$$\begin{align}
\begin{aligned}
1&= a+2b \\
1&=-a+b
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&=\frac{-1}{3} \\
b&= \frac{2}{3}
\end{aligned}
\end{align}$$

de modo que $x_1+x_2=\frac{-1}{3}(x_1-x_2)+\frac{2}{3}(2x_1+x_2)$

Finalmente los dos sistemas de ecuaciones son equivalentes.

