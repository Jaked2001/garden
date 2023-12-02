---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/ingegneria-sanitaria-ambientale/esercitazioni/es-03-analisi-di-reazione-isa/"}
---

# Es3 - Analisi di reazione - ISA

### Grado di conversione

Dato un rettore alimentato.
$X_{A}$ ci dice quanto della specie viene rimossa dal reattore
$$
X_{A} = \frac{C_{A_{0}} - C_{A_{u}} }{C_{A_{0}}}
$$
Si può scrivere anche come
$$
X_{A} = 1- \frac{C_{A}}{C_{A_{0}}}
$$

## Parte 1

L'obiettivo è trovare il volume del [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/03. Reattori Ideali#Reattore PFR\|reattore PFR]]. Usiamo qualche relazione che faccia uso del [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/03. Reattori Ideali#Tempo di residenza idraulica\|tempo di residenza idraulica]].
$$
\theta_{H} = \frac{V}{Q}
$$
Ci serve il bilancio di massa che se integrata ci fornisce il $\theta_{H}$
Ci serve il [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/03. Reattori Ideali#Bilancio di materia - PFR\|bilancio di materia]] per il reattore PFR:
$$
\frac{dC_{A}}{d \theta_{H}} = r_{A}
$$
separando le variabili e integrando:
$$
\begin{align}
\int_{C_{A_{0}}}^{C_{A_{u}}} \frac{d_{C_{A}}}{r_{A}} = \int_{0}^{\theta_{H_{\rm TOT}}} \, d\theta_{H} \\
\int_{C_{A_{u}}}^{C_{A_{0}}} -\frac{1}{r_{A}} \, dC_{A} = \int_{0}^{\theta_{H_{\rm TOT}}} \, d\theta_{H}
\end{align} 
$$
Siccome nei dati ho $r_{A}(X_{A})$ devo fare un cambio di variabile nell'integrale
$$
C_{A} = C_{A_{0}} (1-X_{A})
$$
Quindi
$$
dC_{A} = -C_{A_{0}} dX_{A}
$$
Ottengo così l'integrale:
$$
\theta_{H_{\rm TOT}} = \int_{X_{A}}^{0} -\frac{1}{r_{A}(X_{A})} (-C_{A_{0}}) \, dX_{A}
$$
Invertendo gli estremi e cambiando di segno e poi moltiplicando per $Q$ ottengo:
$$
V = Q \theta_{H_{\rm TOT}} = Q C_{A_{0}} \int_{0}^{X_{A_{u}}} -\frac{1}{r_{A}(X_{A})} \, dx 
$$

## Procedimento

Calcolo $- \frac{1}{r_{A}}$




Pensare a come sarebbe il volume se il reattore fosse un CFSTR
L'equilibrio di materia per un [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/03. Reattori Ideali#Reattore CFSTR\|reattore CFSTR]] ci da
$$
0 = \frac{C_{A_{0}}-C_{A_{u}} + r_{A} \theta_{H}}{\theta_{H}}
$$
da cui possiamo ricavare $\theta_{H}$
$$
- \frac{1}{r_{A}} (C_{A_{0}}-C_{A_{u}})
$$

Nel caso di CFSTR il volume non sarebbe area sottesa dalla curva ma come area di un rettangolo. che ha per base la $X_{A}$ e come altezza la $- \frac{1}{r_{A}}$ calcolata in $X_{A}$.

Secondo i nostri dati abbiamo che 
$$
Q_{m} = Q C_{A_{0}}
$$
quindi calcolando il volume del CFSTR come
$$
V = Q_{m} \cdot \left( - \frac{1}{r_{A}} \right) \cdot X_{A}
$$
corrisponde proprio all'equazione scritta sopra in quanto ricordo essere
$$
X_{A} = \frac{C_{A_{0}} - C_{A_{u}}}{C_{A_{0}}}
$$
Si nota che il volume richiesto per un reattore CFSTR rispetto a un PFR a parità di condizione è molto maggiore.

___
[[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/🩺 Ingegneria Sanitaria Ambientale\|🩺 Ingegneria Sanitaria Ambientale]]
