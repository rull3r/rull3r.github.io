---
layout: post
title: Solución Cap$:$ 1, Sec$:$1.2, Ejercicio$:$ 5
subtitle: Algebra Lineal | Hoffman - Kunze | 2º Edición | Español
gh-repo: rull3r/Solucionario-AlgebraLineal-HoffmanAndKunze
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, algebra lineal,cuerpo, numeros complejos,binario]
full-width: true
comments: true
---

<div class="box-note">
Sea F un conjunto que contiene exactamente dos elementos, 0 y 1. Se define una adición
y multiplicación por las tablas:

$$
\begin{array}{c|cc}
+ & 0 & 1 \\ \hline
0 & 0 & 1 \\
1 & 1 & 0 \\
\end{array}
\quad\quad
\begin{array}{c|cc}
\times & 0 & 1 \\ \hline
0 & 0 & 0 \\
1 & 0 & 1 \\
\end{array}$$

Verificar que el conjunto F, juntamente con estas dos operaciones, es un cuerpo.
    
</div>

### Solucion

1. **Conmutatividad de la adición**:
   - Una operación es conmutativa si la tabla muestra simetría a lo largo de la diagonal que va desde la esquina superior izquierda hasta la esquina inferior derecha. Esto se aprecia en la tabla de adición. 
   
	- **Caso trivial 1**: $0 + 0 = 0$
	- **Caso trivial 2**: $1 + 1 = 0$
	- **Caso no trivial 1**: $0 + 1 = 1$
	- **Caso no trivial 2**: $1 + 0 = 1$

   Por lo que podemos afirmar que la adición es conmutativa.

2. **Asociatividad de la adición**:
   - Existen ocho casos posibles. Sin embargo, si $x = y = z = 0$ o $x = y = z = 1$, la conclusión es evidente. Así, vemos los siguientes casos:

   - **Caso trivial 1**: $(0 + 0) + 0 = 0 + (0 + 0)$
   - **Caso trivial 2**: $(1 + 1) + 1 = 1 + (1 + 1)$
   - **Caso no trivial 1**: $(0 + 1) + 0 = 0 + (1 + 0)$
   - **Caso no trivial 2**: $(1 + 0) + 0 = 1 + (0 + 0)$
   - **Caso no trivial 3**: $(0 + 0) + 1 = 0 + (0 + 1)$
   - **Caso no trivial 4**: $(1 + 1) + 0 = 1 + (1 + 0)$
   - **Caso no trivial 5**: $(0 + 1) + 1 = 0 + (1 + 1)$
   - **Caso no trivial 6**: $(1 + 0) + 1 = 1 + (0 + 1)$
   
   Por lo tanto, podemos concluir que la adición es asociativa.

3. **Elemento neutro de la adición**:
   - Al examinar la tabla de adición, observamos que el elemento identificado como 0 efectivamente actúa como un elemento neutro, ya que no altera el resultado cuando se suma a otro elemento.

4. **Inverso aditivo**:
   - La suma de 1 y 1 resulta en 0, lo que implica que el inverso aditivo de 1 es 1. De manera similar, la suma de 0 y 0 es 0, indicando que el inverso aditivo de 0 es 0. En términos simples, $-1 = 1$ y $-0 = 0$, lo que significa que cada elemento tiene un inverso aditivo.

5. **Conmutatividad de la multiplicación**:
   - Como se explicó anteriormente, una operación es conmutativa si la tabla muestra simetría a lo largo de la diagonal que va desde la esquina superior izquierda hasta la esquina inferior derecha. Esto se cumple en la tabla de multiplicación, lo que confirma que la multiplicación es conmutativa.

6. **Asociatividad de la multiplicación**:
   - Al igual que con la adición, hay ocho casos a considerar. Si $x = y = z = 1$, la conclusión es clara. Todos los casos son:

   - Caso trivial 1: $(0 \cdot 0) \cdot 0 = 0 \cdot (0 \cdot 0)$
   - Caso trivial 2: $(1 \cdot 1) \cdot 1 = 1 \cdot (1 \cdot 1)$
   - Caso no trivial 1: $(0 \cdot 1) \cdot 0 = 0 \cdot (1 \cdot 0)$
   - Caso no trivial 2: $(1 \cdot 0) \cdot 0 = 1 \cdot (0 \cdot 0)$
   - Caso no trivial 3: $(0 \cdot 0) \cdot 1 = 0 \cdot (0 \cdot 1)$
   - Caso no trivial 4: $(1 \cdot 1) \cdot 0 = 1 \cdot (1 \cdot 0)$
   - Caso no trivial 5: $(0 \cdot 1) \cdot 1 = 0 \cdot (1 \cdot 1)$
   - Caso no trivial 6: $(1 \cdot 0) \cdot 1 = 1 \cdot (0 \cdot 1)$

   Por lo tanto, podemos afirmar que la multiplicación es asociativa.

7. **Elemento neutro de la multiplicación**:
   - Al analizar la tabla de multiplicación, notamos que el elemento identificado como 1 actúa como un elemento neutro, ya que no altera el resultado cuando se multiplica por otro elemento.

8. **Inverso multiplicativo**:
   - Dado que solo hay un elemento distinto de cero, que es 1, y $1 \cdot 1 = 1$, concluimos que 1 tiene un inverso multiplicativo. En otras palabras, $1^{-1} = 1$.

9. **Distributividad de la multiplicación respecto a la adición**:
   - Se pueden considerar ocho casos posibles. Si $x = 0$, ambos lados de la igualdad son claramente iguales a cero, cubriendo así cuatro casos. Si $x = y = z = 1$, la conclusión es evidente. Por lo tanto, nos quedan tres casos. Si $x = 1$ y $y = z = 0$, ambos lados son cero. Finalmente, quedan dos casos donde $x = 1$ y uno de $y$ o $z$ es igual a 1 y el otro es igual a 0. En ambos casos, ambos lados son iguales a 1. Por lo tanto, se cumple la igualdad $x(y + z) = (x + y)z$ en los ocho casos.


por lo tanto F es un cuerpo