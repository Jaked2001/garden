---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/idrologia/esercitazioni/es-06-statistica-per-l-idrologia-idro/"}
---


# [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Esercitazioni/Es 06 - Statistica per l'idrologia - Idro\|Es 06 - Statistica per l'idrologia - Idro]]

# Riferimenti teorici

Vd. slide: [[Es 6 - Statistica per l'idrologia - Slide - Idro.pdf]]

**Variabile Casuale:** Variabile i cui valori sono incerti e imprevedibili



# Svolgimento


## Esercizio 1

Calcolare i parametri statistici.
- Media
- Varianza
- Scarto quadratico medio
- Coefficienti di variazione
- Coefficiente di asimmetria
- Coefficiente di Curtosi
- Massimo
- Minimo
- Mediana
- Moda


Applicare le formule ai dati forniti

| Parametro                  | Formula excel                                      |
| -------------------------- | -------------------------------------------------- |
| Numerosità del campione    | [[CONTA.NUMERI(dati)\|CONTA.NUMERI(dati)]]                             |
| Media                      | [[MEDIA(dati)\|MEDIA(dati)]]                                    |
| Varianza                   | [[VAR.C(dati)\|VAR.C(dati)]]                                    |
| Scarto quadratico medio    | [[DEV.ST(dati)\|DEV.ST(dati)]]                                   |
| coefficiente di variazione | $\dfrac{\text{Deviazione standard}}{\text{Media}}$ |
| Coefficiente di asimmetria | [[ASIMMETRIA(dati)\|ASIMMETRIA(dati)]]                               |
| Coefficiente di Curtosi    | [[CURTOSI(dati)\|CURTOSI(dati)]]                                  |
| Massimo                    | [[MAX(dati)\|MAX(dati)]]                                      |
| Minimo                     | [[MIN(dati)\|MIN(dati)]]                                      |
| Mediana                    | [[MEDIANA(dati)\|MEDIANA(dati)]]                                  |
| Moda                       | [[MEDIA(dati)\|MEDIA(dati)]]                                    |


## Esercizio 2

### Distribuzione Normale

Riscrivi [[Media\|Media]], [[Deviazione Standard\|Deviazione Standard]] e numerosità nelle celle apposite.

Crea una colonna di contatori con i numeri da 1 a "numerosità"

Nella colonna "X" aggiungere i dati ordinati in ordine crescente. Questa è la colonna della variabile aleatoria (del nostro campione) di cui vogliamo calcolare le statistiche.

Nella colonna "Fs" dobbiamo inserire la [[Frequenza di non superamento\|Frequenza di non superamento]] $F(x_{i})$. Questa è la probabilità che il campione assuma valore $x\le x_{i}$. Con i valori di "X" in ordine crescente calcoliamo il rapporto tra il numero di volte che il campione assume un valore inferiore o uguale a $x_{i}$ (nel nostro caso, con i dati in ordine crescente, questo sarà proprio il valore del contatore alla data posizione) fratto la numerosità del campione.

Al fine di evitare i valori 0 e 1 si applicano delle correzioni. Nel nostro caso sfrutteremo la cosiddetta correzione di Blom, che consiste nel calcolare Fs nel modo seguente:
$$
Fs = \frac{i-b}{N+1-2b}
$$
dove:
- $i:$ valore del contatore
- $b:$ fattore di correzione (in questo caso di Blom) pari a $b = \frac{3}{8}$
- $N:$ numerosità del campione


A questo punto procediamo a calcolare la [[Università/Triennale/2° anno/2° Semestre/Probabilità e statistica/Appunti/03. Variabili Aleatorie#Densità continua\|funzione di densità di probabilità]] (indicata anche come "pdf", $p(x)$) e la [[Università/Triennale/2° anno/2° Semestre/Probabilità e statistica/Appunti/03. Variabili Aleatorie#Funzione di Ripartizione\|funzione di ripartizione]] ("CDF", $P(x)$).

Queste sono rispettivamente, per la [[Università/Triennale/2° anno/2° Semestre/Probabilità e statistica/Appunti/03. Variabili Aleatorie#Variabile Aleatoria Normale o Gaussiana\|distribuzione gaussiana o normale]]:
$$
\begin{align}
p(x) &= \frac{e^{\frac{(x-\mu)^{2}}{2 \sigma^{2}}}}{\sqrt{2 \pi \sigma^{2}}} \quad -\infty<x<\infty \\
P(x) &= \frac{1}{\sqrt{2 \pi \sigma^{2}}} \int_{-\infty}^{x} e^{- \dfrac{(x-\mu)^{2}}{2 \sigma^{2}}} \, dx 
\end{align}
$$

 
In excel possono essere calcolate facilmente facendo uso di 2 formule, rispettivamente:

| Parametro | Formula excel                                                  |
| --------- | -------------------------------------------------------------- |
| pdf       | [[DISTRIB.NORM(dati, media, deviazione_standard, cumulativo)\|DISTRIB.NORM(dati, media, deviazione_standard, cumulativo)]] |
| CDF       | [[DISTRIB.NORM(dati, media, deviazione_standard, cumulativo)\|DISTRIB.NORM(dati, media, deviazione_standard, cumulativo)]] |
A questo punto si può cominciare a disegnare alcuni grafici. 








### Distribuzione LogNormale



### Distribuzione Gumbel






