---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/06-bipoli-e-potenza-elettrica-et/","dg-note-properties":{"aliases":null,"Materia":"ET","Tipo":"T","Stato":"🟢 Fatto","Slide":null,"PDF":null,"Parents":["[[🔌 Elettrotecnica]]"],"Children":null}}
---

# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET\|06 - Bipoli e potenza elettrica - ET]]

## Bipolo


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/03-introduzione-allo-studio-delle-reti-elettriche-et/#bipolo" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Bipolo

```ad-Definizione
title: Bipolo

Il **bipolo** è un componente accessibile da due poli che gode delle seguenti proprietà:
- La corrente entrante ad un terminale è uguale alla corrente uscente
- La tensione tra i due terminali è una differenza di potenziale

```

Un qualsiasi bipolo è completamente identificato dalla relazione tensione-corrente ai suoi terminali.

![Schermata 2024-03-24 alle 13.35.12.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Elettrotecnica/Appunti/allegati/allegati/Schermata%202024-03-24%20alle%2013.35.12.png)

#### Convenzioni per tensione e corrente su un bipolo

I riferimenti di tensione e corrente ai capi di un [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Bipolo\|#Bipolo]] possono essere fissati in modo arbitrario. È utile quindi definire subito delle convenzioni.
In particolare useremo:
- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Convenzione del generatore\|#Convenzione del generatore]]
- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Convenzione dell'utilizzatore\|#Convenzione dell'utilizzatore]]

Il prodotto dei valori della corrente e della tensione vale
$$
V_{AB}I = P \qquad \rm [VA = W]
$$
dove $P$ ha le dimensioni di una **potenza**.

![03 - Introduzione allo studio delle reti elettriche - ET 2024-06-13 17.32.53.excalidraw.png](/img/user/Excalidraw/03%20-%20Introduzione%20allo%20studio%20delle%20reti%20elettriche%20-%20ET%202024-06-13%2017.32.53.excalidraw.png)
[[Excalidraw/03 - Introduzione allo studio delle reti elettriche - ET 2024-03-24 13.43.47.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/03 - Introduzione allo studio delle reti elettriche - ET 2024-03-24 13.40.18.excalidraw\|🖋 Edit in Excalidraw]]

La [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza attiva - reale\|potenza attiva]] del resistore è
$$
P = VI \ge 0
$$
ed è sempre **NON** negativa (il resistore non può erogare potenza). La [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza istantanea\|potenza istantanea]] ha valore massimo $V_{M}I_{M} = 2VI$.

Essendo $\varphi=0$ il [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Fattore di potenza\|fattore di potenza]] $\cos(\varphi)=1$. Quindi, tutta la [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza assorbita\|potenza assorbita]] coincide con la [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza apparente\|potenza apparente]] $A$. La [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|potenza reattiva]] $Q = 0$.
$$
A = \sqrt{P^{2}+Q^{2}} = P
$$
quindi
$$
P = A = VI = RI^{2} \qquad Q = 0
$$

___

Il resistore in regime sinusoidale può essere descritto anche facendo riferimento alle grandezze [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Fasore\|fasoriali]].
$$
\begin{align}
i(t) &\Longrightarrow \overline{I} = Ie^{j\beta} \\
v(t) &\Longrightarrow \overline{V} = Ve^{j\alpha}
\end{align}
$$
Il rapporto tra i fasori vale:
$$
\frac{\overline{V}}{\overline{I}} = \frac{V}{I}e^{j\varphi} = R
$$
Essendo $\varphi=0$ poiché tensione e corrente risultano in fase.



</div></div>



## Generatore ideale di tensione


<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">





# [[Generatore ideale di tensione\|Generatore ideale di tensione]]


```ad-Definizione
title: Generatore ideale di tensione

Il **generatore ideale di tensione** è un [[00 - Introduzione elettrotecnica#Dipolo|dipolo]] attivo che verifica la relazione:
$$
E = E_{s} \quad \forall I
$$

```

Si indica con il simbolo:

![Generatore ideale di tensione 2024-03-03 18.09.15.excalidraw.png](/img/user/Excalidraw/Generatore%20ideale%20di%20tensione%202024-03-03%2018.09.15.excalidraw.png)
[[Excalidraw/Generatore ideale di tensione 2024-03-03 18.12.01.excalidraw\|🖋 Edit in Excalidraw]]

Essendo la [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Potenza\|potenza]] data da
$$
P = VI = VI_{s}
$$
è evidente che il **generatore ideale di corrente** può avere potenza negativa (nel 4° quadrante).


</div></div>


## Bipoli particolari

### Cortocircuito

```ad-Definizione
title: Cortocurcuito

Il cortocircuito è un [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Bipolo\|#Bipolo]] che corrisponde a un [[Resistore\|Resistore]] a [[04 - Fenomeni di conduzione e resistori - ET#Resistenza elettrica|resistenza]] nulla ($R = 0$) e caratterizzato dalla seguente equazione:
$
V = 0 \quad \forall I
$

```

![Corto Circuito - 2024-06-14 17.49.24.excalidraw.png](/img/user/Excalidraw/Corto%20Circuito%20-%202024-06-14%2017.49.24.excalidraw.png)
[[Excalidraw/06 - Bipoli e potenza elettrica - ET 2024-06-14 17.50.45.excalidraw\|🖋 Edit in Excalidraw]]%%



## Potenza elettrica

In *regime stazionario* la **potenza** scambiata ad una porta elettrica dotata di tensione $V$ e corrente $I$vale
$$
P = VI \quad \rm [W] = [watt]
$$
Più in generale, la **potenza istantanea**, quando non ci si trovi in regime stazionario, è:
$$
p(t) = v(t)i(t)
$$
