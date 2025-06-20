---
layout: post
title: Solución Cap 1, Ejercicio 1.5.1
subtitle: Cadenas de Markov Gibbs Fields, Monte Carlo Simulation and Queues  |  Pierre Bremaud | 2da Edición | Ingles
gh-repo: rull3r/Solucionario-MarkovChains-Bremaud
gh-badge: [star, fork, follow]
tags: [solucionario, probabilidad, cadenas-markov, simulaciones-estocásticas, teoria-conjuntos, modelos-estocasticos, procesos-aleatorios, calculo-probabilistico, principio-inclusion-exclusion, eventos-independientes]
full-width: true
comments: true
---

<div class="box-note">
Demuestre y generalice las siguientes identidades probabilísticas:<br>

<ol>
    <li>
            1. $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
        </li><br>
    <li>
        2. $P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(A \cap B) - P(B \cap C) - P(C \cap A) + P(A \cap B \cap C)$
    </li>
</ol>
</div>

#### Parte 1: Para dos conjuntos
Por definición de probabilidad de la unión:
$$
P(A \cup B) = P(A) + P(B) - P(A \cap B)
$$
donde $P(A \cap B)$ corrige la doble contabilidad.

#### Parte 2: Para tres conjuntos (fórmula extendida)
La probabilidad se calcula como:
$$
\begin{aligned}
P(A \cup B \cup C) = & \underbrace{P(A) + P(B) + P(C)}_{\text{Suma individual}} \\
& - \underbrace{[P(A \cap B) + P(A \cap C) + P(B \cap C)]}_{\text{Corrección de pares}} \\
& + \underbrace{P(A \cap B \cap C)}_{\text{Triple intersección}}
\end{aligned}
$$

<center>
<img src="https://upload.wikimedia.org/wikipedia/commons/4/42/Inclusion-exclusion.svg" width="300" alt="Diagrama de Venn para inclusión-exclusión">
</center>




### Generalización (Principio de Inclusión-Exclusión)

Para $n$ eventos $A_1, A_2, ..., A_n$:

$$
\begin{aligned}
P\left(\bigcup_{i=1}^n A_i\right) = & \sum_{i=1}^n P(A_i) \\
& - \sum_{1 \leq i < j \leq n} P(A_i \cap A_j) \\
& + \sum_{1 \leq i < j < k \leq n} P(A_i \cap A_j \cap A_k) \\
& - \cdots \\
& + (-1)^{n+1} P\left(\bigcap_{i=1}^n A_i\right)
\end{aligned}
$$

**Ejemplo para 4 conjuntos**:

$$
\begin{aligned}
P(A_1 \cup A_2 \cup A_3 \cup A_4) = & (P(A_1) + P(A_2) + P(A_3) + P(A_4)) \\
& - (P(A_1 \cap A_2) + \cdots + P(A_3 \cap A_4)) \\
& + (P(A_1 \cap A_2 \cap A_3) + \cdots ) \\
& - P(A_1 \cap A_2 \cap A_3 \cap A_4)
\end{aligned}
$$


<div class="box-note">

  <h3>📚 Referencias Teóricas</h3>
  
  <section>
    <h4 class="category">🔹 Fundamentos Probabilísticos</h4>
    <ul>
      <li><a href="https://es.wikipedia.org/wiki/Principio_de_inclusi%C3%B3n-exclusi%C3%B3n" target="_blank" rel="noopener">Principio de inclusión-exclusión</a></li>
      <li><a href="https://es.wikipedia.org/wiki/%C3%81lgebra_de_sucesos" target="_blank" rel="noopener">Álgebra de sucesos</a></li>
    </ul>
  </section>

  <section>
    <h4 class="category">🔹 Teoría de Conjuntos</h4>
    <ul>
      <li><a href="https://es.wikipedia.org/wiki/Uni%C3%B3n_de_conjuntos" target="_blank" rel="noopener">Unión e intersección</a></li>
      <li><a href="https://es.wikipedia.org/wiki/Diagrama_de_Venn" target="_blank" rel="noopener">Diagramas de Venn</a></li>
    </ul>
  </section>

  <section>
    <h4 class="category">🔹 Profundización</h4>
    <ul>
      <li><a href="https://es.wikipedia.org/wiki/Probabilidad_compuesta" target="_blank" rel="noopener">Probabilidad compuesta</a></li>
      <li><a href="https://es.wikipedia.org/wiki/Independencia_(probabilidad)" target="_blank" rel="noopener">Independencia estadística</a></li>
    </ul>
  </section>
</div>