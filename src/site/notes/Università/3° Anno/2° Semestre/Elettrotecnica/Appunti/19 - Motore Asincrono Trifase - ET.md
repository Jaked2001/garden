---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/19-motore-asincrono-trifase-et/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|19 - Motore Asincrono Trifase - ET]]

Nella figura sottostante è mostrato lo schema di una **macchina asincrona trifase**

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

Quando nelle spire passa corrente, si genera un [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/18 - Campo magnetico rotante\|campo magnetico rotante]].

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
Pertanto, la pulsazione delle grandezze rotoriche, data un'unica coppia polare è pari alla velcoità angolare del campo inducente (statorico)
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

In [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Condizione di sincronismo\|#Condizione di sincronismo]]
$
\Omega_{rot} = \omega_{s} \qquad\Longrightarrow\qquad s = 0
$

```

### Fase di avviamento

Vedendo gli avvolgimenti come degli induttori, si può rappresentare il circuito equivalente come segue:

![19 - Motore Asincrono Trifase - ET 2024-07-03 18.59.43.png](/img/user/Excalidraw/19%20-%20Motore%20Asincrono%20Trifase%20-%20ET%202024-07-03%2018.59.43.png)


A [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Funzionamento a rotore bloccato\|rotore bloccato]] si ha semplicemente trasferimento di potenza elettrica per accoppiamento elettromagnetico e la macchina si comporta come un [[Trasformatore\|Trasformatore]] con il secondario in corto circuito. --> Abbiamo un **trasformatore trifase**

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

A rotore bloccato, la pulsazione delle grandezze indotte rotoriche è proprio $\omega$. Allora, proprio come nel trasformatore, è rispettata l'ipotesi di isofrequenzialità.

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
$$
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
Questa resistenza è funzione dello [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Scorrimento\|#Scorrimento]]. È quindi una resistenza variabile e definisce il **carico meccanico** del motore.

![19 - Circuito equivalente monofase a rotore libero con resistenza equivalente - ET 2024-07-04 11.55.19.png](/img/user/Excalidraw/19%20-%20Circuito%20equivalente%20monofase%20a%20rotore%20libero%20con%20resistenza%20equivalente%20-%20ET%202024-07-04%2011.55.19.png)


E quindi, riscrivendo la [[Legge di Kirchhoff delle Tensioni (LKT)\|LKT]] tenendo conto della resistenza equivalente:
$$
\overline{E}_{20} = \left( R_{r} + X_{dr} \right) \overline{I}_{2} + R_{e}\overline{I}_{2}
$$
La corrente $\overline{I}_{2}$ resta invariata.

Il circuito equivalente monofase, rappresentando le grandezze in funzione dello scorrimento, diventa:

![19 - Circuito equivalente monofase a rotore libero in funzione di scorrimento - ET 2024-07-04 12.01.12.png](/img/user/Excalidraw/19%20-%20Circuito%20equivalente%20monofase%20a%20rotore%20libero%20in%20funzione%20di%20scorrimento%20-%20ET%202024-07-04%2012.01.12.png)


In questo modo possiamo rappresentare le varie grandezze. In particolare, la resistenza equivalente, assumerà valori diversi nella [[#Condizione di sincronismo]] e nella [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Circuito equivalente monofase a rotore bloccato\|condizione di rotore bloccato]]:
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
Nel [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]] il rendimento si aggira intorno al:
- $\eta \sim 60\%:$ per piccoli motori
- $\eta \sim 97\%:$ per grandi motori











</div></div>



___


**Potenza reattiva**:

![19 - Potenza reattiva MAT - ET 2024-07-04 12.26.36.png](/img/user/Excalidraw/19%20-%20Potenza%20reattiva%20MAT%20-%20ET%202024-07-04%2012.26.36.png)



<div class="transclusion internal-embed is-loaded"><div class="markdown-embed">



## Flussi di potenza reattiva nel MAT

In termini di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Potenza reattiva\|potenza reattiva]] si ha che al sistema è fornita una potenza in ingresso $Q_{in}$.

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

Sia il [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Circuito equivalente monofase a rotore libero\|#Circuito equivalente monofase a rotore libero]] quello riportato in figura:

![19 - Circuito equivalente monofase a rotore libero con resistenza equivalente - ET 2024-07-04 11.55.19.png](/img/user/Excalidraw/19%20-%20Circuito%20equivalente%20monofase%20a%20rotore%20libero%20con%20resistenza%20equivalente%20-%20ET%202024-07-04%2011.55.19.png)

Abbiamo detto essere
$$
R_{e} = R_{r} \frac{1-s}{s}
$$
Pertanto, la potenza meccanica del [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET\|MAT]] in presenza di 3 coppie polari, è data da:
$$
P_{m} = 3R_{e}I_{2}^{2}
$$
dalla quale si ricava la [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Potenza meccanica - MAT\|#Potenza meccanica - MAT]]

L'[[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Impedenza\|impedenza]] totale del circuito di rotore è:
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

La **coppia meccanica** del [[19 - Motore Asincrono Trifase - ET|MAT]] è
$
C_{m} = \frac{P_{m}}{\Omega_{rot}}
$
dove:
- $\Omega_{rot}:$ Velocità angolare del rotore (nel riferimento statorico)
- $P_{m}:$ [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/19 - Motore Asincrono Trifase - ET#Potenza meccanica - MAT\|#Potenza meccanica - MAT]]

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
\frac{3p}{\omega} \frac{R_{r}}{\dfrac{R_{r}^{2}}{s} + sX_{dr}^{2}} \cdot E^{2}_{20}
$$
Si osservi che la coppia meccanica scala con il quadrato della tensione al secondario a vuoto.


### Potenza meccanica - MAT

Abbiamo detto essere
$$
R_{e} = R_{r} \frac{1-s}{s}
$$

```ad-Definizione
title: Potenza meccanica ($P_{m}$)

La **potenza meccanica** consegnata alla resistenza equivalente del rotore del [[19 - Motore Asincrono Trifase - ET|MAT]] in presenza di 3 coppie polari, è data da:
$
P_{m} = 3R_{e}I_{2}^{2}
$


```
