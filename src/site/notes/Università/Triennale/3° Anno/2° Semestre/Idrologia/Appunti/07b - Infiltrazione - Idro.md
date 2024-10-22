---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/idrologia/appunti/07b-infiltrazione-idro/","tags":["UNI"]}
---

# [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro\|07b - Infiltrazione - Idro]]

```ad-Definizione
title: Infiltrazione

L'**infiltrazione** ha luogo attraverso la superficie del suolo durante e dopo gli eventi meteorici.

```


Avviene quando coesistono nello stesso ambiente: aria, acqua e matrice solida.

I fattori che influenzano le modalità di infiltrazione sono vari:
- Quelli che influenzano la **quantità d'acqua disponibile**
	- Tipo di precipitazione (pioggia, neve o grandine)
	- Andamento spazio-temporale dell'intensità della precipitazione
	- Morfologia della superficie del suolo (pendenza dei versanti, presenza di depressioni superficiali)
- Quelli che influenzano l'**attitudine del terreno a lasciare infiltrare l'acqua:**
	- Caratteristiche fisico-chimiche del materiale costituente il suolo (roccia o materiale sciolto, composizione mineralogica, assortimento granulometrico, presenza di una struttura)
	- Uso del suolo (copertura vegetale, presenza di apparati radicali, trattamenti meccanici quali aratura o dissodamento, drenaggi)
	- Condizioni iniziali di umidità



I secondi si possono distinguere in due categorie:
- Fattori **costanti nel tempo** (o variabili su tempi molto lunghi)
	- Morfologia della superficie del suolo
	- Caratteristiche fisico-chimiche del materiale del suolo
- Fattori **dipendenti dal tempo**
	- Condizioni iniziali di umidità del suolo

## Modellazione dell'infiltrazione

I modelli fisico-matematici dell'infiltrazione si riferiscono al moto dell'acqua attraverso un **mezzo poroso omogeneo**.

A una certa profondità dalla superficie del suolo si individua una **superficie libera della falda** che separa la zona in cui il mezzo è completamente saturo d'acqua da quella in cui i meati lasciati liberi dallo scheletro solido sono solo parzialmente occupati da acqua - **Terreno non saturo**

Nei terreni saturi si può applicare la [[Università/Triennale/3° Anno/1° Semestre/Fondamenti di Geotecnica/Appunti/Moti di filtrazione/02. Moti di Filtrazione#Legge di D'Arcy\|Legge di D'Arcy]]. Nel caso di mezzi non saturi entrano in gioco forze di natura capillari di cui la legge di D'Arcy non tiene conto.

Il processo di infiltrazione avviene attraverso la zona *non satura* del terreno (a meno che la superficie libera della falda coincida con la superficie del terreno).

### Definizioni

#### Umidità del suolo

L'**umidità del suolo** è
$$
\theta= \frac{W_{a}}{W_{t}}
$$
dove:
- $W_{a}:$ Volume d'acqua nel suolo
- $W_{t}:$ Volume totale del suolo

La [[Università/Triennale/3° Anno/1° Semestre/Fondamenti di Geotecnica/Appunti/00. Caratteristiche generali delle terre#Porosità\|porosità]]:

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/triennale/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#porosita" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



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

$\theta_{r}$ è detto **contenuto** d'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Acqua di ritenzione\|#Acqua di ritenzione]] e costituisce l'acqua che non si può muovere.


![07b - Infiltrazione - Idro 2024-05-05 16.14.27.excalidraw.png](/img/user/Excalidraw/07b%20-%20Infiltrazione%20-%20Idro%202024-05-05%2016.14.27.excalidraw.png)


![Schermata 2024-05-05 alle 18.07.15.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-05-05%20alle%2018.07.15.png)

Descrivere:
- Falda
- Frangia capillare
- Zona non satura


#### Acqua di ritenzione

```ad-Definizione
title: Acqua di detenzione

L'**acqua di detenzione** o di **ritenzione** è il totale dell'acqua tra adsorbimento, adesione e capillare isolata:
$
W_{r} = \text{adsorbimento} + \text{adesione} + \text{capillare isolata}
$

```

L'acqua di ritenzione non può essere estratta per gravità o pompaggio.

Essa costituisce di fatto il livello minimo di acqua che si trova nel terreno.

#### Acqua libera

```ad-Definizione
title: Acqua libera ($W_{e}$)

$
W_{e} = W_{a} - W_{r}
$
dove:
- $W_{a}:$ [[#Volume d'acqua]]
- $W_{r}:$ [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Acqua di ritenzione\|#Acqua di ritenzione]]
```


#### Porosità efficace

```ad-Definizione
title: Porosità efficace
$
n_{e} = \frac{W_{v}-W_{r}}{W_{t}}
$
dove:
- $W_{v}:$ [[#Volume dei vuoti]]
- $W_{r}:$ [[#Acqua di ritenzione]]
- $W_{t}:$ Volume totale del suolo
```


#### Capacità specifica di detenzione

```ad-Definizione
title: Capacità specifica di detenzione

$
n_{d} = \frac{W_{r}}{W_{t}}
$
dove:
- $W_{r}:$ [[#Acqua di ritenzione]]
- $W_{t}:$ Volume totale del suolo
```


#### Grado di saturazione


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/triennale/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#grado-di-saturazione" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



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



Il diagramma sopra mostra l'andamento dell'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Umidità del suolo\|#Umidità del suolo]] nel sottosuolo. 

Si notino intanto le due fasce sottostanti:
- Frangia capillare (satura)
	- La zona che contiene parte dell'acqua che risale dalla falda per capillarità
- Zona satura
	- La zona contenente l'acqua - la falda acquifera

Al di sopra di queste due fasce si instaurano i [[Università/Triennale/3° Anno/1° Semestre/Fondamenti di Geotecnica/Appunti/Moti di filtrazione/02. Moti di Filtrazione\|Moti di Filtrazione]].

In <mark style="background: #D2B3FFA6;">viola</mark> è raffigurato l'andamento dell'umidità in condizioni "di riposo" - quando non piove. In particolare notiamo che l'umidità iniziale è pari a $\color{purple}\theta_{i}$. $\theta_{i}$ sarà sicuramente maggiore di $\theta_{r}$ (umidità con [[#Acqua di ritenzione]]).

Quando comincia a piovere, con [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Intensità di pioggia\|intensità di pioggia]] $i$, il suolo diventa più umido ma dopo un tempo $t_{1}$ solo un piccolo spessore di suolo risente dell'aumento di umidità: la prima <mark style="background: #FFB86CA6;">linea arancione</mark>. Man mano che passa il tempo l'umidità aumenta sempre di più fino a quando al suolo si raggiunge la saturazione. È a questo punto che può crearsi in superficie un [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Battente idrico\|#Battente idrico]]. Il tempo necessario a raggiungere questa condizione è detto [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Tempo di ponding\|#Tempo di ponding]]. Questo avviene quando l'umidità del suolo eguaglia la porosità (tutti i vuoi sono riempiti d'acqua - saturazione).

Se sul grafico sopra prendo in considerazione una linea orizzontale (a una data profondità) per ogni istante (ovvero per ogni profilo di umidità) posso calcolare la quantità di acqua e aria nel terreno. Questa linea prende il nome di **Fronte di Green-Ampt**. Questo è un approccio adottato per semplificare la modellazione: si ipotizza quindi che, al di sopra del fronte, la $\theta= n$, mentre al di sotto, $\theta=\theta_{i}$

### Modellazione

Lo studio dell'acqua attraverso un mezzo poroso non saturo si affronta classicamente introducendo alcune ipotesi:

```ad-tip
title: Ipotesi

- Il suolo è visto come un **mezzo continuo equivalente** nel quale coesistono le tre fasi: aria, acqua, scheletro solido.
- Lo scheletro solido è **indeformabile**
- L'aria all'interno dei meati è costantemente in contatto con l'atmosfera

```

Il terreno risulta caratterizzato da un valore costante di porosità $n(x,y,z)$. 

Si introducono le variabili:
- $\theta(x,y,z,t):$ [[Università/Triennale/2° anno/1° Semestre/Geologia applicata/Lezioni/07. Proprietà Fisiche delle Rocce#Contenuto d'acqua\|contenuto d'acqua]] volumetrico
- $\boldsymbol{v}(x,y,z,t):$ Vettore della velocità di filtrazione (specific discharge)
	- $v_{j}:$ Componente del vettore velocità rappresentante la portata che attraversa una superficie unitaria di normale $\boldsymbol{\hat{j}}$
	- $h(x,y,z,t) = z+\psi(x,y,z,t):$ potenziale del campo vettoriale della velocità - carico idraulico
		- Carico totale = profondità + **risalita capillare**

![Schermata 2024-07-15 alle 10.40.16.png|350](/img/user/Schermata%202024-07-15%20alle%2010.40.16.png)

L'acqua, per vie delle forze elettriche di adesione alle particelle e di coesione tra molecole d'acqua si incurva formano un **menisco** all'interno del **meato**. L'angolo tra l'acqua e il solido è detto *angolo di contatto*.

La concavità del menisco è dovuta alla differenza di pressione esercitata dall'aria e dall'acqua. In  particolare, la concavità sarà verso l'alto quando la pressione dell'aria è maggiore di quella dell'acqua.

La differenza tra le due pressioni prende il nome di **PRESSIONE CAPILLARE**.

La risalita è dovuta alle pressioni capillari e si ha sotto le ipotesi:
- Meato piccolo abbastanza da permettere le forze capillari
- Pressione dell'aria del meato = pressione atmosferica

![Schermata 2024-07-15 alle 11.09.38.png](/img/user/Schermata%202024-07-15%20alle%2011.09.38.png)

$\psi$, il **carico capillare** risulta essere:
$$
\psi = \frac{p_{air}-p_{wat}}{\gamma_{w}} = - \frac{\alpha T\cos\theta}{\gamma_{wat}r}
$$
dove:
- $\alpha:$ Dipende dalla geometria del meato ($\alpha = 2$ per la circonferenza)
- $r:$ Dimensione caratteristica del meato
- $T:$ Tensione superficiale dell'acqua

Tanto più piccolo è il meato, tanto di più l'acqua risale. In idrologia $h$ è considerato negativo.

Si considera negativo perché la pressione nel meato è minore e quindi c'è tipo **suzione**.


#### Modellazione fisico-matematica

##### Equazione di continuità

Nei mezzi porosi saturi

Si consideri un volume di controllo. Si scriva il bilancio di massa:
$$
\frac{\mathrm{d}}{\mathrm{d}t} \iiint_{V} \rho_{W} \, dV + \iint_{S} \rho_{W} \vec{V}\cdot \vec{ds}  = 0
$$

In forma differenziale diventa:
$$
\rho_{W} \frac{\partial \theta}{\partial t}dxdydz + \rho \left( q+ \frac{\partial q}{\partial z}dz - q \right)dxdy = 0
$$
dove
- $\theta:$ [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Umidità del suolo\|#Umidità del suolo]]
- $q = -k \frac{\partial h}{\partial z}:$ portata secondo D'Arcy

Si ottiene così
$$
\boldsymbol{\frac{\partial \theta}{\partial t} + \frac{\partial q}{\partial z}} = 0
$$

##### Equazione del moto - Equazione di Richards

Ricordando quanto detto nella [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Modellazione\|#Modellazione]] per la capillarità, Il carico totale è dovuto, oltre che da $z$, dal contributo della **capillarità:** $\psi$.

$$
h = z + \psi
$$
dove:
- $h:$ Carico totale (che prima chiamavo $H$)
- $\psi:$ Carico idraulico dovuto alle quote di attrito che si verificano nei mezzi saturi (prima lo indicavo con $h$)

La [[Università/Triennale/3° Anno/1° Semestre/Fondamenti di Geotecnica/Appunti/Moti di filtrazione/02. Moti di Filtrazione#Legge di D'Arcy\|legge di Darcy]] diventa quindi:
$$
q = -k \frac{\partial (\psi +z)}{\partial z} = -k \frac{\partial \psi}{\partial z} - k
$$
Moltiplico e divido per $\partial\theta$ e ottengo:
$$
q = -k \frac{\partial \psi}{\partial \theta} \frac{\partial \theta }\partial z - k
$$
Definisco la **diffusività dell'acqua**
$$
D = k \frac{\partial \psi}{\partial \theta}
$$
e quindi posso scrivere:
$$
q = - \left( D \frac{\partial\theta }{\partial z} +k\right)
$$
Sostituisco la $q$ così trovata nell'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Equazione di continuità\|#Equazione di continuità]] e ottengo l'**equazione del moto**:

```ad-Teo
title: Equazione di Richards - Equazione del moto

L'equazione del moto monodimensionale nei **mezzi porosi NON saturi** in condizioni **non stazionarie**, detta anche *Equazione di Richards* è:

$
\frac{\partial \theta}{\partial t} = \frac{\partial}{\partial z}  \left( D \frac{\partial\theta }{\partial z} +k\right)
$

Che tiene conto della *[[09. Elementi di idrogeologia#Permeabilità|permeabilità]] del terreno* e della *diffusività dell'umidità*
```

L'equazione di Richards è un'equazione NON lineare in quanto sia $D$ che $k$ dipendono da $\theta$. 

Per la non linearità l'equazione di Richards è molto difficile da risolvere. Pertanto si usano di solito modelli semplificati come l'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Equazione di Horton\|#Equazione di Horton]]

##### Equazione di Horton

L'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Equazione del moto - Equazione di Richards\|Equazione di Richards]] può essere integrata abbastanza facilmente supponendo $D$ e $k$ costanti.

```ad-Teo
title: Equazione di Horton

Si ottiene l'Equazione di Horton:
$
f^{*}(t) = f^{*}_{\infty}+(f^{*}_{i}-f_{\infty}^{*}) e^{-kt}
$
dove:
- $f_\infty^{*}:$ Valore limite ($t \to \infty$)
- $f_{i}^{*}:$ Valore iniziale ($t = 0$)
```

L'**intensità di filtrazione potenziale** è quella che si verifica quando si suppone che ci sia acqua in superficie sufficiente ad alimentare l'infiltrazione senza limitazioni.

![Schermata 2024-07-15 alle 12.02.19.png](/img/user/Schermata%202024-07-15%20alle%2012.02.19.png)

L'equazione di Horton fornisce l'infiltrazione potenziale nel terreno. Se l'intensità di pioggia supera la filtrazione potenziale (quella di Horton), la filtrazione del terreno è quella di Horton e la differenza, $p(t)$, è ruscellamento
$$
f(t) =
\begin{cases}
i(t) &\qquad i(t) < f^{*}(t) \\
f^{*}(t) &\qquad i(t) \geq f^{*}(t)
\end{cases}
$$

$$
p(t) =
\begin{cases}
0 &\qquad i(t) < f^{*}(t) \\
i(t) - f^{*}(t) &\qquad i(t) \geq f^{*}(t) 
\end{cases}
$$

Quando si supera il $t_{p}$ ([[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Tempo di ponding\|#Tempo di ponding]]), l'infiltrazione $f(t)$ = 0 e quindi si ha che $p(t) \equiv i(t)$.

###### Intensità di infiltrazione potenziale

È data dall'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Equazione di Horton\|#Equazione di Horton]] e costituisce l'infiltrazione che si avrebbe se ci fosse disponibilità idrica illimitata: quella cioè che dipende solo dalle caratteristiche del terreno
$$
f^{*}(t)
$$


###### Intensità di Infiltrazione effettiva

L'infiltrazione effettiva è quella reale, cioè quella che si verifica effettivamente durante un determinato evento di pioggia.
$$
f(t)
$$

###### Infiltrazione cumulata potenziale

Rappresenta il volume d'acqua che può infiltrare in un dato terreno al tempo $t$:
$$
F^{*}(t) = \int_{0}^{t}f^{*}(t) \, dx 
$$

###### Infiltrazione cumulata effettiva

$$
F(t) = \int_{0}^{t}f(t) \, dx 
$$

##### Modello di Green-Ampt

Il modello di Green-Ampt descrive l'infiltrazione aggiungendo alcune ipotesi all'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Equazione di Horton\|#Equazione di Horton]]. Esso suppone che l'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Umidità del suolo\|#Umidità del suolo]] possa assumere solo 2 valori: $\theta_{s}$ (saturo) e $\theta_{d}$ (asciutto-dry).

In pratica si suppone, come in figura, che il terreno bagnato sia già direttamente saturo e ci sia una superficie di separazione netta (**fronte di Green-Ampt**) con il terreno asciutto. Con l'avanzare della pioggia il fronte procede verso il basso fino a raggiungere la frangia capillare e la falda.

Questo modello inoltre suppone la perenne presenza di un velo idrico in superficie.

L'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Infiltrazione potenziale effettiva\|#Infiltrazione potenziale effettiva]] nel modello di Green-Ampt è descritta dalla seguente:
$$
F(t) = Kt + \psi \Delta \theta \ln\left[  1 + \frac{F(t)}{\psi \Delta \theta}  \right]
$$
Per applicare il modello è necessario conoscere tutti i parametri che compaiono:
- $\eta:$ porosità
- $K:$ permeabilità
- $\psi:$ Carico di suzione
- $\theta_{i}:$ umidità iniziale del terreno

Poiché il velo idrico si forma solo dopo un certo tempo, detto [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Tempo di ponding\|#Tempo di ponding]], si possono distinguere i seguenti casi:
- $t<t_{p}$: l’intensità di pioggia è inferiore alla capacità di infiltrazione e quindi l’infiltrazione reale è pari all’intensità di pioggia.
- $t=t_p$: l’intensità di pioggia supera la capacità di infiltrazione e comincia a formarsi il velo idrico sulla superficie che si satura. IN QUESTO CASO l’infiltrazione reale è pari all’infiltrazione potenziale, ossia alla capacità massima di infiltrazione del terreno
- $t>t_p$: la precipitazione continua e il fronte orizzontale di saturazione si sposta verso il basso. L’intensità di infiltrazione continua ad essere uguale a quella potenziale

Il [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Tempo di ponding\|#Tempo di ponding]] può essere determinato con la seguente formula:
$$
t_{p} = \frac{K\psi \Delta \theta }{i(i-K)}
$$

```ad-attention
title: Attenzione

In realtà, il [[#Modello di Green-Ampt]] così come è stato descritto fino ad ora non tiene conto di un effetto di cui però si ha conto empiricamente.

![Schermata 2024-07-22 alle 16.42.08.png](/img/user/Schermata%202024-07-22%20alle%2016.42.08.png)

Quando inizia a piovere solitamente l'intensità di pioggia è minore all'[[#Intensità di infiltrazione potenziale]]. Come detto l'acqua si infiltra tutta, MA NON SOLO: essa si infiltra più velocemente di quanto previsto dal modello. Pertanto, anche quando, in virtù del modello, l'intensità di pioggia supera l'[[#Intensità di infiltrazione potenziale]], per un certo intervallo di tempo $t_{0}$ l'acqua che precipita continuerà comunque a infiltrarsi tutta. Solo dopo $t_{0}$ si ottiene ruscellamento. È pertanto fondamentale, nell'applicazione del modello, tenere conto di questo fenomeno e traslare la curva di infiltrazione teorica.

```


#### Rifiuto del suolo

##### Principio del catino

Il principio del catino è un metodo attraverso il quale viene studiata l'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro\|Infiltrazione]].

Esso si basa sul considerare il terreno come un invaso il quale, fino a quando non si sia completamente saturato, continuerà ad accettare acqua senza che avvenga il ruscellamento.

$$
f(t)=
\begin{cases}
i(t) &\qquad h(t)\leq C \\
0 &\qquad h(t) > C
\end{cases}
$$
dove:
- $h(t):$ [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Altezza di pioggia\|altezza di pioggia]] complessiva caduta al tempo $t$
- $C:$ Capacità iniziale dell'invaso


##### Metodo SCS - Curve Number (CN)

L'ente statunitense [[Soil Conservation Service - SCS\|Soil Conservation Service - SCS]] ha introdotto, per la valutazione dell'infiltrazione e delle piogge nette, il Curve Number

```ad-Definizione
title: Curve Number

Il **Curve Number** è un parametro usato per stimare la quantità d'acqua che defluisce rispetto a tutta quella che tocca terra.
È compreso tra 0 e 100.
- CN = 100: Terreno impermeabile oppure superficie di acqua (acqua non assorbe acqua)
- CN>0: Superficie naturale

```

Il metodo si basa sui seguenti presupposti:
- La quantità di pioggia netta $P_{n}$ caduta durante un evento meteorico è inferiore o al limite uguale alla quantità totale di pioggia precipitata $P$
- Dopo che inizia il ruscellamento superficiale, la quantità d'acqua addizionale che precipita e si infiltra nel bacino, $F_{a}$ è minore o al limite uguale alla ritenzione potenziale massima $S$ del bacino stesso
- Esiste una certa quantità di afflusso iniziale, $I_{a}$ che viene totalmente infiltrata nel bacino prima del ruscellamento. Il deflusso potenziale è quindi pari a $P-I_{a}$

Inoltre si considera vera questa proporzione
$$
\frac{F_{a}}{S} = \frac{P_{n}}{P-I_{a}}
$$
dove:
- $F_{a}:$ Perdite reali
- $S:$ Perdite potenziali
- $P_{n}:$ Piogge nette - Deflusso reale
- $P:$ Pioggia precipitata
- $I_{a}:$ Afflusso iniziale
- $P-I_{a}:$ Deflusso potenziale

ossia: *"il rapporto tra perdite reali e potenziali è uguale al rapporto tra deflussi reali e potenziali"*

Essendo l'equazione di continuità:
$$
P = P_{e} + I_{a} + F_{a}
$$
dalla quale si può ricavare la pioggia netta (pioggia effettiva) $P_{e}$:
$$
P_{e} = \frac{(P-I_{a})^{2}}{P-I_{a}+S}
$$
Solitamente si considera $I_{a} = 0.2 S$.

$$
S= 254\left(  \frac{100}{CN}-1  \right)
$$

$S$ viene stimato per mezzo del **Curve Number** che dipende da 3 fattori fondamentali:
- [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Tipo di suolo\|#Tipo di suolo]]
- [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Uso del suolo\|#Uso del suolo]]
- [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Stato di imbimbimento\|#Stato di imbimbimento]]

###### Tipo di suolo

![Schermata 2024-07-15 alle 17.05.36.png|350](/img/user/Schermata%202024-07-15%20alle%2017.05.36.png)

###### Uso del suolo

Da rurale a urbano. Assegna valori specifici di CN per ogni [[Università/Triennale/2° anno/2° Semestre/GIS/GIS 1/6. Uso Suolo#Uso del suolo\|uso del suolo]].

###### Stato di imbimbimento

Anche detto Stato iniziale di umidità del terreno. Dipende dalle piogge nei 5 giorni prima.

I valori del CN tabellati in funzione del [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Tipo di suolo\|#Tipo di suolo]] e dall'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Uso del suolo\|#Uso del suolo]] sono riferiti alle condizioni standard di umidità: CN(II).

![Schermata 2024-07-22 alle 16.55.15.png](/img/user/Schermata%202024-07-22%20alle%2016.55.15.png)

