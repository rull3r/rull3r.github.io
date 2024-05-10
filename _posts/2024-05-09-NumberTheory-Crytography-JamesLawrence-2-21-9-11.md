---
layout: post
title: Solución Cap$:$ 2, Sec$:$2.1, Ejercicios$:$ 9 al 11
subtitle: An Introduction to Number Theory with Cryptography |  James Kraft - Lawrence Washington | 2º Edición | Ingles
gh-repo: rull3r/Solucionario-NumberTheory-Crytography-JamesLawrence
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,latex,libro, crypto, criptografica ,algebra abstracta, divisibilidad, numeros, teoria de numeros]
comments: true
---


<div class="box-note">
9) Probar o proporcionar un contraejemplo para las siguientes afirmaciones:
<ol>
    <li value = "a)">Si $6 \nmid a$ y $6 \nmid b$, entonces $6 \nmid ab$.</li>
    <li value = "b)">Si $6 \nmid a$ y $6 \nmid b$, entonces $36 \nmid ab$.</li>
    <li value = "c)">Si $6 \nmid a$ y $6 \nmid b$, entonces $6 \nmid (a + b)$.</li>
</ol>
</div>
<ol>
    <li value="a)">
    Falso: Tomemos $a = 2$ y $b = 3$. Como $6 \nmid 2$ y $6 \nmid 3$, pero $6 \mid (2 \cdot 3)$, la afirmación es falsa.
    </li><br>
    <li value="b)">
    Falso: Tomemos $a = 9$ y $b = 4$. Como $6 \nmid 9$ y $6 \nmid 4$, pero $36 \mid (9 \cdot 4)$, la afirmación es falsa.
    </li><br>
    <li value="c)">
    Falso: Tomemos $a = 1$ y $b = 5$. Como $6 \nmid 1$ y $6 \nmid 5$, pero $6 \mid (1 + 5)$, la afirmación es falsa.
    </li>
</ol>
<div class="box-note">
10) Probar o proporcionar un contraejemplo para las siguientes afirmaciones:
<ol>
    <li value = "a)">Si $6 \mid a$ y $6 \mid b$, entonces $6 \mid ab$.</li>
    <li value = "b)">Si $6 \mid a$ y $6 \mid b$, entonces $36 \mid ab$.</li>
</ol>
</div>
<ol>
    <li value="a)">
    Por defincion tenemos que $a = 6d$ y $b = 6f$, donde $d$ y $f$ son enteros. Entonces, $ab = (6d)(6f) = 6(6df)$. Dado que $6df$ es un entero, $ab$ es divisible por 6.
    </li><br>
    <li value="b)">
    Por defincion tenemos que $a = 6d$ y $b = 6f$, donde $d$ y $f$ son enteros. Entonces, $ab = (6d)(6f) = 36(df)$. Dado que $df$ es un entero, $ab$ es divisible por 36.
    </li>
</ol>

<div class="box-note">
11) Probar o proporcionar un contraejemplo para las siguientes afirmaciones:
<ol>
    <li value = "a)">Si $c \mid a$ y $c \mid b$, entonces $c \mid ab$.</li>
    <li value = "b)">Si $c \mid a$ y $c \mid b$, entonces $c^2 \mid ab$.</li>
    <li value = "c)">Si $c \nmid a$ y $c \nmid b$, entonces $c \nmid (a + b)$.</li>
</ol>
</div>

<ol>
    <li value="a)">
    Por definición, si $c\mid a$, entonces $a = cd$ para algún entero $d$, y si $c\mid b$, entonces $b = cf$ para algún entero $f$.
    Entonces, $ab = (cd)(cf) = c(cdf)$.
    Como $cdf$ es un entero, $c$ divide a $ab$, por lo tanto $c \mid ab$. siempre que  $c\neq0$ obviamente
    </li><br>
    <li value="b)">
    Por definición, si $c\mid a$, entonces $a = cd$ para algún entero $d$, y si $c\mid b$, entonces $b = cf$ para algún entero $f$.
    Entonces, $ab = (cd)(cf) = c^2df$.
    Como $df$ es un entero, $c^2$ divide a $ab$, por lo tanto $c^2 \mid ab$. siempre que  $c\neq0$ obviamente   
    </li><br>
    <li value="c)">
    Es falso. Tomemos $a = 1$, $b = 5$ y $= 6$. Como $6 \nmid 1$ y $6 \nmid 5$, pero $6 \mid (1 + 5)$, la afirmación es falsa. como en el ejercicio 9
    </li>
</ol>





