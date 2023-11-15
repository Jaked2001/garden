---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/ingegneria-sanitaria-ambientale/esercitazioni/es-05-analisi-dei-reattori-boh-isa/"}
---


# Es 5 - Analisi dei reattori boh

## Riferimenti teorici

Per determinare il volume possiamo passare dal [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/03. Reattori Ideali#Tempo di residenza idraulica\|Tempo di residenza]] che possiamo ricavare dall'equazione di [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/03. Reattori Ideali#Bilancio di materia - PFR\|bilancio di materia]]

Velocità di reazione PFR senza ricircolo:
$$
\frac{dC_{A}}{d \theta_{H}} = r_{A}
$$
che integrata diventa
$$
\theta_{\rm TOT} = \int_{C_{A_{u}}}^{C_{A_{0}}} - \frac{1}{r_{A}} \, dC_{A}
$$

Velocità di reazione PFR con ricircolo:
$$
\frac{dC_{A}}{d \theta^{*}} = r_{A} \qquad \theta_{H}^{*} = \frac{\theta_{H}}{1+\alpha}
$$
che integro ottenendo:
$$
(1+\alpha) \int_{C_{A_{u}}}^{C_{a_{i}}} -\frac{dC_{A}}{r_{A}} = \int_{0}^{\theta_{H}} \, d \theta_{H}
$$
Avevamo ottenuto $C_{A_{i}}$ come media pesata:
$$
C_{A_{i}} = \frac{QC_{A_{0}}+Q_{R}C_{A_{u}}}{Q+Q_{R}}
$$

Per la prima parte è uguale a [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 03 - Analisi di reazione - ISA\|Es 03 - Analisi di reazione - ISA]].
Per la seconda, con ricircolo, dobbiamo usare l'altra formula.
$C_{A_{i}}$ l'abbiamo ricavato
Teniamo conto che l'ingresso e l'uscita devono essere gli stessi.
$$
C_{A_{u}} = 1
$$
$C_{A_{i}}$ varia a seconda di quanto è il rapporto di ricircolo. Infatti diventa:
$$
C_{A_{i}}=\frac{C_{A_{0}}+\alpha(C_{A_{u}})}{1+\alpha}
$$
Vediamo come varia $\theta_{H}$ in funzione di $\alpha$. Quindi usiamo più rapporti di ricircolo. 
Non conviene fissare $\alpha$ e vedere quanto viene $C_{A_{i}}$. Conviene scegliere $C_{A_{i}}$ con gli stessi valori di $C_{A}$ in tabella e vediamo a ritroso quanto corrisponde in termini di $\alpha$.

$\alpha$ lo ricaviamo ribaltando la formula di $C_{A_{i}}$.
$$
\alpha  = \frac{C_{A_{0}}-C_{A_{i}}}{C_{A_{i}}-C_{A_{u}}}
$$
Per $\alpha \to \infty$, $C_{A_{i}} \to C_{A_{u}}$ ossia un reattore in cui appena entra il fluido, ha concentrazione di uscita. Quindi al limite è un CFSTR. L'asintoto lo possiamo trovare con la formula di un CFSTR.

❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗Confrontare con il volume necessario per un CFSTR.
❗❗❗❗❗❗❗❗❗❗❗❗❗


#### Riferimenti utili


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/3-anno/1-semestre/ingegneria-sanitaria-ambientale/appunti/03-reattori-ideali/#confronto-efficienza-tra-cfstr-e-pfr" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

$<div class="markdown-embed-title">

# Confronto tra CFSTR e PFR

</div>


## Confronto efficienza tra CFSTR e PFR

Per confrontare il [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 05 - Analisi dei reattori boh - ISA#Reattore CFSTR\|#Reattore CFSTR]] con [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 05 - Analisi dei reattori boh - ISA#Reattore PFR\|#Reattore PFR]] si può procedere in due modi:
1. A parità di $C_{A_{0}}$ e $C_{A_{u}}$ confrontare i [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 05 - Analisi dei reattori boh - ISA#Tempo di residenza idraulica\|#Tempo di residenza idraulica]] $\theta_{H}$
2. A parità di $C_{A_{0}}$ e $\theta_H$ confrontare le concentrazioni in uscita $C_{A_{u}}$
Per la natura delle equazioni di [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 05 - Analisi dei reattori boh - ISA#Bilancio di materia\|#Bilancio di materia]], conviene il metodo 1.

Si ricorda da [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 05 - Analisi dei reattori boh - ISA#Bilancio di materia - CFSTR\|#Bilancio di materia - CFSTR]] e [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 05 - Analisi dei reattori boh - ISA#Bilancio di materia - PFR\|#Bilancio di materia - PFR]]:
$
\begin{matrix}
\text{CFSTR} && \text{PFR} \\
QC_{A_{0}} - Q C_{A_{u}} + r_{A}V = 0 && \frac{dC_{A}}{d \theta_{H}} \\
- r_{A} = \frac{C_{a_{0}} - C_{A_{u}} }{\theta_{H}} && \int_{C_{A_{0}}}^{C_{A_{u}}} \frac{1}{r_{A}} \, dC_{A}= \int_{0}^{\theta_{H}} \, d\theta_{H} \\
\theta_{H} = - \frac{1}{r_{A}}(C_{A_{0}} - C_{A_{u}}) && \int_{C_{A_{u}}}^{C_{A_{0}}}- \frac{1}{r_{A}} \, dC_{A} = \int_{0}^{\theta_{H}} \, d\theta_{H}
\end{matrix}
$
Quindi per il CFSTR, $\theta_{h}$ è l'area del rettangolo blu, mentre per il PFR è l'area sottesa dalla curva, evidenziata in rosso

![03. Reattori Ideali 2023-11-06 13.11.06.excalidraw.png](/img/user/Excalidraw/03.%20Reattori%20Ideali%202023-11-06%2013.11.06.excalidraw.png)


Quindi, nel caso ci sia una relazione monotona tra $r_{A}$ e $C_{A}$ nei due reattori, il [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 05 - Analisi dei reattori boh - ISA#Reattore PFR\|#Reattore PFR]] risulta essere più efficiente - ha [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Esercitazioni/Es 05 - Analisi dei reattori boh - ISA#Tempo di residenza idraulica\|#Tempo di residenza idraulica]] minore.

In caso di relazione generica non possiamo dire nulla a priori e tocca analizzare caso per caso.


</div></div>


