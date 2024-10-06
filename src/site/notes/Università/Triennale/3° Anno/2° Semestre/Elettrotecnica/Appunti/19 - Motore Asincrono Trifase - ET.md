---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/19-motore-asincrono-trifase-et/","tags":["UNI"]}
---

# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|19 - Motore Asincrono Trifase - ET]]

Nella figura sottostante è mostrato lo schema di una **macchina asincrona trifase**.

![19 - Schema costruttivo di una macchina asincrona trifase- ET 2024-07-03 12.58.18.png](/img/user/Excalidraw/19%20-%20Schema%20costruttivo%20di%20una%20macchina%20asincrona%20trifase-%20ET%202024-07-03%2012.58.18.png)


Il motore è costituito da:
- 6 cave interno statore
- 6 cave esterno rotore
In realtà sono molte di più, ma a livello didattico ha senso studiare un motore in questa configurazione.

Vi saranno pertanto:
- 3 avvolgimenti statorici (**induttore**)
- 3 avvolgimenti rotorici (**indotto**)
sfasati spazialmente di 120°

Gli avvolgimenti rotorici sono in genere connessi a stella.

Lo schema di un motore reale è riportato nella figura sottostante:

![Schermata 2024-07-03 alle 13.08.40.png](/img/user/Schermata%202024-07-03%20alle%2013.08.40.png)

Quando nelle spire passa corrente, si genera un [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/18 - Campo magnetico rotante - ET\|campo magnetico rotante]].

## Principio di funzionamento

Partiamo a macchina ferma. Alimentiamo i conduttori statorici e si genera un campo magnetico rotante che comincia a investire in sequenza i conduttori rotorici.

Nella prima investitura del conduttore rotorico. Si trova investita da un campo magnetico B a velocità angolare $\omega_{s}$. Varia continuamente il flusso di questo campo dando origine a una f.e.m. indotta. La spira è cortocircuitata su se stessa. Costituisce un percorso chiuso. Alla fem indotta corrisponde una corrente. Lo stesso avviene alle altre 2 spire.

Sule spire rotoriche, scorrono 3 correnti:
$$
i_{1r},\, i_{2r},\, i_{3r}
$$
Anche queste 3 correnti sono sfasate di 120° e costituiscono una terna trifase (se le spire sono uguali).

La pulsazione di queste correnti la chiamiamo $\omega_{2}$.

Sui lati attivi delle spire, troveremo le forze di Laplace. Il rotore comincerà allora a ruotare. Ricordo che il rotore non è alimentato. La velocità di rotazione del rotore è $\Omega_{rot}$.

```ad-note
title: Osservazione

Velocità angolari
- Campo magnetico statorico ruota a $\omega_{s}$
- Velocità angolare del rotore - $\Omega_{rot}$
**Tutte le altre $\omega$ sono pulsazioni**
```

Essendo le 3 correnti $i_{1r},\, i_{2r},\, i_{3r}$ un sistema trifase equilibrato. Allora anche queste produrranno un campo di induzione rotante $\vec{B}_{r}$ (campo magnetico rotorico). Questo, nel sistema di riferimento del rotore, risulta rotante a velocità angolare $\omega_{r2}$:
$$
\omega_{r2} = \frac{\omega_{2}}{p}
$$
dove $p$ è il numero di coppie polari.

Ricapitolando le grandezze:
- $\omega:$ **pulsazione** delle grandezze *statoriche*
- $\omega_{2}:$ **pulsazione** delle grandezze *rotoriche*

- $\omega_{s}:$ **velocità angolare** del *campo statorico*
- $\omega_{2r}:$ **velocità angolare** del *campo rotorico* (nel SR solidale con il rotore)
- $\omega_{R}:$ **velocità angolare** del *campo rotorico* nel sistema di riferimento statorico
- $\Omega_{R}:$ **velocità angolare** del *rotore*, nel riferimento statorico

### Funzionamento a rotore bloccato

Immaginiamo che la spira sia bloccata, in modo che non possa muoversi. Questa è comunque spazzata da un campo rotante.

![19 - Funzionamento MAT a rotore bloccato - ET 2024-07-03 17.42.21.png](/img/user/Excalidraw/19%20-%20Funzionamento%20MAT%20a%20rotore%20bloccato%20-%20ET%202024-07-03%2017.42.21.png)


Il campo magnetico statorico $\vec{B}_{s}$ ruota a velocità angolare $\omega_{s}$. La spira è bloccata. Su di essa, per via del campo magnetico, scorre una corrente $\overline{I}_{r}$.

Sia:
- $S:$ area della spira
- $\alpha(t) = \omega_{s}t:$ angolo tra $\hat{n}$ e $\vec{B}_{s}$

Posso scrivere il flusso associato alla spira come:
$$
\phi_{r} (t) = \iint_{S} \vec{B}_{s} \cdot \hat{n} \, dS = B_{s}S\cos\alpha  = B_{s}S\cos(\omega_{s}t)
$$
e quindi si avrà una fem indotta pari a:
$$
e_{r}(t) = - \frac{\mathrm{d}\phi_{r}}{\mathrm{d}t}  = \omega_{s}B_{s}S\sin(\omega_{s} t) 
$$
Pertanto, la pulsazione delle grandezze rotoriche, data un'unica coppia polare è pari alla velocità angolare del campo inducente (statorico)
$$
\omega_{20} = \omega_{s}
$$
(lo $0$ indica la configurazione di **rotore bloccato**)

In generale, per $p$ coppie polari:
$$
\omega_{20}  = p\omega_{s}
$$

### Funzionamento a rotore libero

Quando il rotore si trova in rotazione a velocità angolare $\Omega_{rot}$ l'espressione della pulsazione delle grandezze rotoriche $\omega_{2}$ cambia: questo è dovuto al fatto che varia anche la velocità di rotazione del campo statorico che investe gli avvolgimenti.

Infatti, se mi posiziono in un SR solidale al rotore, vedrò ruotare il campo magnetico a velocità angolare:
$$
\omega_{s}-\Omega_{rot}
$$
Pertanto, la pulsazione delle correnti rotoriche per $p$ coppie polari sarà:
$$
\omega_{2} = p(\omega_{s}-\Omega_{rot})
$$
cui corrisponde una velocità angolare. Quindi, la velocità angolare del campo rotorico $\vec{B}_{r}$ sarà:
$$
\omega_{r2} = \frac{\omega_{2}}{p} = \omega_{s}-\Omega_{rot}
$$
Guardiamo ora il sistema dal sistema di riferimento fisso dello statore. La velocità angolare $\omega_{R}$ del campo rotorico nel sistema di riferimento fisso è:
$$
\begin{align}
\omega_{R} &= \omega_{r2} + \Omega_{rot} = \\
&= (\omega_{s}-\Omega_{rot}) + \Omega_{rot} = \omega_{s}
\end{align}
$$
Ossia, la velocità angolare del campo rotorico è uguale alla velocità angolare del campo statorico:
$$
\omega_{R} = \omega_{s}
$$
Al traferro, i due campi ruotano esattamente alla stessa velocità (sono **sincroni**) e danno luogo a un campo totale pari alla somma dei due.

#### Condizione di sincronismo

In realtà, i campi rotorico e statorico sono sincroni solamente in fase di avviamento, ammesso cioè che il rotore sia fermo ($\Omega_{rot} = 0$).

Infatti, la pulsazione delle grandezze rotoriche, $\omega_{2}$ è legata alla pulsazione delle grandezze statoriche $\omega$ secondo:
$$
\omega_{2} = p(\omega_{s}-\Omega_{rot}) = \omega - p\Omega_{rot}
$$
ricordando ($\omega = p\omega_{s}$)

Pertanto, $\omega = \omega_{2}$ se e solo se $\Omega_{rot} = 0$ (avviamento),

In generale $\omega_{2}<\omega$.

Quando il rotore ruota così velocemente da ruotare a $\omega_{s}$, la pulsazione delle grandezze rotoriche va a 0.
$$
\omega_{2} = p(\omega_{s}-\Omega_{rot}) \stackrel{\Omega_{rot}\to\omega_{s}}{\to}  0
$$
In questa condizione allora anche le forze di Laplace vanno a zero. Pertanto, per via dell'attrito, il rotore rallenta la sua velocità di rotazione. Se il rotore rallenta: $\omega_{2}\ne 0$: c'è differenza tra $\omega_{s}$ e $\Omega_{rot}$ --> si restaurano le forze di laplace.

La **condizione di sincronismo**, ossia quando la velocità di rotazione del rotore $\Omega_{rot}$ è uguale alla velocità di rotazione del campo magnetico (statorico o rotorico, tanto loro sono sempre uguali), è una condizione puramente ideale. 

Pertanto, il rotore insegue perennemente il campo magnetico rotante senza poterlo mai raggiungere. Per questo motivo il motore si chiama asincrono: c'è sempre sfasamento tra rotore e campo rotante.

##### Scorrimento

In condizioni reali di funzionamento, si ha sempre che il rotore ruota più lentamente del campo magnetico:
$$
\Omega_{rot} < \omega_{s}
$$
Per quantificare questo sfasamento si definisce lo scorrimento:

```ad-Definizione
title: Scorrimento o slittamento ($s$)

Lo scorrimento o slittamento è
$
s = \frac{\omega_{s}-\Omega_{rot}}{\omega_{s}}
$
e rappresenta la frazione di giro che perde il rotore per ogni giro del campo magnetico. Quantifica di quanto il rotore rimane indietro.

```

Lo scorrimento si può esprimere anche in termini di giri al minuto:
$$
s = \frac{n_{s}-n_{rot}}{n_{s}}
$$
dove
$$
n_{s} = \frac{60\omega}{2\pi p} = \frac{60f}{p}
$$
```ad-tip

In condizione di avviamento:
$
\Omega_{rot} = 0 \qquad\Longrightarrow\qquad s = 1
$

In [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Condizione di sincronismo\|#Condizione di sincronismo]]
$
\Omega_{rot} = \omega_{s} \qquad\Longrightarrow\qquad s = 0
$

```

### Fase di avviamento

Vedendo gli avvolgimenti come degli induttori, si può rappresentare il circuito equivalente come segue:

![19 - Motore Asincrono Trifase - ET 2024-07-03 18.59.43.png](/img/user/Excalidraw/19%20-%20Motore%20Asincrono%20Trifase%20-%20ET%202024-07-03%2018.59.43.png)


A [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Funzionamento a rotore bloccato\|rotore bloccato]] si ha semplicemente trasferimento di potenza elettrica per accoppiamento elettromagnetico e la macchina si comporta come un [[Trasformatore\|Trasformatore]] con il secondario in corto circuito. --> Abbiamo un **trasformatore trifase**

#### Circuito equivalente monofase a rotore bloccato

![19 - Circuito equivalente monofase a rotore bloccato ET 2024-07-03 19.04.48.png](/img/user/Excalidraw/19%20-%20Circuito%20equivalente%20monofase%20a%20rotore%20bloccato%20ET%202024-07-03%2019.04.48.png)


- $\overline{V}_{1}:$ tensione con cui alimento le fasi statoriche
- $R_{s}:$ Resistenza sugli avvolgimenti statorici che tiene conto dell'effetto joule
- $X_{ds}:$ Reattanza degli avvolgimenti statorici - reattanza di dispersione - flusso non concatenato
- $X_{dr}:$ Reattanza degli avvolgimenti rotorici - reattanza di dispersione - flusso non concatenato
- $R_{r}:$ Perdite per effetto Joule sul circuito rotorico
- $X_{0}:$ Perdite di potenza reattiva dovuta alla magnetizzazione dei nuclei (statore e rotore)
- $R_{0}:$ Perdite di potenza attiva (correnti parassite e per isteresi) nei due nuclei (statore e rotore)

La magnetizzazione del nucleo qui è diversa. In mezzo, per far funzionare la macchina, ci deve essere un traferro che separa il nucleo: le reattanze di dispersione sono più consistenti del trasformatore classico.

A rotore bloccato, la pulsazione delle grandezze indotte rotoriche è proprio $\omega$. Allora, proprio come nel trasformatore, è rispl,kytettata l'ipotesi di isofrequenzialità.

Si ha quindi:
$$
\overline{I}_{2} = \frac{\overline{E}_{20}}{(R_{r}+jX_{dr})}
$$
#### Circuito equivalente monofase a rotore libero

A rotore libero:
- Il circuito di statore rimane equivalente
- Il circuito di rotore lavora a pulsazione $s$ volte quella del circuito statorico

![19 - Circuito equivalente monofase a rotore libero - ET 2024-07-03 19.18.35.png](/img/user/Excalidraw/19%20-%20Circuito%20equivalente%20monofase%20a%20rotore%20libero%20-%20ET%202024-07-03%2019.18.35.png)


Sia $\phi_{r}$ il flusso concatenato con la generica spira rotorica:
$$
\overline{E}_{2s} = -j \underbrace{\omega_{2}}_{\omega_{2} = s\omega} \overline{\phi }_{r} = s \underbrace{(-j\omega \overline{\phi }_{r})}_{\overline{E}_{20}}
$$
dove:
- $\overline{E}_{20}:$ fem a rotore bloccato
e quindi
$$
\overline{E}_{2s} = s\overline{E}_{20}
$$
Anche per la reattanza
$$
X_{drs} = \omega_{2}L_{dr} = s\omega L_{dr} = sX_{dr}
$$

Scriviamo [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] al circuito rotorico:
$$\large
\begin{align}
\overline{E}_{2s} &= (R_{r}+jX_{rds})\cdot \overline{I}_{2}  \\
{\color{red} s} \overline{E}_{20} &= (R_{r}+j{\color{red} s}X_{rd})\cdot \overline{I}_{2} \\
\overline{E}_{20} &= \left( \frac{R_{r}}{s} + jX_{rd} \right)\cdot \overline{I}_{2}
\end{align}
$$
Tenuto conto che
$$
\frac{R_{r}}{s} = \frac{R_{r}}{s} + R_{r}-R_{r} = R_{r} \frac{1-s}{s} + R_{r}
$$
Definisco una **resistenza equivalente** $R_{e}$
$$
R_{e} \stackrel{\triangle}{=} R_{r} \frac{1-s}{s}
$$
Questa resistenza è funzione dello [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Scorrimento\|#Scorrimento]]. È quindi una resistenza variabile e definisce il **carico meccanico** del motore.

![19 - Circuito equivalente monofase a rotore libero con resistenza equivalente - ET 2024-07-04 11.55.19.png](/img/user/Excalidraw/19%20-%20Circuito%20equivalente%20monofase%20a%20rotore%20libero%20con%20resistenza%20equivalente%20-%20ET%202024-07-04%2011.55.19.png)


E quindi, riscrivendo la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] tenendo conto della resistenza equivalente:
$$
\overline{E}_{20} = \left( R_{r} + X_{dr} \right) \overline{I}_{2} + R_{e}\overline{I}_{2}
$$
La corrente $\overline{I}_{2}$ resta invariata.

Il circuito equivalente monofase, rappresentando le grandezze in funzione dello scorrimento, diventa:

![19 - Circuito equivalente monofase a rotore libero in funzione di scorrimento - ET 2024-07-04 12.01.12.png](/img/user/Excalidraw/19%20-%20Circuito%20equivalente%20monofase%20a%20rotore%20libero%20in%20funzione%20di%20scorrimento%20-%20ET%202024-07-04%2012.01.12.png)


In questo modo possiamo rappresentare le varie grandezze. In particolare, la resistenza equivalente, assumerà valori diversi nella [[#Condizione di sincronismo]] e nella [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Circuito equivalente monofase a rotore bloccato\|condizione di rotore bloccato]]:
$$
\begin{cases}
R_{e}&= 0 \qquad &\Omega_{rot}=0,  &s = 1,  &\frac{1-s}{s} = 0  &\text{Rotore bloccato} \\
R_{e} &= \infty  \qquad &\Omega_{rot}=\omega_{s},  &s = 0,  &\frac{1-s}{s} = \infty  &\text{Sincronismo}
\end{cases}
$$
##### Potenza in condizione di rotore libero - MAT

**Potenza attiva**:

![19 - Potenza attiva MAT - ET 2024-07-04 12.08.45.png](/img/user/Excalidraw/19%20-%20Potenza%20attiva%20MAT%20-%20ET%202024-07-04%2012.08.45.png)



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



## Flussi di potenza attiva nel MAT

$P_{e}:$ Potenza attiva all'ingresso.

Alimentiamo la fase statorica con una potenza $P_{e}$. Questa potenza va:
- $P_{Js}:$ Dispersa per effetto Joule negli avvolgimenti dello statore - in $R_{s}$
- $P_{Fe} = P_{is}+P_{cp}:$ Dispersa al nucelo = Perdite per isteresi + perdite per correnti parassite - in $R_{0}$ e $X_{0}$

La potenza che arriva al circuito secondario (rotore) è $P_{s}$ = **potenza sincrona**. Questa va:
- $P_{Jr}:$ Dispersa per effetto Joule negli avvolgimenti del rotore
- $P_{m};$ la parte restante costituisce il carico meccanico a $R_{e}$ - La potenza meccanica che vogliamo avere

La potenza in ingresso deve essere la somma di tutte le potenze disperse sullo statore e sul rotore.
$
P_{e} = P_{Js} + \underbrace{P_{is}+P_{cp}}_{P_{Fe}} + P_{Jr} + P_{m}
$
Alla potenza meccanica devo però sottrarre perdite per attrito e per ventilazione: $P_{av}$
$
P_{m} = P_{av}+P_{u}
$
La potenza $P_{u}$ è la **potenza utile**.

Si può così definire il **rendimento del MAT**:
$
\eta = \frac{P_{u}}{P_{e}}
$
Nel [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]] il rendimento si aggira intorno al:
- $\eta \sim 60\%:$ per piccoli motori
- $\eta \sim 97\%:$ per grandi motori











</div></div>



___


**Potenza reattiva**:

![19 - Potenza reattiva MAT - ET 2024-07-04 12.26.36.png](/img/user/Excalidraw/19%20-%20Potenza%20reattiva%20MAT%20-%20ET%202024-07-04%2012.26.36.png)



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



## Flussi di potenza reattiva nel MAT

In termini di [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|potenza reattiva]] si ha che al sistema è fornita una potenza in ingresso $Q_{in}$.

La potenza in ingresso si divide come:
- $Q_{ds}:$ Potenza di flusso disperso allo statore
- $Q_{0}:$ Potenza di magnetizzazione del nucleo

La potenza reattiva rimanente si perde tutta come dispersione nelle maglie rotoriche: $P_{dr}$.

Sono tutte positive:
$
Q_{in} = Q_{ds} + Q_{dr} + Q_{0} >0
$
Appare come un carico Ohmico-Induttivo (potrebbe essere necessario un rifasamento)





</div></div>


## Caratteristica meccanica

Sia il [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Circuito equivalente monofase a rotore libero\|#Circuito equivalente monofase a rotore libero]] quello riportato in figura:

![19 - Circuito equivalente monofase a rotore libero con resistenza equivalente - ET 2024-07-04 11.55.19.png](/img/user/Excalidraw/19%20-%20Circuito%20equivalente%20monofase%20a%20rotore%20libero%20con%20resistenza%20equivalente%20-%20ET%202024-07-04%2011.55.19.png)

Abbiamo detto essere
$$
R_{e} = R_{r} \frac{1-s}{s}
$$
Pertanto, la potenza meccanica del [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]] in presenza di 3 coppie polari, è data da:
$$
P_{m} = 3R_{e}I_{2}^{2}
$$
dalla quale si ricava la [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Potenza meccanica - MAT\|#Potenza meccanica - MAT]]

L'[[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|impedenza]] totale del circuito di rotore è:
$$
\begin{align}
\dot{Z}_{r} &= R_{r} + jX_{dr} + R_{r} \frac{1-s}{s} =  \\
&= \frac{R_{r}}{s} + jX_{dr}
\end{align}
$$
La corrente che scorre sull'avvolgimento rotorico è:
$$
\overline{I}_{2} = \frac{\overline{E}_{20}}{\dot{Z}_{r}}
$$
in valore efficace e al quadrato:
$$
I_{2}^{2} =  \frac{E_{20}^{2}}{Z_{r}^{2}} = \frac{E^{2}_{20}}{\frac{R_{r}^{2}}{s^{2}} + X_{dr}^{2}}
$$


### Coppia meccanica - MAT

In generale, la potenza di un organo rotante è legata alla coppia, dalla velocità angolare:
$$
P = C\Omega 
$$

```ad-Definizione
title: Coppia meccanica ($C_m$)

La **coppia meccanica** del [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]] è
$
C_{m} = \frac{P_{m}}{\Omega_{rot}}
$
dove:
- $\Omega_{rot}:$ Velocità angolare del rotore (nel riferimento statorico)
- $P_{m}:$ [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Potenza meccanica - MAT\|#Potenza meccanica - MAT]]

```

Si ricordano le relazioni:
$$
\Omega_{rot} = (1-s)\omega_{s}
$$
dove:
- $\omega_{s}:$ **velocità angolare** del *campo statorico*
- $\Omega_{R}:$ **velocità angolare** del *rotore*, nel riferimento statorico
in cui
$$
\omega_{s} = \frac{\omega}{p}
$$
dove:
- $\omega:$ **pulsazione** delle grandezze *statoriche*
- $p:$ numero di coppie polari

Pertanto si può scrivere la velocità angolare del rotore come
$$
\Omega_{rot} = (1-s) \frac{\omega}{p}
$$
Sostituendo nell'espressione della coppia meccanica l'espressione di $\Omega_{rot}$ insieme a quella della [[#Potenza meccanica - MAT]]:
$$
\begin{align}
C_{m} &= \frac{P_{m}}{\Omega_{rot}} \cdot I_{2}^{2}= \\
&= \frac{3R_{r} \frac{\cancel{(1-s)}}{s}}{\cancel{(1-s)} \frac{\omega}{p}} \cdot \frac{E^{2}_{20}}{\frac{R_{r}^{2}}{s^{2}} + X_{dr}^{2}}= \\
&= \frac{3R_{r}p}{\omega \cancel{s}} \cdot \frac{E^{2}_{20}}{\frac{R_{r}^{2}}{s^{\cancel{2}}} + sX_{dr}^{2}}
\end{align}
$$
In definitiva, la Coppia Meccanica può essere scritta come:
$$
C_{m} = \frac{3p}{\omega} \frac{R_{r}}{\dfrac{R_{r}^{2}}{s} + sX_{dr}^{2}} \cdot E^{2}_{20}
$$
Si osservi che la coppia meccanica scala con il quadrato della tensione al secondario a vuoto. Scala inoltre linearmente col numero di poli (all'aumentare del numero di poli, diminuisce la velocità, ma aumenta la coppia).

Tra i dati di targa del motore, non viene data la tensione al secondario. Viene solo detto a che tensione va alimentato: quella da applicare agli avvolgimenti statorici. Se trascuriamo le cadute di tensione degli avvolgimenti (impedenza avvolgimenti << impedenza nucleo), allora possiamo scrivere:
$$
\overline{E}_{10} \approx \overline{V}_{1}
$$
tensione indotta al primario simile alla tensione applicata agli avvolgimenti statorici (alimentazione)

Il rapporto tra le tensioni indotte al primario e al secondario è uguale al [[Trasformatore#Rapporto di trasformazione\|rapporto di trasformazione]] ($=m$).
$$
m = \frac{E_{10}}{E_{20}}
$$
E quindi $k$ $\left( \frac{1}{m^{2}} \right)$:
$$
k = \frac{1}{m^{2}} = \frac{E_{20}^{2}}{E_{10}^{2}}
$$

Quindi la coppia meccanica può essere riscritta in funzione di $V_{1}\approx E_{10}$:
$$
C_{m} = \frac{3p}{\omega} \frac{R_{r}}{\dfrac{R_{r}^{2}}{s} + sX_{dr}^{2}} \cdot E^{2}_{20} = C_{m} = \frac{3pk}{\omega} \frac{R_{r}}{\dfrac{R_{r}^{2}}{s} + sX_{dr}^{2}} \cdot V^{2}_{1}
$$


#### Caratteristica coppia scorrimento

#UNI/ET/Domanda 

La [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Coppia meccanica - MAT\|#Coppia meccanica - MAT]] può essere quindi espressa come:
$$
C_{m}(s)  = \frac{3pk}{\omega} \frac{R_{r}}{\dfrac{R_{r}^{2}}{s} + sX_{dr}^{2}} \cdot V^{2}_{1}
$$
di cui si segnalano le seguenti 2 condizioni particolari:
$$
C_{m}=
\begin{cases}
\text{Avviamento} \quad\longrightarrow\quad s=1 \, (\Omega_{rot} = 0) \quad\longrightarrow\quad C_{s} = C_{avv} = \dfrac{3pk}{\omega} \dfrac{R_{r}}{R_{r}^{2} + X_{dr}^{2}} \cdot V^{2}_{1} \\
\text{Sincronismo} \quad\longrightarrow\quad s=0 \, (\Omega_{rot} = \omega _{s}) \quad\longrightarrow\quad C_{m} = 0
\end{cases}
$$
La coppia di Avviamento è anche detto **coppia di spunto**.

Graficando l'andamento della coppia meccanica in funzione dello [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Scorrimento\|#Scorrimento]].

![19 - Caratteristica meccanica coppia-scorrimento MAT - ET 2024-07-04 15.23.57.png](/img/user/Excalidraw/19%20-%20Caratteristica%20meccanica%20coppia-scorrimento%20MAT%20-%20ET%202024-07-04%2015.23.57.png)



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



###### Punto di massimo

Il punto di massimo della coppia si può trovare cercando il minimo del denominatore dell'espressione di $C_{m}(s)$.
Infatti, nell'espressione, tutti i termini sono positivi e il numeratore non varia con $s$.
$
\frac{\mathrm{d}}{\mathrm{d}s}\left(  \frac{R^{2}_{r}}{s} + sX_{dr}^{2}  \right) \stackrel{!}{=} 0
$
Da cui si ottiene
$
-\frac{R^{2}_{r}}{s^{2}} + X_{dr}^{2} = 0
$
che fornisce:
$
s = \pm \frac{R_{r}}{X_{dr}}
$
Quando la macchina funziona da motore, $s\ge0$ (Sarebbe negativo se la macchina funzionasse da generatore).

Si ottiene quindi che lo scorrimento corrispondente al massimo della coppia si ha per:
$
s_{MAX}= \frac{R_{r}}{X_{dr}}
$
```ad-note
title: Osservazione
Posso spostare la posizione del massimo della coppia variando le resistenze

```

In genere $s_{MAX}$ è molto piccolo, compreso tra $1\div10\%$, essendo la macchina progettata per minimizzare le perdite per [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/04 - Fenomeni di conduzione e resistori - ET#Potenza dissipata per Effetto Joule\|effetto Joule]] (e quindi progettata con $R_{r}$ piccoli).

La coppia massima associata al [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]] è quindi:
$
C_{MAX} = C_{m}(s_{MAX}) = \frac{3pk}{2\omega } \cdot \frac{1}{X_{dr}} \cdot V_{1}^{2}
$
dove si osservi che $C_{MAX}$:
- Aumenta al diminuire di $X_{dr}$
- Non dipende da $R_{r}$





</div></div>





### Potenza meccanica - MAT

Abbiamo detto essere
$$
R_{e} = R_{r} \frac{1-s}{s}
$$

```ad-Definizione
title: Potenza meccanica ($P_{m}$)

La **potenza meccanica** consegnata alla resistenza equivalente del rotore del [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]] in presenza di 3 coppie polari, è data da:
$
P_{m} = 3R_{e}I_{2}^{2}
$


```

### Stabilità della caratteristica meccanica

#UNI/ET/Domanda 

Immaginiamo di avere il [[19 - Motore Asincrono Trifase - ET|MAT]] inizialmente funzionante, a regime. Sta lavorando a una coppia pari alla coppia resistente (che si oppone al moto del rotore)
$$
C_{r} = C_{m}
$$
#### Funzionamento instabile

```ad-Definizione
title: Funzionamento instabile

Si parla di **funzionamento instabile** del [[19 - Motore Asincrono Trifase - ET|MAT]] quando questo lavora con un valore di [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Scorrimento\|#Scorrimento]] *maggiore* a quello di massimo della coppia:
$
s>s_{MAX}
$


```

![19 - Funzionamento instabile MAT - ET 2024-07-04 15.57.04.png](/img/user/Excalidraw/19%20-%20Funzionamento%20instabile%20MAT%20-%20ET%202024-07-04%2015.57.04.png)


Il motore si trova nella situazione B: Sta lavorando a una coppia uguale a quella resistente
$$
C_{m} = C_{r}
$$
Si immagini ora che, per qualunque motivo, la coppia resistente aumenti a un qualche valore $C_{r}'$. Questo comporterà una diminuzione della velocità angolare del rotore $\Omega_{rot}$ con conseguente aumento dello [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Scorrimento\|#Scorrimento]]. Pertanto, il motore si troverà a lavorare con una [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Coppia meccanica - MAT\|coppia meccanica]] inferiore, $C_{m}'$, corrispondente alla situazione $B'$.

La nuova coppia motrice risulta ancora inferiore alla coppia resistente: ancora una volta il rotore rallenterà, lo scorrimento aumenterà e la coppia motrice diminuirà. Questo andrà avanti fin quando non si raggiunge la condizione di rotore fermo: $s = 1$.

Chiaramente, dovesse aversi la situazione duale per cui la coppia resistente diminuisce invece di aumentare, la situazione sarà invertita e la coppia motrice aumenterà fino al valore massimo.


```ad-Teo
title: Funzionamento instabile

Si ha **funzionamento instabile** nel tratto della [[#Caratteristica meccanica]] in cui la coppia risulta decrescente al crescere dello [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Scorrimento\|#Scorrimento]], ossia:
$
\frac{\mathrm{d}C}{\mathrm{d}s} < 0 
$

```



#### Funzionamento stabile

```ad-Definizione
title: Funzionamento stabile

Si parla di **funzionamento stabile** del [[19 - Motore Asincrono Trifase - ET|MAT]] quando questo lavora con un valore di [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Scorrimento\|#Scorrimento]] *minore* a quello di massimo della coppia:
$
s<s_{MAX}
$


```

![19 - Funzionamento stabile MAT - ET 2024-07-04 16.14.51.png](/img/user/Excalidraw/19%20-%20Funzionamento%20stabile%20MAT%20-%20ET%202024-07-04%2016.14.51.png)


Il motore si trova nella situazione A: Sta lavorando a una coppia uguale a quella resistente
$$
C_{m} = C_{r}
$$
Si immagini ora che, per qualunque motivo, la coppia resistente aumenti a un qualche valore $C_{r}'$. Questo comporterà una diminuzione della velocità angolare del rotore $\Omega_{rot}$ con conseguente aumento dello [[#Scorrimento]]. Pertanto, il motore si troverà a lavorare con una [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Coppia meccanica - MAT\|coppia meccanica]] superiore, $C_{m}'$, corrispondente alla situazione $A'$.

La nuova coppia motrice riesce a compensare la nuova coppia resistente $C_{r}'$.

Chiaramente, dovesse aversi la situazione duale per cui la coppia resistente diminuisce invece di aumentare, la coppia motrice sarà ancora capace di compensare la coppia resistente, portando a un nuovo punto di lavoro stabile.

```ad-Teo
title: Funzionamento stabile

Si ha **funzionamento stabile** nel tratto della [[#Caratteristica meccanica]] in cui la coppia risulta crescente al crescere dello [[#Scorrimento]], ossia:
$
\frac{\mathrm{d}C}{\mathrm{d}s}>0 
$
Inoltre, la macchina risulta tanto più stabile, quanto più ripido è il tratto di curva, ossia quanto minore risulta $s_{MAX} = \dfrac{R_{r}}{X_{dr}}$
```

## Problemi di avviamento

#### Coppia nominale

```ad-Definizione
title: Coppia nominale ($C_{n}$)

La **coppia nominale** $C_{n}$ corrisponde al valore di coppia a regime della macchina:
$
C_{n} = \frac{P_{n}}{\Omega_{rot}}
$


```

Essa è inferiore alla coppia massima.

Generalmente, la coppia di spunto (o coppia di avviamento) è inferiore alla coppia nominale
$$
C_{avv} \approx 0.2\div0.5\,C_{MAX}
$$
Pertanto, la situazione $C_{avv}<C_{n}$ può comportare dei problemi in fase di avviamento.

### Coppia resistente > Coppia di avviamento

$$
C_{r} < C_{avv}
$$
Se la coppia resistente è maggiore della coppia di spunto (coppia di avviamento), la macchina non parte ($\Omega_{rot} = 0, \quad s = 1$).

Per $s= 1$ corrisponde un valore unico della resistenza equivalente:
$$
R_{e} = R_{r} \frac{1-s}{s} = 0
$$
La macchina si trova quindi in condizioni di *assenza del carico meccanico*: Si tratta di una situazione equivalente al [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/06 - Bipoli e potenza elettrica - ET#Cortocircuito\|cortocircuito]] da cui deriva un ulteriore problema. In condizioni di corto, la corrente del circuito $I_{cc}$ arriva ad assumere valori molto maggiori di $I_{n}$:
$$
I_{cc} \approx 5\div 6 \, I_{n}
$$
e questa condizione può portare al danneggiamento dei componenti del motore


### Coppia resistente < Coppia di avviamento

$$
C_{r} < C_{avv}
$$
Se la coppia resistente è **minore** della coppia di spunto (coppia di avviamento), la macchina si avvia. La fase di avviamento però risulta comunque troppo lunga (in questa fase, come per il caso [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Coppia resistente > Coppia di avviamento\|#Coppia resistente > Coppia di avviamento]], si ha sempre una corrente di Corto circuito), e rischia ancora di danneggiare la macchina.

Per avere avviamento corretto della macchina, non basta che la coppia di spunto sia maggiore di quella resistente, ma serve anche che l'avviamento sia abbastanza rapido.

## Tipi di rotore

### Rotore avvolto

### Rotore a gabbia di scoiattolo

![Schermata 2024-07-08 alle 16.06.37.png](/img/user/Schermata%202024-07-08%20alle%2016.06.37.png)

I rotore a gabbia di scoiattolo è un rotore che, invece di avere avvolgimenti come nel [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Rotore avvolto\|#Rotore avvolto]], presenta barre conduttrici di $\rm Al, Cu$ o bronzo, cortocircuitate alle estremità da 2 anelli robusti, abbattendo così le $R_{r}$ (resistenze rotoriche).

#### Rotore a doppia gabbia di scoiattolo

![Schermata 2024-07-08 alle 16.09.48.png](/img/user/Schermata%202024-07-08%20alle%2016.09.48.png)

Spesso, il [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Rotore a gabbia di scoiattolo\|#Rotore a gabbia di scoiattolo]] è in realtà costituito da due file di barre metalliche.
- Esterna: di sezione $S_{e}$ piccola
- Interna: di sezione $S_{i}$ grande


## Modalità di avviamento

#UNI/ET/Domanda 

- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Avviamento reostatico\|#Avviamento reostatico]]
- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Avviamento nei motori a gabbia\|#Avviamento nei motori a gabbia]]
- [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Avviamento con commutazione\|#Avviamento con commutazione]]

### Avviamento reostatico

Si ricorda che per la coppia meccanica, lo [[Excalidraw/19 - Caratteristica meccanica coppia-scorrimento MAT - ET 2024-07-04 15.23.57#Punto di massimo\|scorrimento di massimo]], e il rispettivo massimo, sono dati da:
$$
s_{MAX} = \frac{R_{r}}{X_{dr}} \qquad C_{MAX} = \frac{3pk}{2\omega } \cdot \frac{1}{{\color{red}X_{dr}}} \cdot V_{1}^{2}
$$

![19 - Caratteristica meccanica - avviamento reostatico  - ET 2024-07-04 16.51.43.png](/img/user/Excalidraw/19%20-%20Caratteristica%20meccanica%20-%20avviamento%20reostatico%20%20-%20ET%202024-07-04%2016.51.43.png)


Poiché la coppia massima non dipende dalla resistenza rotorica, si può pensare di spostare lo scorrimento $s_{MAX}$, aumentandolo, variando $R_{r}$, senza far cambiare il valore massimo della coppia (ovviamente ammesso di mantenere costante la reattanza $X_{dr}$).

In questo modo si passerà dalla curva $R_{1}$ alla curva $R_{2}$. In questa condizione, la coppia di avviamento, $\color{blue} C_{avv}(R_{2})$ risulta maggiore di quella che si otteneva prima. Andando ancora ad aumentare la resistenza al rotore si può fare in modo che la coppia di avviamento approcci sempre di più la $C_{MAX}$.

Questa condizione si ottiene aggiungendo un **banco di reostati (resistori) di avviamento** in modo da far avviare la macchina con la coppia massima disponibile. Gli avvolgimenti rotorici sono collegati all'albero tramite 3 contatti striscianti a forma di anelli. Quest'ultimi sono a loro volta collegati a 3 resistenze variabili a stella; questi risultano quindi in serie con gli avvolgimenti rotorici

![Schermata 2024-07-04 alle 17.24.58.png](/img/user/Schermata%202024-07-04%20alle%2017.24.58.png)

La situazione migliore è quindi quella in cui la $C_{avv} = C_{MAX}$. Essendo $C_{avv}$ la coppia che si ha per $s = 1$, si deve imporre la condizione:
$$
s_{MAX} = 1
$$
ossia:
$$
s_{MAX} = \frac{R_{r}+R_{avv}}{X_{dr}} = 1
$$
Da questa espressione si trova che la massima resistenza del banco reostatico è
$$
R_{avv} = X_{dr}-R_{r}
$$
All'avviamento quindi si collega la resistenza $R_{avv}$ ottenendo 2 vantaggi:
- La macchina parte con coppia massima disponibile
- $I_{avv}<I_{cc}$ - Anche se $R_{e}=0$ (essendo $s=1$), in serie ad $R_{r}$ è comunque presente $R_{avv}$ che limita la corrente circolante negli avvolgimenti rotorici

#### Rimozione del reostato

È chiaro che, una volta avviato il motore, non conviene più farlo lavorare sulla caratteristica di avviamento, in quanto comporterebbe un notevole abbassamento del rendimento.

Bisognerà pertanto diminuire **gradualmente** la $R_{avv}$ fino a rimuoverla del tutto.


È importantissimo far si che la $R_{avv}$ sia rimossa gradualmente e non tutta insieme.

![19 - Caratteristica meccanica di avviamento - MAT - ET 2024-07-04 17.30.34.png](/img/user/Excalidraw/19%20-%20Caratteristica%20meccanica%20di%20avviamento%20-%20MAT%20-%20ET%202024-07-04%2017.30.34.png)


Se la si rimuovesse tutta insieme (come nella figura sopra), il motore si arresterebbe.

Immaginiamo infatti di avere una certa coppia $C_{r}$ come indicata in figura. A regime, sulla curva di avviamento, sarà bilanciata da una coppia uguale alla quale corrisponde il valore di [[#Scorrimento]] $\color{\purple} s_{A}$. Ora rimuoviamo di botto il reostato. All'improvviso, a parità di velocità (e quindi di scorrimento), si avrebbe a disposizione una coppia nettamente inferiore (quella in $A'$). Questo porterebbe ad avere la coppia resistente maggiore della coppia motrice, nel tratto di curva a [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Funzionamento instabile\|#Funzionamento instabile]]. Il motore si arresterebbe.

___

Il reostato dovrà pertanto essere rimosso gradualmente. Dovrò fare in modo che, ogni volta che rimuovo una quota-parte di reostato, la nuova coppia motrice corrispondente al medesimo valore di scorrimento, sia ancora maggiore alla coppia resistente. 

![Schermata 2024-07-04 alle 17.41.08.png](/img/user/Schermata%202024-07-04%20alle%2017.41.08.png)


### Avviamento nei motori a gabbia

L'[[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Avviamento reostatico\|#Avviamento reostatico]] è utilizzabile soltanto nelle macchine a rotore avvolto, in cui gli avvolgimenti rotorici sono avvolti sui pacchi di lamierini rotorici utilizzando le cave, le quali però indeboliscono la struttura. 

Spesso si usa un rotore detto [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Rotore a gabbia di scoiattolo\|#Rotore a gabbia di scoiattolo]]. 
Poiché però gli anelli di cc sono solidali al rotore, è precluso l'utilizzo del reostato di avviamento.

Il problema maggiore nei motori a g.d.s. è che, per via della bassa resistenza, le correnti di spunto sono molto elevate ($I_{cc}$).

![Schermata 2024-07-04 alle 17.51.46.png](/img/user/Schermata%202024-07-04%20alle%2017.51.46.png)

Si raffigura il circuito monofase equivalente del rotore a gabbia di scoiattolo:

![19 - CEM Rotore a gabbia di scoiattolo - ET 2024-07-04 18.00.40.png](/img/user/Excalidraw/19%20-%20CEM%20Rotore%20a%20gabbia%20di%20scoiattolo%20-%20ET%202024-07-04%2018.00.40.png)


dove:
- $\dot{Z}_{L} = R_{L}+jX_{L}:$ Impedenza di linea
- $\dot{Z}_{M}:$ Impedenza di ingresso del motore, dipendente dallo scorrimento (ossia da $\Omega_{rot}$)
- $\overline{V}:$ Tensione di alimentazione degli avvolgimenti statorici del [[19 - Motore Asincrono Trifase - ET|MAT]]

Si può calcolare la caduta percentuale di tensione:
$$
\Delta V_{\%} = \frac{R_{L}P+X_{L}Q}{V^{2}} \cdot 100
$$

Il motore è generalmente alimentato a $V = 220\,\rm V$. La caduta di tensione però deve rimanere contenuta in modo da limitare le correnti di avviamento. Se ciò non avviene, si finisce solo per aumentare la caduta percentuale, facendo diminuire la tensione di alimentazione con il risultato di avere correnti di avviamento elevate e una macchina che non parte.

Per ovviare a ciò si sfrutta l'[[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Avviamento con commutazione stella-triangolo\|#Avviamento con commutazione stella-triangolo]]

#### Avviamento con commutazione stella-triangolo

Questo tipo di avviamento, nei motori a gabbia di scoiattolo, sfrutta il fatto che, a parità di tensioni, le correnti di carico nella [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a stella\|configurazione a stella]] risultano essere 1/3 di quelle nella [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/08 - Reti in regime stazionario - ET#Configurazione a triangolo\|configurazione a triangolo]].

Anche se la tensione di alimentazione del motore è $\overline{V}$, la tensione sulle fasi statoriche risulterà la tensione stellata
$$
\overline{E} = \frac{\overline{V}}{\sqrt{3}}
$$
La corrente sul carico (corrispondente nel collegamento a stella alla [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/15 - Reti trifasi - ET#Correnti di linea\|corrente di linea]]) sarà:
$$
\overline{I}_{\star} = \frac{\overline{E}}{\dot{Z}} = \frac{\overline{V}}{\sqrt{3}\dot{Z}} 
$$
La coppia di spunto anche risulterà ridotta. Essendo essa proporzionale al quadrato della tensione:
$$
C_{\triangle} = 3 C_{\star}
$$
#### Avviamento nei motori a doppia gabbia di scoiattolo

Nel [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Rotore a doppia gabbia di scoiattolo\|#Rotore a doppia gabbia di scoiattolo]] si è detto che le sezioni delle gabbie sono così relazionate:
$$
S_{e}<S_{i}
$$
Si possono calcolare le impedenze delle due gabbie:
$$
\begin{align}
\dot Z_{i} &= R_{i} + jsX_{di} \\
\dot Z_{e} &= R_{e} + jsX_{de}
\end{align}
$$
È chiaro che la corrente totale che scorre nelle gabbie è la somma delle correnti delle singole gabbie:
$$
\overline{I}_{r} = \overline{I}_{i} + \overline{I}_{e}
$$
E lo stesso posso dire per le coppie:
$$
C_{m} = C_{mi} + C_{me}
$$


**AVVIAMENTO** - $s=1$

![Schermata 2024-07-08 alle 16.29.16.png](/img/user/Schermata%202024-07-08%20alle%2016.29.16.png)

In fase di avviamento, le impedenze diventano:
$$
\begin{align}
\dot Z_{i} &= R_{i} + jX_{di} \\
\dot Z_{e} &= R_{e} + jX_{de}
\end{align}
$$
La resistenza rotorica, rispetto alla reattanza induttiva è trascurabile.
Essendo, per via delle dimensioni
$$
X_{di} \gg X_{de} 
$$
sarà anche vero, in termini di impedenze:
$$
\dot Z_{i} \gg \dot Z_{e}
$$
Pertanto, la corrente di rotore, risulterà, in fase di avviamento, pari a quella della gabbia esterna
$$
\overline{I}{r} \simeq \overline{I}_{e}
$$

**VICINO AL SINCRONISMO** - $s\ll1$

![Schermata 2024-07-08 alle 16.29.47.png](/img/user/Schermata%202024-07-08%20alle%2016.29.47.png)

Una volta avviata, per velocità vicine al sincronismo, essendo lo [[#Scorrimento]] molto minore di 1, l'impedenza risulterà simile alla resistenza:
$$
\begin{align}
\dot Z_{i} &= R_{i} + jsX_{di} \simeq  R_{i}\\
\dot Z_{e} &= R_{e} + jsX_{de} \simeq  R_{e}
\end{align}
$$
Essendo 
$$
R_{i}\ll R_{e} \quad\Longrightarrow\quad Z_{i}\ll Z_{e}
$$
Pertanto, la corrente rotorica sarà pari a quella della gabbia interna
$$
\overline{I}_{r} \simeq \overline{I}_{i}
$$



In condizioni di funzionamento intermedie la corrente si ripartirà tra le due gabbie e si avrà [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Caratteristica coppia scorrimento\|#Caratteristica coppia scorrimento]] intermedia tra le situazioni di $s =1$ e $s=0$.

![Schermata 2024-07-08 alle 16.30.00.png](/img/user/Schermata%202024-07-08%20alle%2016.30.00.png)





