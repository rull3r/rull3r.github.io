---
layout: post
title: Solución Cap$:$ 1, Sec$:$1, Ejercicio$:$ 3
subtitle: Algebra Moderna |  I. N. Herstein | 2º Edición | Español
gh-repo: rull3r/Solucionario-AlgebraModerna-Herstein
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,latex,libro, algebra moderna ,algebra abstracta,conjuntos, grupos]
comments: true
---

<div class="box-note">

Pruébese que $A \cup  \left( B \cap C\right) = \left( A \cup B \right)  \cap \left( A \cup C\right) $.   

</div>

<ol>
    <li>
        <span style="font-size: 30px;">($\Rightarrow$)</span>
        Sea $x \in A \cup  \left( B \cap C\right)$ entonces $x \in A$ o $x \in B \cap C$. Si $x \in A$, entonces $x \in A \cup B$ y $x \in A \cup C$. Si $x \in B \cap C$, entonces $x \in B$ y $x \in C$, lo que implica que $x \in A \cup B$ y $x \in A \cup C$. Por lo tanto, $x \in (A \cup B) \cap (A \cup C)$.
    </li><br>
    <li>
        <span style="font-size: 30px;">($\Leftarrow$)</span>
    	Sea $x \in (A \cup B) \cap (A \cup C)$ entonces $x \in A \cup B$ y $x \in A \cup C$. Si $x \in A \cup B$, entonces $x \in A$ o $x \in B$. Si $x \in A$, entonces $x \in A \cup (B \cap C)$. Si $x \in B$, entonces $x \in B \cap C$, lo que implica que $x \in A \cup (B \cap C)$. De manera similar, si $x \in A \cup C$, entonces $x \in A$ o $x \in C$. Si $x \in A$, entonces $x \in A \cup (B \cap C)$. Si $x \in C$, entonces $x \in B \cap C$, lo que implica que $x \in A \cup (B \cap C)$.
        Por lo tanto, $x \in A \cup (B \cap C)$.
    </li>
</ol>






