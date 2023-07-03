---
layout: post
title: Solución Cap$:$ 1, Sec$:$1, Ejercicio$:$ 1
subtitle: Topología  |  James Munkres | 2º Edición | Español
gh-repo: rull3r/Solucionario-Topologia-Munkres
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,topologia,conjuntos, logica, latex,libro, teoria de conjuntos,union, Morgan]
comments: true
---

<div class="box-note">
  Compruebe las leyes distributivas para la union y la intersección , asi como tambien las leyes De Morgan.
</div>

### Solucion

Para cualquier conjuntos $A$, $B$, y $C$, primero veremos que $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$,

$$\begin{align}
(\subset) \begin{aligned}
x \in A \cup (B \cap C) &\implies x \in A \text{ o } x \in (B \cap C)\\
&\implies x \in A \text{ o } \left(x \in B \text{ y } x \in C \right)\\
&\implies \left(x \in A \text{ o } x \in B\right) \text{ y } \left(x \in A \text{ o }x \in C \right)\\
&\implies x \in \left(A \cup B\right) \text{ y } x \in \left(A \cup C\right)\\
&\implies x \in \left(A \cup B\right) \cap \left(A \cup C\right)
\end{aligned}
\quad\quad\quad\quad
(\supset)\begin{aligned}
x \in (A \cup B) \cap (A \cup C) &\implies x \in (A \cup B) \text{ y } x \in (A \cup C)\\
&\implies \left(x \in A \text{ o } x \in B\right) \text{ y } \left(x \in A \text{ o }x \in C \right)\\
&\implies x \in A \text{ o } \left(x \in B \text{ y } x \in C \right)\\
&\implies x \in A \text{ o } x \in (B \cap C)\\
&\implies x \in A \cup (B \cap C)
\end{aligned}
\end{align}$$

<div class="box-warning">

Antes de continuar ya habras notado que para estas demostraciones usamos logica y asumimos que la distribucion de los conectivos logicos es cierta, por eso te dejo aqui la tabla de la verdad que servira para de demostracion

<h2>Propiedad Distributiva de AND sobre OR:</h2>
<p>Para cualquier proposiciones p, q y r:</p>
<p>(p AND q) OR r = (p OR r) AND (q OR r)</p>

<h3>Tabla de verdad:</h3>
<table>
  <tr>
    <th>p</th>
    <th>q</th>
    <th>r</th>
    <th>(p AND q) OR r</th>
    <th>(p OR r) AND (q OR r)</th>
  </tr>
  <tr>
    <td>V</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>V</td>
    <td>V</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>V</td>
    <td>F</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>V</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>F</td>
    <td>V</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
</table>

<p>Observamos que los valores de verdad de las expresiones (p AND q) OR r y (p OR r) AND (q OR r) son idénticos para todas las combinaciones de valores de verdad de p, q y r. Por lo tanto, se cumple la propiedad distributiva de AND sobre OR.</p>

<h2>Propiedad Distributiva de OR sobre AND:</h2>
<p>Para cualquier proposiciones p, q y r:</p>
<p>(p OR q) AND r = (p AND r) OR (q AND r)</p>

<h3>Tabla de verdad:</h3>
<table>
  <tr>
    <th>p</th>
    <th>q</th>
    <th>r</th>
    <th>(p OR q) AND r</th>
    <th>(p AND r) OR (q AND r)</th>
  </tr>
  <tr>
    <td>V</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>V</td>
    <td>V</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>V</td>
    <td>F</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>V</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>F</td>
    <td>V</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>V</td>
    <td>V</td>
    <td>V</td>
  </tr>
  <tr>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
    <td>F</td>
  </tr>
</table>

<p>Observamos que los valores de verdad de las expresiones (p OR q) AND r y (p AND r) OR (q AND r) son idénticos para todas las combinaciones de valores de verdad de p, q y r. Por lo tanto, se cumple la propiedad distributiva de OR sobre AND.</p>

<p>Estas demostraciones utilizando tablas de verdad confirman las propiedades distributivas de las conectivas lógicas AND y OR.</p>
</div>

Ahora veremos que $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$,

$$\begin{align}
(\subset) \begin{aligned}
x \in A \cap (B \cup C) &\implies x \in A \text{ y } x \in (B \cup C)\\
&\implies x \in A \text{ y } \left(x \in B \text{ o } x \in C \right)\\
&\implies \left(x \in A \text{ y } x \in B\right) \text{ o } \left(x \in A \text{ y }x \in C \right)\\
&\implies x \in \left(A \cap B\right) \text{ o } x \in \left(A \cap C\right)\\
&\implies x \in \left(A \cap B\right) \cup \left(A \cap C\right)
\end{aligned}
\quad\quad\quad\quad
(\supset)\begin{aligned}
x \in (A \cap B) \cup (A \cap C) &\implies x \in \left(A \cap B\right) \text{ o } x \in \left(A \cap C\right)\\
&\implies \left(x \in A \text{ y } x \in B\right) \text{ o } \left(x \in A \text{ y }x \in C \right)\\
&\implies x \in A \text{ y } \left(x \in B \text{ o } x \in C \right)\\
&\implies  x \in A \text{ y } x \in (B \cup C)\\
&\implies x \in A \cap (B \cup C)
\end{aligned}
\end{align}$$


Es el turno ahora de las Leyes De Morgan

Sean los conjuntos $A$, $B$, primero veremos que $(A \cap B)^c = A^c \cup B^c$,

$$\begin{align}
(\subset) \begin{aligned}
x \in (A \cap B)^c &\implies x \notin (A \cap B)\\
&\implies \text{si no esta en la interseccion,}\\
&\hspace{1.55cm}\text{entonces puede estar en A o en B}\\
&\implies x \notin A \text{ o }  x \notin B\\
&\implies x \in A^c \text{ o }  x \in B^c\\
&\implies x \in A^c \cup  B^c
\end{aligned}
\quad\quad\quad\quad
(\supset)\begin{aligned}
 x \in A^c \cup  B^c &\implies x \in A^c \text{ o }  x \in B^c\\
&\implies x \notin A \text{ o }  x \notin B\\
&\implies \text{si ni en A ni en B,}\\
&\hspace{1.55cm}\text{entonces no puede estar en la interseccion}\\
&\implies x \notin (A \cap B)\\
& \implies x \in (A \cap B)^c\\
\end{aligned}
\end{align}$$

Ahora veremos que $(A \cup B)^c = A^c \cap B^c$,

$$\begin{align}
(\subset) \begin{aligned}
x \in (A \cup B)^c &\implies x \notin (A \cup B)\\
&\implies \text{si ni en A ni en B,}\\
&\hspace{1.55cm}\text{entonces no puede estar en la interseccion}\\
&\implies x \notin A \text{ y }  x \notin B\\
&\implies x \in A^c \text{ y }  x \in B^c\\
&\implies x \in A^c \cap  B^c
\end{aligned}
\quad\quad\quad\quad
(\supset)\begin{aligned}
 x \in A^c \cap B^c &\implies x \in A^c \text{ y }  x \in B^c\\
&\implies x \notin A \text{ y }  x \notin B\\
&\implies \text{si no esta en A y ni en B,}\\
&\hspace{1.55cm}\text{entonces no puede estar en la union}\\
&\implies x \notin (A \cup B)\\
& \implies x \in (A \cup B)^c\\
\end{aligned}
\end{align}$$