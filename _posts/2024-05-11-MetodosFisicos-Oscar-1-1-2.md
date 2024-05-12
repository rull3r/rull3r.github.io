---
layout: post
title: Solución Cap$:$ 1, Sec$:$1.1, Ejercicio$:$ 2
subtitle: Métodos Matemáticos de la Física |  Oscar Reula | 1º Edición | Español
gh-repo: rull3r/Solucionario-MetodosFisicos-Oscar
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,fisica,algebra,topologia,conjuntos, cuerpo,fisica, metodos]
full-width: true
comments: true
---

<div class="box-note">
	Prueba que el espacio métrico $(X,d)$ posee una topología inducida por su métrica.
</div>

Un espacio métrico $(X,d)$ con $X$ un conjunto de puntos y $d:X\times X \longrightarrow \mathbb{R}$ que satisface las siguientes propiedades:

<ol>
    <li value="i)">$d(x,x')=0\Leftrightarrow x=x'$</li>
    <li value="ii)">$d(x,x')=d(x',x)$</li>
    <li value="iii)">$d(x,x')+d(x',x'')\geq d(x,x'')$</li>
</ol>

Luego, sea $\tau_d=\left\lbrace O \mid \forall x \in O, \exists \beta_d(x,r)\subset B \colon \beta_d(x,r)\subset O \right\rbrace $ donde $B$ es el conjunto de todos abiertos en $X$ y $\beta_d(x,r)$ es una bola abierta bajo la métrica $d$, solo resta demostrar las siguientes propiedades:

<ol>
    <li value="1)">Como $X$ y $\emptyset$ son abiertos, entonces están en $\tau_d$.</li><br>
    <li value="2)">Sea $O_i$ una familia de subconjuntos abiertos arbitraria de $O$ y sea $O'=\bigcup_iO_i$. Si $O'=\emptyset$, entonces $O'$ está en $\tau_d$. Si $O'\neq\emptyset$, sea $x\in O_i$ para algún $i$ y como $O_i\subset O$, entonces $\exists\beta_d(x,r)\subset O_i$ por lo tanto $\beta_d(x,r)\subset O'$, luego $O'$ está en $\tau_d$.</li><br>
    <li value="3)">Sean $O_1, O_2$ dos subconjuntos cualesquiera de $O$, sea $x\in O_1\cap O_2$, entonces $\exists\beta_d(x,r_1)\subset O_1$ y $\exists\beta_d(x,r_2)\subset O_2$ con $r=\min \{r_1,r_2\}$ tendremos que $\beta_d(x,r)\subseteq \beta_d(x,r_1)$ y $\beta_d(x,r)\subseteq \beta_d(x,r_2)$, por lo tanto $\beta_d(x,r)\subseteq O_1\cap O_2$. Esto demuestra que la intersección está en $\tau_d$, de modo que $\tau_d$ es la topología inducida por la métrica $d$.</li>
</ol>


