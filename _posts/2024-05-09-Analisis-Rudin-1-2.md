---
layout: post
title: Solución Cap$:$ 1, Ejercicio$:$ 2
subtitle: Principios de Análisis Matemático |  Walter Rudin | 1º Edición | Español
gh-repo: rull3r/Solucionario-Analisis-Rudin
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, algebra lineal,cuerpo, numeros complejos]
full-width: true
comments: true
---

<div class="box-note">
	Demostrar que no existe ningún numero racional que su cuadrado sea $12$.
</div>

### Solucion

Procederemos por reducción al absurdo. Suponemos que sí existe ese numero racional, sea $x=\sqrt{12}=\frac{a}{b}$, es decir, $12=\frac{a^2}{b^2}\Rightarrow12b^2=a^2$, $a^2$ no puede ser impar ya que $12b^2=a^2$ con $b=2s+1$ y $a=2t+1$ tenemos $12(4s^2+4s+1)=4t^2+4t+1\Rightarrow -48s^2-48s+4t^2+4t=11\Rightarrow 4(-12s^2-12s+t^2+t)=11$ lo cual es una contradicción porque 11 es primo.<br><br>
Si $a^2$ es par entonces $a=2k\Rightarrow a^2=4k^2$ luego $4k^2=12b^2\Rightarrow k^2=3b^2$ si $k^2$ es impar $b^2$ también es impar, esto es $k=2y+1$ y $b=2w+1$ entonces $4y^2+4y+1=3(4w^2+4w+1)\Rightarrow 4y^2+4y+1=12w^2+12w+3$ finalmente $4(y^2+y-3w^2-3w)=2$ lo cual es una contradicción porque 2 no es múltiplo de 4
