---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/03-statistica-in-topografia-tp/"}
---

# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP\|03 - Statistica in Topografia - TP]]



Ogni volta che facciamo una misura compiamo un errore. Ci sono diverse cause di errore:
- Strumento
- Operatore
- Ambiente

Gli errori di misura possono essere categorizzate in 3 tipologie:
- Noise
- Bias
- Outlier


Siamo interessati a definire un [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#centro\|#centro]] di misura.

### Robustezza di una grandezza

## Centro

```ad-Definizione
title: Centro

Quando si esegue una misura, il **centro** è il valore che decido essere rappresentativo del fenomeno stocastico che ho davanti.

```

Il centro può essere scelto in vari modi, ognuno dei quali, vedremo, ha dei pro e dei contro. Intanto procediamo con il definire alcune grandezze statistiche utili.


### Media aritmetica

```ad-Definizione
title: Media Aritmetica

$$
\mu = \frac{1}{N} \sum\limits_{i=1}^{N} x_{i}
$$
dove:
- $x_{i}:$ sono i valori di cui calcolo la media
- $N:$ la numerosità del campione
```

La media, per quanto semplice da calcolare, non è un buon parametro da prendere come [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Centro\|#Centro]] di una serie di misure. La media infatti è molto [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Robustezza di una grandezza\|poco robusta]].

```ad-example
title: Esempio

Immaginiamo di avere il seguente set di dati:
$$
\begin{align}
3.4721 \\
3.4718 \\
3.4719 \\
3.4723 \\
{\color{red} 4.4722}
\end{align}
$$
Se calcoliamo la media solo dei primi 4 valori otteniamo $\mu = 3.4720$. Se invece includo anche il quinto valore (quello in rosso), ottengo $\mu = 3.6721$. È evidente che, con una singola misura molto diversa dalle altre, si ottenga una media molto diversa. 

In particolare si dice che 4.4722 è un [[#Autolier]] (= che sta fuori). Non è quindi rappresentativo del fenomeno rispetto agli altri 4 valori. 

Attenzione! Questo non vuol dire che sia sbagliato e gli altri giusti. Potrebbe essere l'unico esatto.
```



### Mediana

```ad-Definizione
title: Mediana
La **mediana** ($Me$) è il valore tale che la [[#frequenza relativa]] dei valori minori di $Me$ e dei valori maggiori di $Me$ è la stessa e pari a 0.5.
$$
\sum\limits_{i=1}^{N_{Me}} f_{i} = \sum\limits_{i = N_{me}+1}^{N} f_{i} = 0.5
$$
dove 
- $f_{i}:$ [[#Frequenza relativa]]

```



La mediana è una grandezza [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/03 - Statistica in Topografia - TP#Robustezza di una grandezza\|robusta]].


## Dispersione

### Varianza

### Deviazione Standard

### MAD (Median Absolute Deviation)

#### NMAD (Normalized MAD)

### Covarianza

### Coefficiente di correlazione lineare

### Dipendenza e Indipendenza stocastica


# Misure

## Precisione vs Accuratezza




