---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/idrologia/appunti/07b-infiltrazione-idro/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro\|07b - Infiltrazione - Idro]]

L'infiltrazione ha luogo attraverso la superficie del suolo durante e dopo gli eventi meteorici. 

I fattori che influenzano le modalità di infiltrazione sono vari:
- Quelli che influenzano la quantità d'acqua disponibile
	- Tipo di precipitazione (pioggia, neve o grandine)
	- Andamento spazio-temporale dell'intensità della precipitazione
	- Morfologia della superficie del suolo (pendenza dei versanti, presenza di depressioni superficiali)
- Quelli che influenzano l'attitudine del terreno a lasciare infiltrare l'acqua:
	- Caratteristiche fisico-chimiche del materiale costituente il suolo (roccia o materiale sciolto, composizione mineralogica, assortimento granulometrico, presenza di una struttura)
	- Uso del suolo (copertura vegetale, presenza di apparati radicali, trattamenti meccanici quali aratura o dissodamento, drenaggi)
	- Condizioni iniziali di umidità



I secondi si possono distinguere in due categorie:
- Fattori **costanti nel tempo**
	- Morfologia della superficie del suolo
	- Caratteristiche fisico-chimiche del materiale del suolo
- Fattori **dipendenti dal tempo**
	- Condizioni iniziali di umidità del suolo

## Modellazione dell'infiltrazione

I modelli fisico-matematici dell'infiltrazione si riferiscono al moto dell'acqua attraverso un mezzo poroso omogeneo.

A una certa profondità dalla superficie del suolo si individua una **superficie libera della falda** che separa la zona in cui il mezzo è completamente saturo d'acqua da quella in cui i meati lasciati liberi dallo scheletro solido sono solo parzialmente occupati da acqua - Terreno non saturo

Il processo di infiltrazione avviene attraverso la zona non satura del terreno (a meno che la superficie libera della falda coincide con la superficie del terreno).

### Definizioni

#### Umidità del suolo

L'**umidità del suolo** è
$$
\theta= \frac{W_{a}}{W_{t}}
$$

La [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Appunti/00. Caratteristiche generali delle terre#Porosità\|porosità]]:

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#porosita" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



#### Porosità

```ad-Teo
title: Porosità ($n$)

Rapporto tra il volume dei vuoti e il volume totale
$
\begin{align}
n = \frac{V_{v}}{V_{\text{TOT}}} && 0 < n < 1
\end{align}
$

dove $n=1$ corrisponde al nulla
```


</div></div>


> W $\equiv$ V per la porosità

$\theta_{r}$ è detto **contenuto** [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Acqua di ritenzione\|#Acqua di ritenzione]] e costituisce l'acqua che non si può muovere.


![07b - Infiltrazione - Idro 2024-05-05 16.14.27.excalidraw.png](/img/user/Excalidraw/07b%20-%20Infiltrazione%20-%20Idro%202024-05-05%2016.14.27.excalidraw.png)


![Schermata 2024-05-05 alle 18.07.15.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-05-05%20alle%2018.07.15.png)

#### Acqua di ritenzione

```ad-Definizione
title: Acqua di detenzione

L'**acqua di detenzione** o di **ritenzione** è il totale dell'acqua tra adsorbimento, adesione e capillare isolata:
$$
W_{d} = \text{adsorbimento} + \text{adesione} + \text{capillare isolata}
$$

```

#### Acqua libera

```ad-Definizione
title: Acqua libera ($W_{e}$)

$$
W_{e} = W_{a} - W_{d}
$$
dove:
- $W_{a}:$ [[#Volume d'acqua]]
- $W_{d}:$ ???
```


#### Porosità efficace

```ad-Definizione
title: Porosità efficace
$$
n_{e} = \frac{W_{v}-W_{d}}{W_{t}}
$$
dove:
- $W_{v}:$ [[#Volume dei vuoti]]
- $W_{d}:$ ???
- $W_{t}:$ Volume totale del suolo
```


#### Capacità specifica di detenzione

```ad-Definizione
title: Capacità specifica di detenzione

$$
n_{d} = \frac{W_{d}}{W_{t}}
$$
dove:
- $W_{d}:$ ???
- $W_{t}:$ Volume totale del suolo
```


#### Grado di saturazione


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#grado-di-saturazione" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



#### Grado di saturazione

```ad-Teo
title: Grado di Saturazione ($S_{r}$)

$
\begin{align}
S_{r} = \frac{V_{w}}{V_{v}} && 0 < S_{r} < 1
\end{align}
$

```

Campione:
- Completamente saturo: $S_{r} = 1$
- Completamente asciutto: $S_{r} = 0$

</div></div>


> V $\equiv$ W


#### Tempo di ponding

```ad-Definizione
title: Tempo di ponding ($t_{p}$)

Il **tempo di ponding** è il tempo che il suolo impiega, in caso di pioggia, a raggiungere la condizione di saturazione e far si che si verifichi ruscellamento.

```

Si forma ristagno dell'acqua in superficie, come una pozzanghera. Pond infatti in inglese significa pozzanghera.

### Il fenomeno dell'infiltrazione

![07b - Infiltrazione - Idro 2024-05-05 20.05.56.excalidraw.png](/img/user/Excalidraw/07b%20-%20Infiltrazione%20-%20Idro%202024-05-05%2020.05.56.excalidraw.png)


Il diagramma sopra mostra l'andamento dell'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Umidità del suolo\|#Umidità del suolo]] nel sottosuolo. 

Si notino intanto le due fasce sottostanti:
- Frangia capillare
	- La zona che contiene parte dell'acqua che risale dalla falda per capillarità
- Zona satura
	- La zona contenente l'acqua - la falda acquifera

Al di sopra di queste due fasce si instaurano i [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Appunti/Moti di filtrazione/02. Moti di Filtrazione\|Moti di Filtrazione]].

In <mark style="background: #D2B3FFA6;">viola</mark> è raffigurato l'andamento dell'umidità in condizioni "di riposo" - quando non piove. In particolare notiamo che l'umidità iniziale è pari a $\color{purple}\theta_{i}$.

Quando comincia a piovere, con [[Università/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Intensità di pioggia\|intensità di pioggia]] $i$, il suolo diventa più umido ma dopo un tempo $t_{1}$ solo un piccolo spessore di suolo risente dell'aumento di umidità: la prima <mark style="background: #FFB86CA6;">linea arancione</mark>. Man mano che passa il tempo l'umidità aumenta sempre di più fino a quando al suolo si raggiunge la saturazione. È a questo punto che può crearsi in superficie un [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Battente idrico\|#Battente idrico]]. Il tempo necessario a raggiungere questa condizione è detto [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Tempo di ponding\|#Tempo di ponding]].

### Modellazione

Lo studio dell'acqua attraverso un mezzo poroso non saturo si affronta classicamente introducendo alcune ipotesi:

```ad-tip
title: Ipotesi

- Il suolo è visto come un mezzo continuo equivalente nel quale coesistono le tre fasi: aria, acqua, scheletro solido.
- Lo scheletro solido è indeformabile
- L'aria all'interno dei meati è costantemente in contatto con l'atmosfera

```

Il terreno risulta caratterizzato da un valore costante di porosità $n(x,y,z)$. 

Si introducono le variabili:
- $\theta(x,y,z,t):$ [[Università/2° anno/1° Semestre/Geologia applicata/Lezioni/07. Proprietà Fisiche delle Rocce#Contenuto d'acqua\|contenuto d'acqua]] volumetrico
- $\boldsymbol{v}(x,y,z,t):$ Vettore della velocità di filtrazione (specific discharge)
	- $v_{j}:$ Componente del vettore velocità rappresentante la portata che attraversa una superficie unitaria di normale $\boldsymbol{\hat{j}}$
	- $H(x,y,z,t) = z+h(x,y,z,t):$ potenziale del campo vettoriale della velocità

