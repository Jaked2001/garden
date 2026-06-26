---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/00-introduzione-elettrotecnica/","dg-note-properties":{"aliases":null,"Materia":"ET","Tipo":"T","Stato":"🪶 Scrivere","Slide":null,"PDF":null,"Parents":["[[🔌 Elettrotecnica]]"],"Children":["[[Giovanni De Bellis]]"]}}
---


# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica\|00 - Introduzione elettrotecnica]]

## Dipolo

Il dipolo è un componente accessibile da due poli
I dipoli sono lineari

Un esempio di dipolo è il [[Resistore\|Resistore]].


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">




# [[Resistore\|Resistore]]

![Resistore 2024-02-26 18.37.25.excalidraw.png](/img/user/Excalidraw/Resistore%202024-02-26%2018.37.25.excalidraw.png)
[[Excalidraw/Resistore 2024-06-14 17.26.23.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Resistore sinusoidale.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Resistore 2024-06-20 12.10.16.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/00 - Introduzione elettrotecnica 2024-02-26 19.02.19.excalidraw\|🖋 Edit in Excalidraw]]

Per la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] alle due maglie (del primario e del secondario):
$$
\begin{cases}
\overline{V}_{1} &= \overline{E}_{1} + (R_{1}+j\omega L_{1d})\overline{I}_{1} \\
\overline{V}_{2} &= \overline{E}_{2} - (R_{2}+j\omega L_{2d})\overline{I}_{2}
\end{cases}
$$
Il [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Rapporto di trasformazione\|#Rapporto di trasformazione]]
$$
n = \frac{\overline{E}_{1}}{\overline{E}_{2}} = \frac{N_{1}}{N_{2}}
$$
che permette di riscrivere le equazioni sopra:
$$
\begin{cases}
\overline{V}_{1} &= \overline{E}_{1} + (R_{1}+j\omega L_{1d})\overline{I}_{1} = n\overline{E}_{2} + (R_{1}+j\omega L_{1d})\overline{I}_{1} \\
\overline{V}_{2} &= \overline{E}_{2} - (R_{2}+j\omega L_{2d})\overline{I}_{2} \qquad\Longrightarrow\qquad \overline{E}_{2} = \overline{V}_{2} + (R_{2}+j\omega L_{2d})\overline{I}_{2}
\end{cases}
$$
E quindi scrivo $\overline{V}_{1}$ come
$$
\overline{V}_{1} = (R_{1}+j\omega L_{1d})\overline{I}_{1} + n \left( \overline{V}_{2} + (R_{2}+j\omega L_{2d})\overline{I}_{2} \right) 
$$
Si osservi come **NON** c'è proporzionalità diretta tra $V_{1}$ e $V_{2}$.

Le correnti presenti nel circuito equivalente sono legate dalle seguenti relazioni:
$$
\begin{align}
\overline{I}_{10} &= \overline{I}_{1\mu} + \overline{I}_{1f} \\
\overline{I}_{1} &= \overline{I}_{10} + \overline{I}_{12}
\end{align}
$$
Mentre le correnti tra primario e secondario sono legate dalla:
$$
\overline{I}_{12} = \frac{1}{n} \overline{I}_{2}
$$
Si ottengono così le [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/00 - Introduzione elettrotecnica#Equazioni di trasferimento del trasformatore reale\|#Equazioni di trasferimento del trasformatore reale]]

#### Equazioni di trasferimento del trasformatore reale

$$
\begin{cases}
\overline{V}_{1} &= (R_{1}+j\omega L_{1d})\overline{I}_{1} + n \left( \overline{V}_{2} + (R_{2}+j\omega L_{2d})\overline{I}_{2} \right) \\
\overline{I}_{12} &= \cfrac{1}{n} \overline{I}_{2}
\end{cases}
$$

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗



</div></div>
