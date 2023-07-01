---
layout: post
title: Solución Cap$:$ 1, Ejercicios$:$ 1 al 3
subtitle: Graph Theory and Its Applications |  Jonathan L. Gross - Jay Yellen - Mark Anderson | 3º Edición | Ingles
gh-repo: rull3r/Solucionario-GraphTheory-JonathanJayMark
gh-badge: [star, fork, follow]
tags: [solucionario,matematicas,algebra,lineal,latex,libro, grafos, arboles, combinatoria]
full-width: true
comments: true
---
Para los siguientes ejercicios construir un dibujo lineal, una tabla de incidencia y la secuencia de grados del grafo con la especificación formal dada.
<div class="box-note">
	1)<br><br>
	$V = \{u, w, x, z\}$ $\quad$;$\quad$ $E = \{e, f, g\}$ <br>
	endpts$(e) = \{w\}$$\quad$;$\quad$ endpts$(f) = \{x, w\}$$\quad$;$\quad$endpts$(g) = \{x, z\}$   
</div>

<img style="border-collapse: collapse; border: none; border-spacing: 0px;width: 350px;height: 350px;" src="https://raw.githubusercontent.com/rull3r/Solucionario-GraphTheory-JonathanJayMark/master/1-Introduction-to-graph-models/1-Graps-and-Digraphs/imagenes/grafo1-1.png" alt="Grafo 1-1" />
<table style="border-collapse: collapse; border: none; border-spacing: 0px;width: 40%;height: 40%;">
	<tr>
		<td style="border-bottom: 1px solid rgb(0, 0, 0); border-right: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			arista
		</td>
		<td style="border-bottom: 1px solid rgb(0, 0, 0); border-left: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			$e$
		</td>
		<td style="border-bottom: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			$f$
		</td>
		<td style="border-bottom: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			$g$
		</td>
	</tr>
	<tr>
		<td style="border-top: 1px solid rgb(0, 0, 0); border-right: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			endpts
		</td>
		<td style="border-top: 1px solid rgb(0, 0, 0); border-left: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			$w$
		</td>
		<td style="border-top: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			$w$
		</td>
		<td style="border-top: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			$x$
		</td>
	</tr>
	<tr>
		<td style="border-right: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
		</td>
		<td style="border-left: 1px solid rgb(0, 0, 0); padding-right: 3pt; padding-left: 3pt;">
			$w$
		</td>
		<td style="padding-right: 3pt; padding-left: 3pt;">
			$x$
		</td>
		<td style="padding-right: 3pt; padding-left: 3pt;">
			$z$
		</td>
	</tr>
</table>

<3,2,1,0>

<div class="box-note">
	2)<br><br>
    $V = \{u, v, x, y, z\}$ $\quad$;$\quad$ $E = \{a, b, c, d\}$ <br>
	endpts$(e) = \{u, v\}$$\quad$;$\quad$ endpts$(b) = \{x, v\}$$\quad$;$\quad$ endpts$(c) = \{u, v\}$$\quad$;$\quad$ endpts$(d) = \{x\}$
</div>

<div class="box-note">
	3)<br><br>
    $V = \{u, v, x, y, z\}$ $\quad$; $\quad$ $E = \{e, f, g, h, k\}$ <br>
	endpts$(e) = $endpts$(f) = \{u, v\}\quad$;$\quad$ endpts$(g) = \{x, z\}\quad$;$\quad$ endpts$(h) =$ endpts$(k) = \{y\}$
</div>

### Solucion
