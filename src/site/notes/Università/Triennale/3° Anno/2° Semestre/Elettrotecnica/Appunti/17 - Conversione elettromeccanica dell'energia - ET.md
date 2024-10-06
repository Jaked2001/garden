---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/17-conversione-elettromeccanica-dell-energia-et/","tags":["UNI"]}
---

# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET\|17 - Conversione elettromeccanica dell'energia - ET]]


È data una spira immersa in un campo magnetico uniforme, come in figura:

![Schermata 2024-06-30 alle 16.50.27.png](/img/user/Schermata%202024-06-30%20alle%2016.50.27.png)


## Trasformazione di potenza elettrica in potenza meccanica

Il diagramma sopra può essere rappresentato in proiezione secondo il seguente schema:

![17 - Conversione elettromeccanica dell'energia - ET 2024-06-30 16.51.07.excalidraw.png](/img/user/Excalidraw/17%20-%20Conversione%20elettromeccanica%20dell'energia%20-%20ET%202024-06-30%2016.51.07.excalidraw.png)


La spira è percorsa da una corrente $i$. Per via dell'interazione tra corrente e campo magnetico, sui lati della spira perpendicolari al campo si generano delle forze $\vec{F}$ date da:
$$
\vec{dF} = i\vec{dl}\times \vec{B}
$$
che integrata fornisce:
$$
\vec{F} = i\vec{l}\times\vec{B}
$$
dove:
- $l:$ lunghezza dei lati lunghi della spira (**lati attivi** --> paralleli all'asse di rotazione)

Le forze danno origine a una coppia:
$$
C = b\sin(\alpha) \cdot F
$$
dove $F = ilB$
quindi:
$$
C = ilBb\sin\alpha 
$$
La spira elementare, percorsa da corrente $I$, immersa in un campo magnetico uniforme stazionario di intensità $B$, è in grado di convertire potenza elettrica $P_{e}$ in potenza meccanica $P_{m}$.

## Trasformazione di potenza meccanica in potenza elettrica

![Trasformazione di potenza meccanica in potenza elettrica - ET 2024-06-30 17.03.23.excalidraw.png](/img/user/Excalidraw/Trasformazione%20di%20potenza%20meccanica%20in%20potenza%20elettrica%20-%20ET%202024-06-30%2017.03.23.excalidraw.png)


È data una spira immersa in campo magnetico uniforme stazionario di intensità $B$. La spira è in messa in rotazione da una coppia esterna a velocità angolare $\omega$. Attraverso la superficie $S$ della spira si genera un flusso:
$$
\phi = \iint \vec{B}\cdot \hat{n} \,dS 
$$
Essendo $B=\text{cost}$ e $S=\text{cost}$ il flusso sarà:
$$
BS\cos(\alpha) = Blb\cos(\alpha)
$$
Se la spira ruota a velocità angolare $\omega$, l'angolo $\alpha$ è funzione del tempo
$$
\alpha = \omega t
$$
per cui, la funzione che esprime il flusso in funzione del tempo diventa:
$$
\phi (t) = BS\cos(\omega t) = Blb \cos(\omega t)
$$
Per via della rotazione della spira, poiché il flusso varia nel tempo, si genera una fem indotta secondo la [[Legge di Faraday-Neumann Lentz\|Legge di Faraday-Neumann Lentz]]:
$$
e(t) = - \frac{\mathrm{d} \phi }{\mathrm{d}t} 
$$
Si è così effettuata la trasformazione da potenza meccanica $P_{m}$ a potenza elettrica $P_{e}$.


# Macchine elettriche elementari

Caratteristica fondamentale: conversione elettromeccanica dell'energia in maniera continuativa --> uso tante spire per garantire che ci sia sempre coppia.

Devo trovare un modo di far variare $\alpha$ in maniera continua: ad esempio posso generare un **campo magnetico rotante**. A seconda di come ottengo questo effetto avrò:
- Sorgente rotante: faccio girare i magneti
- Sorgente statica: faccio ruotare solo il campo magnetico

## Alimentazione con 1 coppia polare

![17 - Macchina elettrica - 1 coppia polare - ET 2024-06-30 18.19.19.excalidraw.png](/img/user/Excalidraw/17%20-%20Macchina%20elettrica%20-%201%20coppia%20polare%20-%20ET%202024-06-30%2018.19.19.excalidraw.png)


dove:
- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET#Statore\|#Statore]]: la parte fissa
- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET#Rotore\|#Rotore]]: la parte che ruota
- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET#Traferro\|#Traferro]]: Spessore d'aria --> favorisce il gioco necessario al moto relativo statore-rotore

Ad ogni tratto di filo è associato un campo magnetico:

![17 - Linee di campo - 1 coppia polare - ET 2024-06-30 18.26.13.excalidraw.png](/img/user/Excalidraw/17%20-%20Linee%20di%20campo%20-%201%20coppia%20polare%20-%20ET%202024-06-30%2018.26.13.excalidraw.png)


Le linee di campo si muovono sempre dal polo Nord al polo Sud. Pertanto, per come sono disposti campi dei due lati della spira, sullo statore e sul rotore si andranno ad individuare delle polarità come in figura. 

Si consideri ora una generica linea chiusa **linea di circuitazione**:

![17 - 1 coppia polare - Linea di circuitazione - ET 2024-07-01 12.11.02.excalidraw.png](/img/user/Excalidraw/17%20-%201%20coppia%20polare%20-%20Linea%20di%20circuitazione%20-%20ET%202024-07-01%2012.11.02.excalidraw.png)


Calcolando la circuitazione lungo $\gamma$ orientata in senso orario:
$$
\oint_{\gamma} \vec{H}\cdot \vec{dl}  = N\cdot i
$$
Si può spezzare la linea $\gamma$ nei seguenti tratti:
- $\overline{AB}:$ tratto nel rotore
- $\overline{CD}:$ tratto nel traferro
- $\overline{BC}, \overline{DA}:$ tratto nel traferro

Così l'integrale diventa:
$$
\oint_{\gamma} \vec{H} \cdot \vec{dl}  = \frac{1}{\mu_{f}}\int_{A}^{B}  \vec{B}\cdot \vec{dl} + \frac{1}{\mu_{f}}\int_{C}^{D}  \vec{B}\cdot \vec{dl} + 2\frac{1}{\mu_{0}}\int_{\delta}  \vec{B}_{0}\cdot \vec{dl}
$$
Se si suppone che la permeabilità magnetica di rotore e statore sia molto maggiore di quella nel vuoto:
$$
\mu_{f} \gg \mu_{0}
$$
allora l'integrale si riduce ai termini:
$$
\oint_{\gamma} \vec{H} \cdot \vec{dl}  = 2\frac{1}{\mu_{0}}\int_{\delta}  \vec{B}_{0}\cdot \vec{dl}
$$
Come abbiamo detto, con 1 coppia polare, si formano le polarità descritte prima. Se immaginiamo di percorrere in senso orario la macchina elettrica che stiamo analizzando, avremmo un andamento del campo magnetico come in figura:

![17 - Conversione elettromeccanica dell'energia - ET 2024-07-01 17.37.47.excalidraw.png](/img/user/Excalidraw/17%20-%20Conversione%20elettromeccanica%20dell'energia%20-%20ET%202024-07-01%2017.37.47.excalidraw.png)


Si genera pertanto un'onda quadra che può essere resa "più dolce" in vari modi:
- Disseminare lo statore di un numero molto grande di coppie polari
- Sviluppare in [[Serie di Fourier\|Serie di Fourier]] alla prima armonica:
$$
\begin{align}
B(\theta) &= - \frac{4}{\pi } \frac{\mu_{0}Ni}{2\delta} \cos\theta \to \text{min} \\
B(\theta) &= \frac{4}{\pi } \frac{\mu_{0}Ni}{2\delta} \cos\theta \to \text{max}
\end{align}
$$

![17 - Segnale rettangolare e addolcito - 1 coppia polare - ET 2024-07-01 17.51.52.excalidraw.png](/img/user/Excalidraw/17%20-%20Segnale%20rettangolare%20e%20addolcito%20-%201%20coppia%20polare%20-%20ET%202024-07-01%2017.51.52.excalidraw.png)


## Alimentazione con 2 coppie polari

![17 -Macchina elettrica - 2 coppie polari - ET 2024-07-01 17.55.04.excalidraw.png](/img/user/Excalidraw/17%20-Macchina%20elettrica%20-%202%20coppie%20polari%20-%20ET%202024-07-01%2017.55.04.excalidraw.png)


Quando sono presenti 2 coppie polari, esse vengono collegate come mostrato in figura.

Qui si andranno a generare 4 campi magnetici, uno per ogni tratto di filo, e si avranno pertanto 8 polarità:

![17 - Linee di campo - 2 coppie polari - 24-07-01 18.03.41.excalidraw.png](/img/user/Excalidraw/17%20-%20Linee%20di%20campo%20-%202%20coppie%20polari%20-%2024-07-01%2018.03.41.excalidraw.png)


Se immaginiamo di percorrere in senso orario la macchina elettrica che stiamo analizzando, avremmo un andamento del campo magnetico come in figura:

![17 - Segnale rettangolare e addolcito - 2 coppie polari - ET 2024-07-01 18.08.46.excalidraw.png](/img/user/Excalidraw/17%20-%20Segnale%20rettangolare%20e%20addolcito%20-%202%20coppie%20polari%20-%20ET%202024-07-01%2018.08.46.excalidraw.png)


## Alimentazione con corrente sinusoidale

Immaginiamo ora di alimentare la spira con una [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Regime sinusoidale\|corrente sinusoidale]]:
$$
i(t) = \sqrt{2}I\sin(\omega t)
$$
Il campo diventa:
$$
B_{\text{MAX}}(t) = \frac{\mu_{0}Ni(t)}{2\delta} = \frac{\mu_{0}N\sqrt{2}I}{2\delta}\sin(\omega t)
$$
A questo punto, a seconda di quante volte il filo percorre andata e ritorno (numero di polarità/2) si ha:
- $B(\theta,t) = - \dfrac{4}{\pi} \dfrac{\mu_{0}Ni(t)}{2\delta} \cos(\theta):$ per [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET#Alimentazione con 1 coppia polare\|#Alimentazione con 1 coppia polare]]
- $B(\theta,t) = - \dfrac{4}{\pi} \dfrac{\mu_{0}Ni(t)}{2\delta} \cos(2\theta):$ per [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET#Alimentazione con 2 coppie polari\|#Alimentazione con 2 coppie polari]]

$$
B(\theta,t) = - \dfrac{4}{\pi} \dfrac{\mu_{0}Ni(t)}{2\delta} \cos(p\theta)
$$
per p coppie polari





