---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/ingegneria-sanitaria-ambientale/esercitazioni/es-02-cinetica-chimica-isa/"}
---


# Es 02 - Cinetica chimica - ISA
[[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/02. Cinetica delle reazioni chimiche\|2. Cinetica delle reazioni chimiche]]

- [x] mettere i grafici su un'unica riga ✅ 2024-01-19
- [x] Riscaricare grafico caso 2 da [[MatLab\|MatLab]] ✅ 2024-01-19




## Parte 1

$$
C_{B0} = 2 C_{A0}
$$
La cinetica ha espressione
$$
r_{A} = - k C_{A}C_{B}
$$
È ragionevole assumere che il rapporto 1:2 tra le concentrazioni di A e B si mantenga costante durante la reazione.
$$
C_{B} = 2 C_{A} \quad \forall t
$$
Quindi
$$
r_{A} = - k C_{A} \cdot 2 C_{A} = - 2 k C_{A}^{2}
$$
che è un'espressione standard di una cinetica di ordine 2 se la scriviamo con $k' = k$
$$
r_{A} = - k'C_{A}^{2}
$$

Decidiamo di applicare il metodo di analisi integrale. Cerchiamo di interpolare i dati su un piano in cui i piani diventano teoricamente ad andamento lineare. Per cinetica di ordine 2 sugli assi avremo:
$$
\begin{align}
x&: t \\
y&: \frac{1}{C_{A}}
\end{align}
$$
La pendenza sarà il $k'$. Otteniamo $k = \frac{1}{2}k'$ con unità $\rm \left[  \frac{l}{mmol \cdot s}  \right]$

## Parte 2

Ora non è più garantito il rapporto 1:2 iniziale.

NUMERI A CASO IN TABELLA

| t       | $C_{A}$ | $C_{B}$ | $\Delta C_{A}= C_{A_{0}} - C_{A}(t)$ | $\Delta C_{B}$ |
| ------- | ------- | ------- | ------------------------------------ | -------------- |
| 0       | 10      | 10      |                                      |                |
| $t_{1}$ | 9       | 8       | 1                                    | 2              |
| $t_{2}$ | 8       | 6       | 2                                    | 4              |
| $t_{3}$ | 7       | 4       | 3                                    | 6              |

Vediamo che rimane costante la relazione $\Delta C_{B} = 2 \Delta C_{A}$.
$$
C_{B_{0}} - C_{B} = 2(C_{A_{0}}-C_{A})
$$
da cui
$$
C_{B} = C_{B_{0}} - 2(C_{A_{0}}-C_{A})
$$
che ricordando che $C_{A_{0}} = C_{B_{0}}$ diventa
$$
\begin{align}
C_{B} &= C_{B_{0}} - 2(C_{A_{0}}-C_{A}) \\
&= - C_{A_{0}} + 2C_{A}
\end{align}
$$
Sostituendo nell'equazione della reazione:
$$
r_{A} = - k C_{A} \cdot (2C_{A}- C_{A_{0}})
$$
Usando il metodo integrale...
$$
\frac{dC_{A}}{dt} =  - k C_{A} \cdot (2C_{A}- C_{A_{0}})
$$
Che posso risolvere a separazione di variabili
$$
\int_{C_{A_0}}^{C_{A}} \frac{dC_{A}}{C_{A}(2C_{A}-C_{A_{0}})} =-k \int_{0}^{t} dt
$$
Che posso integrare considerando l'integrando come somma di 2 frazioni.
$$
\begin{align}
\int_{C_{A_0}}^{C_{A}} \left( - \frac{1}{C_{A_{0}}} \frac{1}{C_{A}} + \frac{2}{C_{A_{0}}} \frac{1}{2C_{A}-C_{A_{0}}} \right) \, dC_{A} = -k \int_{0}^{t} dt \\
\frac{1}{C_{A_{0}}} \int_{C_{A_0}}^{C_{A}} \left(  \frac{1}{C_{A}} - 2 \frac{1}{2C_{A}-C_{A_{0}}} \right) \, dC_{A} = -k \int_{0}^{t} dt
\end{align}
$$
Che integrato diventa:
$$
\begin{align}
- \frac{1}{C_{A_{0}}} \left( \ln \frac{C_{A}}{C_{A_{0}}} - \ln \frac{2C_{A}-C_{A_{0}}}{2C_{A_{0}}-C_{A_{0}}} \right) = -kt \\
- \frac{1}{C_{A_{0}}} \left( \ln \frac{C_{A}}{C_{A_{0}}} + \ln \frac{C_{A_{0}}}{2C_{A}-C_{A_{0}}} \right) = -kt \\
- \frac{1}{C_{A_{0}}} \ln \frac{C_{A}}{2C_{A}-C_{A_{0}}} = -kt
\end{align}
$$
Che posso linearizzare come
$$
\begin{align}
x&: t \\
y&: \ln \frac{C_{A}}{2C_{A}-C_{A_{0}}}
\end{align}
$$
Ottengo come coefficiente $C_{A_{0}}k$

$C_{A}$ si ricava come
$$
C_{A} = \frac{1}{2} (C_{B_{0}}-C_{B}-2C_{A_{0}})
$$


