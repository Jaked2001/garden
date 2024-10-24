---
{"dg-publish":true,"permalink":"/matrici-complesse-su-calcolatrice-grafica/"}
---

# [[Matrici complesse su calcolatrice grafica\|Matrici complesse su calcolatrice grafica]]


Questo software, chiamato [[SIMEQ\|SIMEQ]], compatibile con la calcolatrice grafica [[TI-84 Plus CE-T\|TI-84 Plus CE-T]] permette di risolvere sistemi di equazioni a coefficienti complessi.

Torna molto utile per risolvere i problemi di [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/🔌 Elettrotecnica\|🔌 Elettrotecnica]].

## Come si usa

Per usarlo occorre scrivere il sistema nella forma:

$$
\begin{cases}
Z_{11}I_{m1} + Z_{12}I_{m2} + \cdots + Z_{1n}I_{mn} = E_{1} \\
Z_{21}I_{m1} + Z_{22}I_{m2} + \cdots + Z_{2n}I_{mn} = E_{2} \\
 \cdots\cdots\cdots\cdots\cdots\cdots\cdots\cdots\cdots\cdots\cdots\cdots\\
Z_{n1}I_{m1} + Z_{n2}I_{m2} + \cdots + Z_{nn}I_{mn} = E_{n}
\end{cases}
$$

Che corrisponde al sistema lineare:

$$
\begin{bmatrix}
Z_{11} & Z_{12} & \cdots & Z_{1n} \\
Z_{21} & Z_{22} & \cdots & Z_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
Z_{n1} & Z_{n2} & \cdots & Z_{nn}
\end{bmatrix}
\begin{bmatrix}
I_{m1} \\ I_{m2} \\ \vdots \\ I_{mn}
\end{bmatrix}
=
\begin{bmatrix}
E_{1} \\ E_{2} \\ \vdots \\ E_{n}
\end{bmatrix}
$$

Una volta fatto ciò occorre inserire tutti i coefficienti $Z_{ij}$ e i termini noti $E_{i}$ in una lista della calcolatrice grafica.
1. Cliccare su `stat`
2. Selezionare `edit`
3. Inserire tutti valori riga per riga nella colonna di $L_{1}$ (prima i $n$ coefficienti, poi $E_{1}$, poi la seconda riga e così via)
4. Uscire con il comando `2nd + mode(quit)`
5. Cliccare su `prgm`
6. Selezionare il programma (nome default: **[[SIMEQ\|SIMEQ]]**)
7. Cliccare `enter`
8. Scrivere il numero di equazioni e Cliccare ancora `enter`
9. Ora, tornando in `stat`>`edit` è possibile ottenere i valori delle incognite come elementi di $L_{2}$


## Installazione