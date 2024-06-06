---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/allegati/arcotangente2/","tags":["UNI","Matematica"]}
---

# [[Università/3° Anno/2° Semestre/Topografia e Positioning/allegati/arcotangente2\|arcotangente2]]

L'**arcotangente2** è una funzione che estende la funzione arcotangente.

In [trigonometria](https://it.wikipedia.org/wiki/Trigonometria "Trigonometria") l'**arcotangente2** è una funzione a due argomenti che rappresenta una variazione dell'[arcotangente](https://it.wikipedia.org/wiki/Arcotangente "Arcotangente"). Comunque presi gli argomenti reali $x$ e $y$ non entrambi nulli, $\arctan2⁡(y,x)$ indica l'angolo in radianti tra il semiasse positivo delle $X$ di un piano cartesiano e un punto di coordinate $(x,y)$ giacente su di esso. L'angolo è positivo se antiorario (semipiano delle ordinate positive, $y>0$) e negativo se in verso orario (semipiano delle ordinate negative, $y<0$).

La funzione restituisce quindi valori in $(-\pi,\pi]$ ed è definita $\forall (x,y)$ **eccetto** $(0,0)$.

![arcotangente2 2024-05-25 22.52.04.excalidraw.png](/img/user/Excalidraw/arcotangente2%202024-05-25%2022.52.04.excalidraw.png)


L'arcotangente2, d'ora in poi anche $\arctan2$, assume i seguenti valori rispetto alle posizioni rappresentate nel diagramma:

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-13 11.34.53.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-13%2011.34.53.excalidraw.png)


| CASI | $\boldsymbol\arctan2$ |
| ---- | --------------------- |
| 1    | $\arctan$             |
| 2    | $\arctan$             |
| 3    | $\arctan$             |
| 4    | $\arctan+\pi$         |
| 5    | $\arctan+\pi$         |
| 6    | $\arctan+\pi$         |
| 7    | $\arctan+2\pi$        |
| 8    | $\arctan+2\pi$        |
| 9    | $\arctan+2\pi$        |

### Motivazione

La funzione [[arcotangente\|arcotangente]] restituisce valori compresi in un intervallo limitato $\displaystyle \left( - \frac{\pi}{2}, \frac{\pi}{2} \right)$. Quindi, quando si vuole ricavare l'angolo di un vettore che giace nella parte sinistra del piano cartesiano non c'è modo di farlo con questa funzione.

## Derivata

L'$\arctan2$ differisce dall'$\arctan$ solo per delle costanti. Non c'è quindi differenza tra le derivate:
In generale:
$$
\frac{d}{d f(x)} \arctan2(f(x)) = \frac{f'(x)}{1+f(x)^{2}}
$$

L'arcotangente 2 si trova spesso in questa forma:
$$
\alpha = \arctan2\left( \frac{x_{0}-x_{1}}{y_{0}-y_{1}} \right)
$$
In problemi di [[Università/3° Anno/2° Semestre/Topografia e Positioning/🧭 Topografia e Positioning\|Topografia]] è spesso necessario derivare la funzione sia in $x_{0}$ che in $y_{0}$:
$$
\begin{align}
\frac{\partial\alpha}{\partial x_{0}} &= \frac{ y_{0}-y_{1} }{ (x_{0}-x_{1})^{2} + (y_{0}-y_1)^{2}} \\ \\

\frac{\partial\alpha}{\partial y_{0}} &=- \frac{ x_{0}-x_{1} }{(x_{0}-x_{1})^{2} +(y_{0}-y_1)^{2}}
\end{align}
$$



