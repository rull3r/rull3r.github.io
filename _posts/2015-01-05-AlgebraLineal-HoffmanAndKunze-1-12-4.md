---
layout: post
title: Solución Cap$:$ 1, Sec$:$1.2, Ejercicio$:$ 4
subtitle: Algebra Lineal | Hoffman - Kunze | 2º Edición | Español
gh-repo: rull3r/Solucionario-AlgebraLineal-HoffmanAndKunze
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, algebra lineal,cuerpo, numeros complejos]
full-width: true
comments: true
---

<div class="box-note">
	Sea $F$ el cuerpo de los números complejos. ¿Son equivalentes los dos sistemas de ecuaciones lineales siguiente? Si es así. expresar cada ecuación de cada sistema como combinación lineal del otro. Tal y como en el problema anterior -> <a href="../2015-01-04-AlgebraLineal-HoffmanAndKunze-1-12-2">Ejercicio 2</a>.

$$\begin{align}
\left\lbrace\begin{aligned}
2x_1+\left(-1+i\right)x_2+x_4&=0\\
3x_2+2ix_3+5x_4&=0
\end{aligned}\right.
\quad\quad
\left\lbrace\begin{aligned}
\left(1+\frac{i}{2}\right)x_1+8x_2-ix_3-x_4&=0\\
\frac{2}{3}x_1-\frac{1}{2}x_2+x_3+7x_4&=0
\end{aligned}\right.
\end{align}$$
    
</div>

### Solucion


Para la ecuación 1 del sistema 1 hacemos $2x_1+\left(-1+i\right)x_2+x_4=a\left(\left(1+\frac{i}{2}\right)x_1+8x_2-ix_3-x_4\right)+b\left(\frac{2}{3}x_1-\frac{1}{2}x_2+x_3+7x_4\right)$

Despues de hacer algunas operaciones aritmeticas nos topamos con el siguiente sistema de ecuaciones

$$
\begin{align}
\begin{aligned}
2&= a  + \dfrac{ai}{2} + \dfrac{2b}{3}\\
-1+i&=8a-\dfrac{b}{2}\\
0&=ai+b\\
1&=-a+7b
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

de la tercera ecuacion del sistema concluimos que $-ai = b$. Pero al sustituir en la cuarta ecuacion del sistema tenemos que

$$1 = -a - 7ai \quad \implies \quad a=-\frac{1}{50}+i\frac{7}{50} \quad \implies \quad b=\frac{7}{50}+i\frac{1}{50}$$ 

estas soluciones no satisfacen la segunda ecuacion del sistema ya que 

$$ 8\left(-\frac{1}{50}+i\frac{7}{50}\right)-\dfrac{\frac{7}{50}+i\frac{1}{50}}{2} = -\frac{23}{100}+i\frac{111}{100} \neq -1+i$$

Concluimos que los dos sistemas de ecuaciones no son equivalentes
