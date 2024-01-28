---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/ingegneria-sanitaria-ambientale/esercitazioni/es-07-equalizzazione-isa/"}
---


# Es 7 - Equalizzazione - ISA

## Equalizzatore in linea (IL)

- [x] Fare parte sulle concentrazioni ✅ 2023-12-10
- [x] Scrivere relazione ✅ 2024-01-28
	- [x] Nei riferimenti teorici, aggiungi figura di regola filo teso ✅ 2024-01-28



Al tempo $t = 0^{+}$ il volume all'interno del reattore (Volume Residuo - $V_{R}$) sarà $V_{R} = 0$.
$$
\begin{cases}
t &= 0^{+} \\
V_{R} &= 0 \\
V_{i_{(0\div 1)}} &= Q_{i}\Delta t
\end{cases}
$$
Al tempo $t = 1^{-}$ sarà presente come volume residuo il volume entrato a $t_{0}^{+}$ e come concentrazione la concentrazione del primo $\Delta t$:
$$
\begin{cases}
t &= 1^{-} \\
V_{R_{1}} &= 0 + V_{i{(0 \div 1)}} \\
C_{A} &= C_{A_{i(0\div 1)}}
\end{cases}
$$
Al tempo $t = 1$, immaginando che il fluido sia estratto tutto alla fine dell'intervallo, ci sarà una certa portata e concentrazione in uscita dall'equalizzatore.
$$
\begin{cases}
t &= 1 \\
V_{u(0\div 1)} &= Q_{u(0\div 1)} \Delta t  \\
V_{R_{1}} &= 0 + V_{i(0\div 1)} - V_{u(0\div 1)} \\
C_{A} &= C_{A_{i(0\div 1)}} \\
C_{A_{u(0 \div 1)}} &= C_{A_{i(0\div 1)}}
\end{cases}
$$
Entrando nel prossimo intervallo $\Delta t = 1 \div 2$, guardiamo al tempo $t = 1^{+}$. 
Il volume residuo sarà il volume residuo all'intervallo precedente ($V_{R_{1}}$) più il volume in ingresso in questo intervallo. Per quanto riguarda la concentrazione invece, questa avrà come contributi la nuova concentrazione in ingresso $C_{A_{i(1\div2)}}$ per la quotaparte del nuovo volume in ingresso $V_{i(1\div 2)}$, e la concentrazione già presente nell'equalizzatore a cui si trova il volume residuo nel reattore per la quota parte $V_{R_{1}}$ ($C_{A_{u(0\div 1)}}$). La concentrazione di ora si trova quindi come media pesata con i volumi delle concentrazioni appena nominate.
$$
\begin{cases}
V_{i(1\div 2)} &= Q_{i(1\div 2)} \Delta t \\
V_{R_{(1\div 2)}} &= V_{R_{1}} + V_{i(1\div 2)} \\
C_{A_{u(1 \div 2)}} &= \dfrac{V_{R_{1}}C_{A_{(0\div 1)}} + V_{i (1\div 2)}C_{A_{i(1\div 2)}}}{V_{R_{1}} + V_{i(1\div 2)}}
\end{cases}
$$



## Equalizzatore fuori linea (FL)

- [x] Controllare a che punto sono arrivato a riscrivere in matlab da Excel ✅ 2024-01-28
- [x] Scrivere relazione sui FL ✅ 2024-01-28
	- [x] Riferimenti teorici ✅ 2024-01-28
	- [ ] 


Nelle conclusioni di entrambi scrivere quanto è il volume necessario ai due bacini.

