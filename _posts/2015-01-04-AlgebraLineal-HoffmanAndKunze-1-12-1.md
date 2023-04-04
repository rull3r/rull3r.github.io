---
layout: post
title: Solución Cap$:$ 1, Sec$:$1.2, Ejercicio$:$ 1
subtitle: Algebra Lineal | Hoffman - Kunze | 2º Edición | Español
gh-repo: rull3r/Solucionario-AlgebraLineal-HoffmanAndKunze
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, algebra lineal,cuerpo, numeros complejos]
full-width: true
comments: true
---

{: .box-note}
Verificar que el conjunto de los números complejos de la forma $x+iy\sqrt{2}$ con $x,y\in\mathbb{Q}$ es un subcuerpo de $\mathbb{C}$.

### Solucion
Procedemos a ver cada uno de los axiomas para comprobar que es un subcuerpo de $\mathbb{C}$ teniendo que $z_1=x_1+iy_1\sqrt{2}$ y que $z_2=x_2+iy_2\sqrt{2}$ con $x_1,x_2,y_1,y_2\in\mathbb{Q}$


<ol>
    <li value="i)">
    Con $x_1=y_1=0$, $z_1=0$ por lo tanto el $0$ esta en el conjunto.    
    </li><br>
    <li value="ii)">
    Con $x_1=1$ y $y_1=0$, $z_1=1$ por lo tanto el $1$ esta en el conjunto.   
    </li><br>
    <li value="iii)">
    $z_1+z_2=x_1+iy_1\sqrt{2}+x_2+iy_2\sqrt{2}=(x_1+x_2)+i(y_1+y_2)\sqrt{2}$ por lo tanto $z_1+z_2$ pertenece al conjunto.  
    </li><br>
    <li value="iv)">
    $-z_1$ esta en el conjunto ya que basta tomar $x_1$ y $y_1$ como negativos.
    </li><br>
    <li value="v)">
    Veamos que $z_1z_2$ pertenecen al conjunto

    $$\begin{align}
    z_1z_2&=(x_1+iy_1\sqrt{2})(x_2+iy_2\sqrt{2})\\
    &=x_1x_2+ix_1y_2\sqrt{2}+ix_2y_1\sqrt{2}+2y_1y_2\\
    &=(x_1x_2+2y_1y_2)+i(x_1y_2+x_2y_1)\sqrt{2}\\
    \end{align}$$
    </li><br>
    <li value="vi)">
    Veamos que $z_1^{-1}$ con $x_1,y_1\neq0$ pertenece al conjunto

    $$\begin{align}
    z_1^{-1}&=\left( \dfrac{1}{x_1+iy_1\sqrt{2}}\right) \left( \dfrac{x_1-iy_1\sqrt{2}}{x_1-iy_1\sqrt{2}}\right) \\
    &=\dfrac{x_1-iy_1\sqrt{2}}{\left(x_1+iy_1\sqrt{2} \right) \left( x_1-iy_1\sqrt{2}\right) }\\
    &=\dfrac{x_1-iy_1\sqrt{2}}{x_1^2+2y_1^2}\\
    &=\dfrac{x_1}{x_1^2+2y_1^2}+i\dfrac{-y_1}{x_1^2+2y_1^2}\sqrt{2}
    \end{align}$$
    </li>
</ol>

Luego el conjunto de los números complejos de la forma $x+iy\sqrt{2}$ con $x,y\in\mathbb{Q}$ es un subcuerpo de $\mathbb{C}$.