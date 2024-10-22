---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/idrologia/appunti/09-trasformazione-afflussi-deflussi-idro/","tags":["UNI"]}
---


# [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/09 - Trasformazione afflussi-deflussi - Idro\|09 - Trasformazione afflussi-deflussi - Idro]]

Siamo interessati a descrivere i deflussi in un sistema. Ci sono però alcune problematiche:
- Le misure dei deflussi sono raramente disponibili e comunque assai onerose.
- È più problematico regionalizzare i deflussi che non le precipitazioni.
- Il deflusso che si vuole stimare si riferisce spesso a una rete di drenaggio non ancora esistente.

Per questo motivo si vuole definire un **modello afflussi-deflussi**; un modello cioè che sia capace, dati gli afflussi ad un bacino, di restituire le portate di deflusso in chiusura dello stesso.

Gli effetti delle caratteristiche del bacino sulla formazione del deflusso sono classicamente compendiati nei due fenomeni del **ritardo** e dell'**invaso**.
- **Ritardo:** deriva dall'estensione del bacino
- **Invaso:** legato all’attitudine del bacino ad immagazzinare acqua

![09 - Trasformazione afflussi-deflussi - Idro 2024-07-16 11.53.43.excalidraw.png|700](/img/user/Excalidraw-2/09%20-%20Trasformazione%20afflussi-deflussi%20-%20Idro%202024-07-16%2011.53.43.excalidraw.png)


Per ciascun blocco vale la conservazione della massa. Ad esempio, per il suolo:
$$
F - Q_{i} - R - E_{s} = \Delta V_{s}
$$
La differenza tra tutto quello che entra e tutto quello che esce fornisce la variazione di volume del sistema.

## Modellazione afflussi-deflussi

È praticamente impossibile rappresentare la [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/09 - Trasformazione afflussi-deflussi - Idro\|trasformazione afflussi-deflussi]] con un modello fisicamente basato a causa della complessità dei fenomeni in gioco e all'elevato numero di parametri da conoscere.

### Modelli lineari e stazionari

```ad-Definizione
title: Modello lineare

I modelli che sfruttiamo sono, in particolare, **modelli lineari**.

Sia 
$p = K_{1}p' +K_{2}p''$
l’ingresso al sistema costituito dalla combinazione lineare degli ingressi $p'$  e $p''$, gli corrisponde un’uscita
$q = K_{1}q' +K_{2}q''$
anch’essa combinazione lineare delle due uscite $q'$ e $q''$.

```

In realtà ci sono alcuni fenomeni, come l’[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro\|Infiltrazione]], che non possono essere descritti in forma lineare. Se però consideriamo dei casi in cui l’infiltrazione sia trascurabile – come nel caso di terreni impermeabili - possiamo adoperare il modello lineare senza eccessivi problemi. Negli altri casi i modelli lineari possono ancora essere considerati a patto di ignorare la quota-parte dell’acqua che non può essere descritta con linearità.

```ad-Definizione
title: Modello stazionario

Si dice **stazionario** un sistema tale che, a due ingressi uguali sfasati di un certo tempo $dt$, corrispondono due uscite anche loro uguali tra loro, sfasate anch’esse dello stesso $dt$.

```


### Modelli completi

Sono concepiti per rappresentare il comportamento del bacino in qualsiasi situazione idrometeorologica. Simulano la trasformazione A/D in qualsiasi condizione di intensità dell’evento di pioggia. Considerano tutti i fenomeni che contribuiscono alla trasformazione ([[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione\|evapotraspirazione]], [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro\|Infiltrazione]], immagazzinamento negli invasi superficiali...)

Per via della grande complessità del problema, è praticamente impossibile rappresentare la trasformazione afflussi-deflussi attraverso un *modello matematico fisicamente basato*.

Più spesso si ricorre a *[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/09 - Trasformazione afflussi-deflussi - Idro#modelli concettuali\|#modelli concettuali]]*



### Modelli concettuali

```ad-Definizione
title: Modelli concettuali

I **modelli concettuali** schematizzano in via semplificata il comportamento del bacino idrografico, o di uno dei sistemi in esso individuati, con il vantaggio di ridurre enormemente il numero di parametri da stimare.

```


Simulano il comportamento del bacino solo in corrispondenza di eventi di natura particolare. Hanno una struttura più semplificata e non considerano tutti i fenomeni. Ne sono un esempio i modelli di piena che simulano il comportamento del bacino in presenza delle piene.

Il punto debole dei modelli concettuali risiede nella mancanza di un chiaro significato fisico dei parametri che in essi compaiono, il che ne rende difficile la stima. I parametri dei modelli concettuali, pertanto, sono trattati alla stregua di parametri di calibrazione.

Il problema che vogliamo risolvere è:

>Assegnato un bacino idrografico, nota la curva di possibilità pluviometrica rappresentativa della zona in cui esso si trova, si vuole conoscere il deflusso che si accompagna ad un assegnato afflusso meteorico.

#### Modelli di piena


Un tipico approccio al [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/09 - Trasformazione afflussi-deflussi - Idro#Modello concettuale\|#Modello concettuale]] è quello dei **modelli di piena**. Questi studiano il sistema durante un evento piena.

Questi sfruttano il fatto che, durante un evento di pioggia di piena, si possono fare alcune ipotesi:
- L'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione\|evapotraspirazione]] è trascurabile
- Si tiene conto solo delle perdite per [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro\|Infiltrazione]]

La formazione dei deflussi superficiali avviene essenzialmente in 2 modi: 
- **Trasferimento della massa liquida:** la goccia d’acqua che cade sulla superficie scorre a velocità variabile; si presenta alla sezione di chiusura del bacino con le altre gocce dopo un certo tempo dal momento in cui è precipitata 
- **Laminazione della massa liquida:** la pioggia caduta sul bacino si accumula temporaneamente sulla superficie di quest’ultimo come se fosse un serbatoio.

Le perdite sono calcolati con il [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/09 - Trasformazione afflussi-deflussi - Idro#Coefficiente di deflusso\|#Coefficiente di deflusso]].

Per quanto riguarda i modelli di piena, la durata dei fenomeni da modellare, che dipende dalle dimensioni del bacino, è di solito molto limitata, dell'ordine delle ore o, per bacini molto estesi, dei giorni. Ciò implica che a rigore non sarebbe possibile definire un coefficiente di deflusso rappresentativo del comportamento del bacino in qualsiasi condizione. In altre parole, il deflusso attraverso la sezione di chiusura di un assegnato bacino, conseguente ad un identico afflusso di pioggia, non è sempre lo stesso in quanto dipende dalle condizioni in cui si trova il bacino allinizio della precipitazione.




❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ ATTENZIONE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

Da qui in poi leggere direttamente nello [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/10 - IUH - Idro\|IUH]].


### Pioggia netta


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/triennale/3-anno/2-semestre/idrologia/appunti/06-perdite-idro/#pioggia-netta" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Pioggia netta

```ad-Definizione
title: Pioggia netta

La **pioggia netta** è la differenza tra la pioggia e le [[#Perdite idrogeologiche]]:
$
p(t) = i(t) - e(t) - v(t)- s(t) - f(t)
$
dove:
- $p(t):$ [[02 - Piogge Intense - Idro#Intensità di pioggia|intensità di pioggia]] netta
- $i(t):$ [[02 - Piogge Intense - Idro#Intensità istantanea di pioggia|Intensità di pioggia]] lorda
- $e(t):$ Intensità di [[#Evapotraspirazione]]
- $\nu(t):$ Intensità di [[#Intercettazione della vegetazione]]
- $s(t):$ Intensità di [[#Invaso nelle depressioni]]
- $f(t):$ Intensità di [[07b - Infiltrazione - Idro|Infiltrazione]]

```


In realtà alcuni di questi termini possono essere trascurati:
$
p(t) = i(t) - \cancel{e(t)} - \cancel{v(t)} - s(t) - f(t)
$
Elimino:
- Su scala annuale: trascuro $v(t)$
- Negli eventi di piena: trascuro $e(t)$

In particolare quando piove e se considero una scala annuale.
$
p(t) = i(t) - s(t) - f(t)
$



</div></div>


Posso introdurre il [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/07b - Infiltrazione - Idro#Curve Number\|Curve Number (CN)]] che permette la valutazione delle perdite tenendo conto della precipitazione caduta nei 5 giorni precedenti.

Questo si fa solo se l'evento di pioggia è reale, non probabilistico.

Se l'evento è probabilistico introduco il concerto di **pioggia netta** definito a partire dal [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/09 - Trasformazione afflussi-deflussi - Idro#Coefficiente di afflusso\|#Coefficiente di afflusso]]

### Modello cinematico

Il **modello cinematico** è un modello concettuale molto semplice basato su alcune ipotesi semplificative:
- La formazione della piena è dovuta solo al trasferimento di volumi d'acqua all'interno del bacino;
- Ogni goccia di pioggia che cade sulla superficie segue un percorso invariabile nel tempo e che dipende solo dal punto in cui essa è caduta;
- La velocità con cui la goccia si muove lungo la superficie non è influenzata dalla presenza di altre gocce;
- La portata nella sezione di chiusura in un dato istante è data dalla somma delle portate elementari, provenienti dalle diverse parti del bacino, che pervengono alla sezione di chiusura in quellistante.

È escluso qualsiasi fenomeno di invaso. Il tempo di corrivazione è assunto costante. Il modello lineare.

	In teoria c'è anche l'ipotesi che non ci sono perdite. Forse lo dice nelle ipotesi prima ma non si capisce bene.

$$
Q(t) = \int_{A} i(x,y,t-t_{c})  \, dA
$$
Si introduce la **curva tempi-aree** - $A(\overline{t_{c}})$: Rappresenta l'area del bacino con tempo di corrivazione $t_{C} \leq \overline{t_{c}}$.
$$
Q(t) = \int_{0}^{T_{c}} i(x,y,t-t_{c}) \, \frac{dA}{dt_{c}} dt_{c}
$$
La derivata della curva tempi area prende il nome di **curva di concentrazione**.


### Modellazione concettuale della trasformazione afflussi-deflussi

Il pluviogramma in ingresso subisce una serie di trasformazioni per riprodurre l'idrogramma in uscita.


#### Modello dell'invaso lineare

Usato nella progettazione delle fognature. Trascura il ritardo. 

In un serbatoio lineare, in ogni istante, la portata uscente è:
$$
kQ(t) = W(t)
$$
dove:
- $k:$ costante di tempo - caratteristica particolare del serbatoio

Per l'equazione di continuità:
$$
(P(t) - Q(t))dt = dW(t)
$$
Sostituendo a $W(t)$ la quantità $kQ(t)$ otteniamo:
$$
k \frac{dQ(t)}{dt} + Q(t) = P(t)
$$

L'integrale generale di questa diventa:
$$
Q(t) = \int_{0}^{t} P(\tau) \frac{1}{k} e^{-\dfrac{(t-\tau)}{k}}d\tau  + Q_{0}e^{- \dfrac{t}{k}} \, dx 
$$
Il primo addendo prende il nome di **integrale di convoluzione** (vd. anche [[Università/Triennale/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/03. Reattori Ideali#Integrale di convoluzione\|integrale di convoluzione]]) mentre il secondo addendo esiste solo se, a $t=0$ esiste una portata non nulla $Q_{0}$
$$
Q(t) = P\left(1 - e^{\frac{t}{k}}\right) + Q_{0}e^{- \frac{t}{k}}
$$


## Definizioni utili

### Coefficiente di deflusso

La prima grande semplificazione che spesso si introduce riguarda il modo in cui si tiene conto di tutti i processi fisici che fanno sì che l'afflusso meteorico che perviene al bacino idrografico in un assegnato intervallo di tempo non si trasformi completamente in deflusso attraverso la sua sezione di chiusura.

Rapporto tra il deflusso attraverso la sezione di chiusura di un bacino e l'afflusso meteorico allo stesso bacino, in un assegnato intervallo di tempo.
$$
\Phi = \frac{D}{A} <1
$$


### Coefficiente di afflusso

Il coefficiente di afflusso rappresenta il rapporto istantaneo tra la portata che attraversa la sezione di chiusura nel bacino e la portata che, nello stesso istante, perviene al bacino sotto forma di precipitazione.
$$
\varphi = \frac{Q}{P}
$$










