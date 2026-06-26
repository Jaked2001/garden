---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/16-macchine-elettriche-et/","tags":["UNI"],"dg-note-properties":{"aliases":null,"Materia":"ET","Tipo":"T","Stato":"🟢 Fatto","Slide":null,"PDF":null,"Parents":["[[🔌 Elettrotecnica]]"],"Children":["[[Trasformatore\|Trasformatore]]"],"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/16 - Macchine elettriche - ET\|16 - Macchine elettriche - ET]]

Le macchine elettriche sono in genere di 2 tipi:
- Statiche - ([[Trasformatore\|Trasformatore]]) - Non ci sono organi in movimento
- Dinamiche - Rotanti (motori - [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]])

## Trasformatore


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">





# [[Trasformatore\|Trasformatore]]

![Trasformatore 2024-06-28 17.51.48.excalidraw.png](/img/user/Excalidraw/Trasformatore%202024-06-28%2017.51.48.excalidraw.png)
[[Excalidraw/Trasformatore 2024-06-28 17.55.16.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore 2024-06-28 18.07.33.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore 2024-06-28 19.15.02.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore - Circuito equivalente ideale 2024-06-28 19.44.51.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore - Trasferimento delle impedenze - 2024-07-09 10.29.57\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore - Circuito eq con resistori - 2024-06-29 19.36.56.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore reale 2024-06-29 19.40.19.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore reale 2024-06-29 19.40.19.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore a vuoto 2024-06-30 12.13.57.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore reale - circuito 2024-06-30 16.05.42.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Trasformatore reale - circuito 2024-06-30 16.05.42.excalidraw\|🖋 Edit in Excalidraw]]

dove:
- $\dot{Z}_{L} = R_{L}+jX_{L}:$ Impedenza di linea
- $\dot{Z}_{M}:$ Impedenza di ingresso del motore, dipendente dallo scorrimento (ossia da $\Omega_{rot}$)
- $\overline{V}:$ Tensione di alimentazione degli avvolgimenti statorici del [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]]

Si può calcolare la caduta percentuale di tensione:
$$
\Delta V_{\%} = \frac{R_{L}P+X_{L}Q}{V^{2}} \cdot 100
$$

Il motore è generalmente alimentato a $V = 220\,\rm V$. La caduta di tensione però deve rimanere contenuta in modo da limitare le correnti di avviamento. Se ciò non avviene, si finisce solo per aumentare la caduta percentuale, facendo diminuire la tensione di alimentazione con il risultato di avere correnti di avviamento elevate e una macchina che non parte.

Per ovviare a ciò si sfrutta l'[[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/16 - Macchine elettriche - ET#Avviamento con commutazione stella-triangolo\|#Avviamento con commutazione stella-triangolo]]

#### Avviamento con commutazione stella-triangolo

Questo tipo di avviamento, nei motori a gabbia di scoiattolo, sfrutta il fatto che, a parità di tensioni, le correnti di carico nella [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a stella\|configurazione a stella]] risultano essere 1/3 di quelle nella [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a triangolo\|configurazione a triangolo]].

Anche se la tensione di alimentazione del motore è $\overline{V}$, la tensione sulle fasi statoriche risulterà la tensione stellata
$$
\overline{E} = \frac{\overline{V}}{\sqrt{3}}
$$
La corrente sul carico (corrispondente nel collegamento a stella alla [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di linea\|corrente di linea]]) sarà:
$$
\overline{I}_{\star} = \frac{\overline{E}}{\dot{Z}} = \frac{\overline{V}}{\sqrt{3}\dot{Z}} 
$$
La coppia di spunto anche risulterà ridotta. Essendo essa proporzionale al quadrato della tensione:
$$
C_{\triangle} = 3 C_{\star}
$$
#### Avviamento nei motori a doppia gabbia di scoiattolo

Nel [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/16 - Macchine elettriche - ET#Rotore a doppia gabbia di scoiattolo\|#Rotore a doppia gabbia di scoiattolo]] si è detto che le sezioni delle gabbie sono così relazionate:
$$
S_{e}<S_{i}
$$
Si possono calcolare le impedenze delle due gabbie:
$$
\begin{align}
\dot Z_{i} &= R_{i} + jsX_{di} \\
\dot Z_{e} &= R_{e} + jsX_{de}
\end{align}
$$
È chiaro che la corrente totale che scorre nelle gabbie è la somma delle correnti delle singole gabbie:
$$
\overline{I}_{r} = \overline{I}_{i} + \overline{I}_{e}
$$
E lo stesso posso dire per le coppie:
$$
C_{m} = C_{mi} + C_{me}
$$


**AVVIAMENTO** - $s=1$

![Schermata 2024-07-08 alle 16.29.16.png](/img/user/Schermata%202024-07-08%20alle%2016.29.16.png)

In fase di avviamento, le impedenze diventano:
$$
\begin{align}
\dot Z_{i} &= R_{i} + jX_{di} \\
\dot Z_{e} &= R_{e} + jX_{de}
\end{align}
$$
La resistenza rotorica, rispetto alla reattanza induttiva è trascurabile.
Essendo, per via delle dimensioni
$$
X_{di} \gg X_{de} 
$$
sarà anche vero, in termini di impedenze:
$$
\dot Z_{i} \gg \dot Z_{e}
$$
Pertanto, la corrente di rotore, risulterà, in fase di avviamento, pari a quella della gabbia esterna
$$
\overline{I}{r} \simeq \overline{I}_{e}
$$

**VICINO AL SINCRONISMO** - $s\ll1$

![Schermata 2024-07-08 alle 16.29.47.png](/img/user/Schermata%202024-07-08%20alle%2016.29.47.png)

Una volta avviata, per velocità vicine al sincronismo, essendo lo [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/16 - Macchine elettriche - ET#Scorrimento\|#Scorrimento]] molto minore di 1, l'impedenza risulterà simile alla resistenza:
$$
\begin{align}
\dot Z_{i} &= R_{i} + jsX_{di} \simeq  R_{i}\\
\dot Z_{e} &= R_{e} + jsX_{de} \simeq  R_{e}
\end{align}
$$
Essendo 
$$
R_{i}\ll R_{e} \quad\Longrightarrow\quad Z_{i}\ll Z_{e}
$$
Pertanto, la corrente rotorica sarà pari a quella della gabbia interna
$$
\overline{I}_{r} \simeq \overline{I}_{i}
$$



In condizioni di funzionamento intermedie la corrente si ripartirà tra le due gabbie e si avrà [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/16 - Macchine elettriche - ET#Caratteristica coppia scorrimento\|#Caratteristica coppia scorrimento]] intermedia tra le situazioni di $s =1$ e $s=0$.

![Schermata 2024-07-08 alle 16.30.00.png](/img/user/Schermata%202024-07-08%20alle%2016.30.00.png)







</div></div>
