---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/15-reti-trifasi-et/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET\|15 - Reti trifasi - ET]]

# Sistema trifase simmetrico

```ad-Definizione
title: Sistema trifase simmetrico 

Si definisce **sistema trifase simmetrico** un insieme di 3 grandezze [[13 - Funzioni sinusoidali e fasori - ET#Funzioni sinusoidali isofrequenziali|sinusoidali isofrequenziali]] di uguale ampiezza, sfasate reciprocamente di $\frac{2\pi}{3}$ ($120°$).
$
\begin{cases}
e_{1}(t) &= \sqrt{2} E\sin(\omega t) \\
e_{2}(t) &= \sqrt{2} E\sin\left( \omega t \mp \frac{2\pi}{3} \right) \\
e_{3}(t) &= \sqrt{2} E\sin\left( \omega t \mp \frac{4\pi}{3} \right) \\
\end{cases}
$

```


Si può dimostrare che:


```ad-Teo
title: Teorema

$
\sum\limits e_{i}() = 0
$
che riscritta in termini [[13 - Funzioni sinusoidali e fasori - ET#Fasore|fasoriali]]:
$
\begin{align}
\sum\limits \overline{E} &= 0 \\
\overline{E}_{1}+ \overline{E}_{2}+ \overline{E}_{3}&= 0
\end{align}
$

```



### Sistema trifase simmetrico diretto

![15 - Reti trifasi - ET 2024-06-22 18.26.29.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-22%2018.26.29.excalidraw.png)


```ad-Definizione
title: Sistema trifase simmetrico diretto

Un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico\|#Sistema trifase simmetrico]] si dice **diretto** se ciascuna grandezza risulta in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|ritardo]] di 120° ($\left(-\frac{2\pi}{3}\right)$ rispetto alla precedente

```


### Sistema trifase simmetrico inverso

![15 - Reti trifasi - ET 2024-06-22 18.37.17.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-22%2018.37.17.excalidraw.png)


```ad-Definizione
title: Sistema trifase simmetrico inverso

Un [[#Sistema trifase simmetrico]] si dice **inverso** se ciascuna grandezza risulta in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|ritardo]] di 120° ($\left(+\frac{2\pi}{3}\right)$ rispetto alla precedente.

```

## Collegamenti generatori-utilizzatori

Si considerino le 3 [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|reti]] *monofase* in figura ognuna caratterizzata da un [[Generatore ideale di tensione sinusoidale\|Generatore ideale di tensione sinusoidale]] $\overline{E}_{i}$ e un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Bipolo in regime sinusoidale e potenza\|bipolo]] di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|impedenza]] $\dot Z_{i}$.

![15 - Reti trifasi - ET 2024-06-23 12.50.33.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2012.50.33.excalidraw.png)


Le 3 correnti sono rispettivamente:
$$
I_{1} = \frac{\overline{E}_{1}}{\dot Z_{1}}
\qquad\qquad
I_{2} = \frac{\overline{E}_{2}}{\dot Z_{2}}
\qquad\qquad
I_{3} = \frac{\overline{E}_{3}}{\dot Z_{3}}
$$
Il sistema rimane equivalente se, i tre bipoli vengono connessi a un unico conduttore di ritorno (detto **neutro**):

![15 - Reti trifasi - ET 2024-06-23 16.56.35.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2016.56.35.excalidraw.png)


Per la [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]]:
$$
\overline{I}_{0} = \overline{I}_{1}+\overline{I}_{2}+\overline{I}_{3}
$$
Inoltre, essendo il sistema un [[#Sistema trifase simmetrico]],
$$
\overline{I}_{1}+\overline{I}_{2}+\overline{I}_{3} = 0
$$
Quindi, la corrente di neutro è nulla:
$$
\overline{I}_{0} = 0
$$
Pertanto, il sistema rimane del tutto equivalente aprendo il neutro. La rete così ottenuta è detta [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET\|Rete trifase]]. Si possono quindi avere:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Reti trifasi con neutro\|#Reti trifasi con neutro]] o (a 4 fili)
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Reti trifasi senza neutro\|#Reti trifasi senza neutro]] o (a tre fili)

### Rete trifase con neutro


![15 - Reti trifasi - ET 2024-06-23 16.56.35.excalidraw.png|550](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2016.56.35.excalidraw.png)


### Rete trifase senza neutro

![15 - Reti trifasi - ET 2024-06-23 12.50.33.excalidraw.png|550](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2012.50.33.excalidraw.png)


## Terne di tensioni trifase

Data una terna di generazione trifase come in figura sono individuabili 2 terne di tensioni:
- La terna di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni stellate\|#Tensioni stellate]]
- La terna di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni concatenate\|#Tensioni concatenate]]

![15 - Reti trifasi - ET 2024-06-23 17.06.55.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2017.06.55.excalidraw.png)


### Tensioni stellate

![15 - Reti trifasi - ET 2024-06-23 17.10.46.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2017.10.46.excalidraw.png)


```ad-Definizione
title: Tensioni stellate

La terna di **tensioni stellate** è quella costituita dalle tre tensioni tra il centro stella e i ciascun terminale di fase 1, 2 e 3. Queste tensioni coincidono con le tensioni dei generatori:
$
\begin{align}
{\color{blue} \overline{V}_{10}} &= \overline{E}_{1}  \\
{\color{blue} \overline{V}_{20}} &= \overline{E}_{2}  \\
{\color{blue} \overline{V}_{30}} &= \overline{E}_{3} 
\end{align}
$

```

Il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Rappresentazione grafica dei fasori\|diagramma fasoriale]] è riportato di seguito:

![15 - Reti trifasi - ET 2024-06-23 17.14.52.excalidraw.png|450](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2017.14.52.excalidraw.png)


È opportuno disporre i fasori a [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a stella\|stella]] applicandoli nello stesso punto $O$ che rappresenta il terminale del centro stella.

Le espressioni delle 3 tensioni saranno date da:
$$
\begin{cases}
\overline{E}_{1} &= E_{1} \\
\overline{E}_{2} &= E_{1}e^{\mp j \frac{2\pi}{3}} \\
\overline{E}_{3} &= E_{1}e^{\mp j \frac{4\pi}{3}}
\end{cases}
$$
dove nell'argomento si usa:
- Segno **meno** ($-$) per [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico diretto\|#Sistema trifase simmetrico diretto]] (tensioni in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|ritardo]])
- Segno **più** ($+$) per [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico inverso\|#Sistema trifase simmetrico inverso]] (tensioni in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|anticipo]])

### Tensioni concatenate

![15 - Reti trifasi - ET 2024-06-23 17.10.34.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2017.10.34.excalidraw.png)


```ad-Definizione
title: Tensioni concatenate

La terna di **tensioni concatenate** è quella costituita dalle tensioni tra i 3 terminali di fase 1, 2 e 3 costituita dai [[13 - Funzioni sinusoidali e fasori - ET#Fasore|fasori]]:
$
\begin{align}
\color{orange} \overline{V}_{12} \\
\color{orange} \overline{V}_{23} \\
\color{orange} \overline{V}_{31}
\end{align}
$

```

Il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Rappresentazione grafica dei fasori\|diagramma fasoriale]] è riportato di seguito:

![15 - Reti trifasi - ET 2024-06-23 17.24.22.excalidraw.png|450](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2017.24.22.excalidraw.png)


È opportuno disporre i fasori a [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a triangolo\|triangolo]].

### Relazioni tra tensioni stellate e concatenate


![15 - Reti trifasi - ET 2024-06-23 17.06.55.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2017.06.55.excalidraw.png)


Scrivendo le [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] rispetto al diagramma sopra, si trovano le relazioni tra le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni stellate\|#Tensioni stellate]] e le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni concatenate\|#Tensioni concatenate]]:
$$
\begin{cases}
\overline{V}_{12} &= \overline{E}_{1}-\overline{E}_{2} \\
\overline{V}_{23} &= \overline{E}_{2}-\overline{E}_{3} \\
\overline{V}_{31} &= \overline{E}_{3}-\overline{E}_{1}
\end{cases}
$$

![15 - Relazioni fasoriali tra terne di tensioni - ET 2024-06-23 18.27.27.excalidraw.png](/img/user/Excalidraw/15%20-%20Relazioni%20fasoriali%20tra%20terne%20di%20tensioni%20-%20ET%202024-06-23%2018.27.27.excalidraw.png)


Nel diagramma fasoriale si mostrano le relazioni tra le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni stellate\|#Tensioni stellate]] e le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni concatenate\|#Tensioni concatenate]].

Si osservi che le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni stellate\|#Tensioni stellate]] $\overline{V}_{12}, \overline{V}_{23}, \overline{V}_{31}$ risultano in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|in anticipo]] di $\frac{\pi}{6}$ (o $30°$) rispetto alle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni concatenate\|#Tensioni concatenate]] $\overline{E}_{1}, \overline{E}_{2}, \overline{E}_{3}$.

Inoltre,
$$
V = \sqrt{3} E \qquad \text{o} \qquad E = \frac{1}{\sqrt{3}}V
$$
## Generatori e carichi trifase

### Generatore trifase

```ad-Definizione
title: Generatore trifase

![15 - Reti trifasi - ET 2024-06-23 18.40.37.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2018.40.37.excalidraw.png)
%%[[15 - Reti trifasi - ET 2024-06-23 18.40.37.excalidraw.md|🖋 Edit in Excalidraw]]%%

Un **generatore trifase** è costituito da tre bipoli [[Generatore ideale di tensione sinusoidale|Generatore ideale di tensione - AC]] che costituiscono una [[#Terne di tensioni trifase|terna di tensioni trifase]]. Sono possibili 3 configurazioni:
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Generatori trifase a stella con neutro\|#Generatori trifase a stella con neutro]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Generatori trifase a stella senza neutro\|#Generatori trifase a stella senza neutro]]
- [[#Generatori trifase a triangolo]]


```

#### Generatori trifase a stella con neutro

![15 - Reti trifasi - ET 2024-06-23 18.44.42.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2018.44.42.excalidraw.png)


- I tre generatori sono collegati [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a stella\|a stella]]
- Il **centro stella** è accessibile dall'esterno (**neutro**)

È disponibile:
- una terna simmetrica di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni stellate\|#Tensioni stellate]] con [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valore efficace]] $E$
- Tra le coppie terminali di fase è disponibile una terna simmetrica di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni concatenate\|#Tensioni concatenate]] $V = \sqrt{3}E$.

#### Generatori trifase a stella senza neutro

![15 - Reti trifasi - ET 2024-06-23 18.50.20.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2018.50.20.excalidraw.png)


- I tre generatori sono collegati [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a stella\|a stella]]
- Il **centro stella** **NON** è accessibile dall'esterno

È disponibile:
 - Una terna simmetrica di tensioni [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni concatenate\|#Tensioni concatenate]] tra le coppie di terminali con [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valore efficace]] $V = \sqrt{3}E$


#### Generatori trifase a triangolo

![15 - Reti trifasi - ET 2024-06-23 18.50.44.excalidraw.png](/img/user/Excalidraw/15%20-%20Reti%20trifasi%20-%20ET%202024-06-23%2018.50.44.excalidraw.png)


- I tre generatori sono collegati [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a triangolo\|a triangolo]]

È disponibile
- Una terna simmetrica di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni concatenate\|#Tensioni concatenate]] con [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valore efficace]] $V = E$

### Carico trifase

A un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Generatore trifase\|#Generatore trifase]] è collegabile un **carico trifase** in una delle seguenti configurazioni:

![15 - Configurazioni terna carico trifase - ET.excalidraw.png](/img/user/Excalidraw/15%20-%20Configurazioni%20terna%20carico%20trifase%20-%20ET.excalidraw.png)


Se il **carico è equilibrato** tutti i carichi hanno stessa [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|impedenza]].

- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Carico trifase a stella con neutro\|#Carico trifase a stella con neutro]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Carico trifase a stella senza neutro\|#Carico trifase a stella senza neutro]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Carico trifase a triangolo\|#Carico trifase a triangolo]]


## Terne di correnti trifase

![15 - Terne di correnti - ET 2024-06-24 11.28.34.excalidraw.png](/img/user/Excalidraw/15%20-%20Terne%20di%20correnti%20-%20ET%202024-06-24%2011.28.34.excalidraw.png)


Nei collegamenti tra generatori e carichi si individua la **terna di correnti di linea** rappresentata dai fasori $\overline{I}_{1}, \overline{I}_{2},\overline{I}_{3}$. Se la terna è [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico\|simmetrica]] si ha che:
$$
\overline{I}_{1} + \overline{I}_{2} + \overline{I}_{3} = 0
$$
Di conseguenza, essendo $I_{0} = \overline{I}_{1} + \overline{I}_{2} + \overline{I}_{3}$ si ha anche che:
$$
\overline{I}_{0} = 0
$$

![15 - Configurazioni terna corrente trifase - ET.excalidraw.png](/img/user/Excalidraw/15%20-%20Configurazioni%20terna%20corrente%20trifase%20-%20ET.excalidraw.png)


- Nei collegamenti a [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a stella\|stella]] le correnti di linea coincidono con le correnti delle fasi interne
- Nei collegamenti a [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a triangolo\|triangolo]] le correnti delle fasi interne (quelle che attraversano le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|impedenze]]) sono diverse dalle correnti di linea; si indicano con $\overline{J}_{12},\overline{J}_{23},\overline{J}_{31}$

Anche le fasi interne costituiscono una terna simmetrica:
$$
\overline{J}_{12} + \overline{J}_{23} + \overline{J}_{31} = 0
$$


### Correnti di linea

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

Le espressioni delle 3 tensioni saranno date da:
$$
\begin{cases}
\overline{I}_{1} &= I_{1} \\
\overline{I}_{2} &= I_{1}e^{\mp j \frac{2\pi}{3}} \\
\overline{I}_{3} &= I_{1}e^{\mp j \frac{4\pi}{3}}
\end{cases}
$$
dove nell'argomento si usa:
- Segno **meno** ($-$) per [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico diretto\|#Sistema trifase simmetrico diretto]] (tensioni in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|ritardo]])
- Segno **più** ($+$) per [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico inverso\|#Sistema trifase simmetrico inverso]] (tensioni in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|anticipo]])

### Correnti di fase

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

Le espressioni delle 3 tensioni saranno date da:
$$
\begin{cases}
\overline{J}_{12} &= J_{12} \\
\overline{J}_{23} &= J_{12}e^{\mp j \frac{2\pi}{3}} \\
\overline{J}_{31} &= J_{12}e^{\mp j \frac{4\pi}{3}}
\end{cases}
$$
dove nell'argomento si usa:
- Segno **meno** ($-$) per [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico diretto\|#Sistema trifase simmetrico diretto]] (tensioni in [[13 - Funzioni sinusoidali e fasori - ET#Sfasamento|ritardo]])
- Segno **più** ($+$) per [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico inverso\|#Sistema trifase simmetrico inverso]] (tensioni in [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Sfasamento\|anticipo]])

### Relazioni tra correnti di linea e correnti di fase

![15 - Relazioni tra correnti di linea e correnti di fase - ET 2024-06-24 11.49.32.excalidraw.png](/img/user/Excalidraw/15%20-%20Relazioni%20tra%20correnti%20di%20linea%20e%20correnti%20di%20fase%20-%20ET%202024-06-24%2011.49.32.excalidraw.png)


Scrivendo le [[Legge di Kirchhoff delle Correnti (LKT)\|LKC]] ai terminali si deduce che [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di linea\|#Correnti di linea]] e [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di fase\|#Correnti di fase]] sono legate dalle seguenti relazioni:
$$
\begin{cases}
\overline{I}_{1} &= \overline{J}_{12}-\overline{J}_{31} \\
\overline{I}_{2} &= \overline{J}_{23}-\overline{J}_{12} \\
\overline{I}_{3} &= \overline{J}_{31}-\overline{J}_{23}
\end{cases}
$$

![15 - Relazioni fasoriali tra terne di correnti - ET 2024-06-24 11.51.41.excalidraw.png](/img/user/Excalidraw/15%20-%20Relazioni%20fasoriali%20tra%20terne%20di%20correnti%20-%20ET%202024-06-24%2011.51.41.excalidraw.png)


Dal diagramma fasoriale si deduce che le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di linea\|#Correnti di linea]] $\overline{I}_{1}, \overline{I}_{2}, \overline{I}_{3}$ sono [[13 - Funzioni sinusoidali e fasori - ET#Sfasamento|ritardo]] di $\frac{\pi}{6}$ (30°) rispetto alle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di fase\|#Correnti di fase]] $\overline{J}_{12}, \overline{J}_{23}, \overline{J}_{31}$.
Inoltre, 
$$
I = \sqrt{3} J \qquad\text{o}\qquad J = \frac{1}{\sqrt{3}} I
$$
## Analisi di una rete trifase simmetrica ed equilibrata

### Possibili configurazioni

- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Rete Yn-Yn\|#Rete Yn-Yn]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Rete Y-Y\|#Rete Y-Y]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Rete D-D\|#Rete D-D]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Rete D-Y\|#Rete D-Y]]
- [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Rete Y-D\|#Rete Y-D]]


#### Rete Yn-Yn

![15 - Rete trifase Yn-Yn - ET 2024-06-26 10.45.07.excalidraw.png](/img/user/Excalidraw/15%20-%20Rete%20trifase%20Yn-Yn%20-%20ET%202024-06-26%2010.45.07.excalidraw.png)


La rete trifase a 4 fili a stella con neutro è costituita da:
- [[#Generatori trifase a stella con neutro]]
- Carico a stella

I generatori sono caratterizzati dallo stesso [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valore efficace]] $E$ e ai capi di ognuno del carico si registra proprio la tensione del generatore corrispondente. Pertanto generatori e carichi sono percorsi dalle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di linea\|#Correnti di linea]]:
$$
\overline{I}_{1} = \frac{\overline{E}_{1}}{\dot{Z}} \qquad \overline{I}_{2} = \frac{\overline{E}_{2}}{\dot{Z}} \qquad \overline{I}_{3} = \frac{\overline{E}_{3}}{\dot{Z}}
$$
Essendo la terna di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni stellate\|#Tensioni stellate]] [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico\|simmetrica]], lo stesso sarà vero per le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di linea\|#Correnti di linea]]. In termini di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valori efficaci]] si avrà quindi che:
$$
I = \frac{E}{Z}
$$

![15 - Fasori Rete Yn-Yn - ET 2024-06-26 10.49.07.excalidraw.png|450](/img/user/Excalidraw/15%20-%20Fasori%20Rete%20Yn-Yn%20-%20ET%202024-06-26%2010.49.07.excalidraw.png)


Ogni corrente $I_{i}$ presenta il medesimo sfasamento rispetto alla rispettiva tensione $E_{i}$ pari a
$$
\varphi = \angle\dot{Z}
$$
dove:
- $\angle\dot{Z}:$ è l'argomento di $\dot{Z}$ - $\dot{Z} = Ze^{\varphi j}$


#### Rete Y-Y

![15 - Rete trifase Y-Y - ET 2024-06-26 10.56.56.excalidraw.png](/img/user/Excalidraw/15%20-%20Rete%20trifase%20Y-Y%20-%20ET%202024-06-26%2010.56.56.excalidraw.png)


La rete trifase a 3 fili a stella (senza neutro) è costituita da:
- [[#Generatori trifase a stella senza neutro]]
- Carico a stella
Si può considerare ottenuta dalla rete [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Rete Yn-Yn\|#Rete Yn-Yn]] senza neutro. Essendo per le proprietà delle reti trifasi $I_{0} = 0$, il neutro può in ogni caso essere eliminato senza alterare la rete.

Tutte le condizioni di funzionamento rimangono inalterate rispetto alla [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Rete Yn-Yn\|#Rete Yn-Yn]].

I generatori sono caratterizzati dallo stesso [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valore efficace]] $E$ e ai capi di ognuno del carico si registra proprio la tensione del generatore corrispondente. Pertanto generatori e carichi sono percorsi dalle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di linea\|#Correnti di linea]]:
$$
\overline{I}_{1} = \frac{\overline{E}_{1}}{\dot{Z}} \qquad \overline{I}_{2} = \frac{\overline{E}_{2}}{\dot{Z}} \qquad \overline{I}_{3} = \frac{\overline{E}_{3}}{\dot{Z}}
$$
Essendo la terna di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Tensioni stellate\|#Tensioni stellate]] [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Sistema trifase simmetrico\|simmetrica]], lo stesso sarà vero per le [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di linea\|#Correnti di linea]]. In termini di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/13 - Funzioni sinusoidali e fasori - ET#Valore efficace\|valori efficaci]] si avrà quindi che:
$$
I = \frac{E}{Z}
$$

![15 - Fasori Rete Yn-Yn - ET 2024-06-26 10.49.07.excalidraw.png|450](/img/user/Excalidraw/15%20-%20Fasori%20Rete%20Yn-Yn%20-%20ET%202024-06-26%2010.49.07.excalidraw.png)


Ogni corrente $I_{i}$ presenta il medesimo sfasamento rispetto alla rispettiva tensione $E_{i}$ pari a
$$
\varphi = \angle\dot{Z}
$$
dove:
- $\angle\dot{Z}:$ è l'argomento di $\dot{Z}$ - $\dot{Z} = Ze^{\varphi j}$


#### Rete D-D

![15 - Rete trifase D-D - ET 2024-06-26 11.01.47.excalidraw.png](/img/user/Excalidraw/15%20-%20Rete%20trifase%20D-D%20-%20ET%202024-06-26%2011.01.47.excalidraw.png)


#### Rete D-Y

#### Rete Y-D

### Rete ridotta monofase

## Potenza nei sistemi trifase

## Rifasamento del carico