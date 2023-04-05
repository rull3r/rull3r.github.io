---
layout: post
title: Solución Cap$:$ 1, Sec$:$1.2, Ejercicio$:$ 3
subtitle: Algebra Lineal | Hoffman - Kunze | 2º Edición | Español
gh-repo: rull3r/Solucionario-AlgebraLineal-HoffmanAndKunze
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, algebra lineal,cuerpo, numeros complejos]
comments: true
---

<div class="box-note">
	Sea $F$ el cuerpo de los números complejos. ¿Son equivalentes los dos sistemas de ecuaciones lineales siguiente? Si es así. expresar cada ecuación de cada sistema como combinación lineal del otro. Tal y como en el problema anterior -> <a href="../2015-01-04-AlgebraLineal-HoffmanAndKunze-1-12-2">Ejercicio 2</a>.

$$\begin{align}
\left\lbrace\begin{aligned}
-x_1+x_2+4x_3=0\\
x_1+3x_2+8x_3=0\\
\frac{1}{2}x_1+x_2+\frac{5}{2}x_3=0
\end{aligned}\right.
\quad\quad
\left\lbrace\begin{aligned}
x_1-x_3=0\\
x_2+3x_3=0
\end{aligned}\right.
\end{align}$$
    
</div>




Para la ecuación 1 del sistema 1 hacemos $-x_1+x_2+4x_3=a(x_1-x_3)+b(x_2+3x_3)$

$$
\begin{align}
\begin{aligned}
-1&= a \\
1&=b	\\
4&=-a+3b
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&= -1 \\
b&= 1
\end{aligned}
\end{align}
$$

de modo que $-x_1+x_2+4x_3=-(x_1-x_3)+(x_2+3x_3)$

<hr>
Para la ecuación 2 del sistema 1 hacemos $x_1+3x_2+8x_3=a(x_1-x_3)+b(x_2+3x_3)$

$$
\begin{align}
\begin{aligned}
1&= a \\
3&= b	\\
8&= -a+3b
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&=1 \\
b&= 3
\end{aligned}
\end{align}
$$

de modo que $x_1+3x_2+8x_3=(x_1-x_3)+3(x_2+3x_3)$

<hr>

Para la ecuación 3 del sistema 1 hacemos $\frac{1}{2}x_1+x_2+\frac{5}{2}x_3=a(x_1-x_3)+b(x_2+3x_3)$

$$
\begin{align}
\begin{aligned}
\frac{1}{2}&= a \\
1&= b	\\
\frac{5}{2}&= -a+3b
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&=\frac{1}{2} \\
b&= 1
\end{aligned}
\end{align}
$$

de modo que $\frac{1}{2}x_1+x_2+\frac{5}{2}x_3=\frac{1}{2}(x_1-x_3)+(x_2+3x_3)$

<hr>

Para la ecuación 1 del sistema 2 hacemos $x_1-x_3=a(-x_1+x_2+4x_3)+b(x_1+3x_2+8x_3)+c(\frac{1}{2}x_1+x_2+\frac{5}{2}x_3)$

$$
\begin{align}
\begin{aligned}
1&= -a+b+\frac{c}{2} \\
0 &=	a+3b+c	\\
-1&=4a+8b+\frac{5}{2}c
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&=-\frac{3}{4} \\
b&=\frac{1}{4}	\\
c&=0
\end{aligned}
\end{align}
$$

de modo que $x_1-x_3=-\frac{3}{4}(-x_1+x_2+4x_3)+\frac{1}{4}(x_1+3x_2+8x_3)+c(\frac{1}{2}x_1+x_2+\frac{5}{2}x_3)$  $\Rightarrow$  $x_1-x_3=-\frac{3}{4}(-x_1+x_2+4x_3)+\frac{1}{4}(x_1+3x_2+8x_3)$
        
<hr>

Para la ecuación 2 del sistema 2 hacemos $x_2+3x_3=a(-x_1+x_2+4x_3)+b(x_1+3x_2+8x_3)+c(\frac{1}{2}x_1+x_2+\frac{5}{2}x_3)$

$$
\begin{align}
\begin{aligned}
0&= -a+b+\frac{c}{2} \\
1 &=	a+3b+c	\\
1&=4a+8b+\frac{5}{2}c
\end{aligned}
\quad
\Rightarrow
\quad
\begin{aligned}
a&=\frac{1}{4} \\
b&=\frac{1}{4}	\\
c&=0
\end{aligned}
\end{align}
$$

de modo que $x_2+3x_3=\frac{1}{4}(-x_1+x_2+4x_3)+\frac{1}{4}(x_1+3x_2+8x_3)+0(\frac{1}{2}x_1+x_2+\frac{5}{2}x_3)$ $\Rightarrow$  $x_2+3x_3=\frac{1}{4}(-x_1+x_2+4x_3)+\frac{1}{4}(x_1+3x_2+8x_3)$

Finalmente los dos sistemas de ecuaciones son equivalentes.