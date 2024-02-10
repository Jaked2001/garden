---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/veicoli-e-impianti-di-trasporto/lezioni/10-motori-ed-equipaggiamenti-per-la-trazione-elettrica-vit/"}
---

# [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT\|10 - Motori ed equipaggiamenti per la trazione elettrica - VIT]]

Nel caso di trazione elettrica, la corrente è captata dalla linea aerea di alimentazione e raggiunge i motori attraverso opportuni equipaggiamenti di trazione.
Il circuito di trazione si chiude attraverso le rotaie che consentono il ritorno di corrente alla sottostazione che alimenta la linea.

## Elettrificazione delle ferrovie

L'alimentazione elettrica da rete fissa non è unificata in ambito europeo. Ogni rete ferroviaria ha storicamente operato scelte diverse.

Il **motore a collettore** nonostante il costo, la delicatezza e l'elevata manutenzione, è stato a lungo la scelta ottimale. 

In paesi come Italia, Belgio, Spagna e Polonia fu adottata la tensione nominale di $3000\, \rm V$ in CC.
Altri paesi, come la Francia, limitarono per prudenza la tensione a $1500 \, \rm V$.

L'avvento dell'[[Alta Velocità\|Alta Velocità]] (AV), con potenze unitarie di oltre $12 \, \rm MW$ ha reso necessario l'utilizzo di reti ad alta tensione.
Si è adottato quindi un sistema a AC monofase a $25 \, \rm V$ a $50 \, \rm Hz$.

## Motore in Corrente Continua

Il motore a corrente continua (CC) si basa sulle forze che nascono in un conduttore percorso da corrente immerso in un campo magnetico.

Infatti, preso un conduttore rettilineo di lunghezza $l$, disposto *normalmente* alle linee di campo magnetico $B$, uniforme e costante, e percorso da una corrente $I$, è sollecitato da una forza che tende a spostarlo normalmente al campo e alla corrente secondo la legge
$$
\vec{F} = l \cdot \vec{I} \times \vec{B}
$$
Il motore in CC è costituito da
- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Rotore\|#Rotore]] o **INDOTTO**: Un corpo cilindrico solidale a un albero, libero di ruotare
- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Statore\|#Statore]]: Una parte fissa

![Schermata 2024-02-06 alle 18.29.23.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2018.29.23.png)

Le spire del [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Rotore\|#Rotore]] sono quindi percorse da una corrente $I$ e immerse in un campo magnetico di intensità $B$.
Ogni spira è pertanto soggetta a una forza di intensità $F = lIB$ tangenziale rispetto a ogni conduttore. Questa forza genera un momento che ha per braccio il raggio del rotore. Essendo nel ramo opposto della spira la corrente con verso opposto, la forza andrà nel verso opposto anch'essa ma avrà la stessa intensità. Ogni spira genera quindi una coppia che determina la rotazione dell'indotto.

Poiché nella rotazione i conduttori del [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Rotore\|#Rotore]] tagliano il campo magnetico, per via della variazione di flusso viene a generarsi una Forza Contro-elettro motrice (una differenza di potenziale) che dipende dal **numero di giri al minuto** ($n$) e dal **flusso del campo** ($\phi$)
$$
E = kn\phi
$$
dove $k$ è una costante che dipende dal **numero di conduttori indotti**, dal **numero  di poli** e dal **tipo di avvolgimento**.

Questa $E$ avrà sicuramente verso opposto alla corrente che scorre nelle spire e sarà determinata come
$$
\vec{E} = \vec{V} \times \vec{B} \cdot l
$$
Secondo la [[Legge di Ohm\|Legge di Ohm]] si avrà quindi che
$$
U = E + R_{c} \cdot I
$$
dove
- $U=$ Tensione di alimentazione
- $E=$ Forza contro-elettro motrice
- $R_{c} =$ Resistenze del circuito
Se si moltiplicano entrambi i membri per la corrente $I$ si ottiene la potenza del motore:
$$
UI = EI + R_{c}I^{2}
$$
che riscrivo come
$$
EI = UI - R_{c}I^{2}
$$
dove:
- $EI = P_{M}$ - Potenza assorbita trasformata in potenza meccanica del motore
- $R_{c}I^{2}$ - Potenza dissipata per [[effetto Joule\|effetto Joule]]
- $UI$ - Potenza fornita al motore

In definitiva quindi

```ad-Teo
In un motore elettrico a corrente continua la potenza meccanica del motore è data da
$$
P_{M} = UI - R_{c}I^{2}
$$
```

Ricordando poi che la tensione $E$ può essere scritta in funzione del flusso come $E = kn\phi$, la potenza meccanica diventa
$$
P_{M} = EI = kn\phi \cdot I
$$
Ora, essendo $\Omega$ la velocità angolare del [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Rotore\|#Rotore]] e $C$ la coppia ad esso trasmessa, si ha che
$$
P_{M} = C \cdot\Omega
$$
La velocità angolare $\Omega$ è data da
$$
\Omega = \frac{2\pi n}{60}
$$
essendo $n$ in $\rm rpm$, ottengo così la velocità angolare in $\rm \frac{rad}{s}$.

A questo punto posso scrivere la coppia del motore elettrico in corrente continua come
$$
C = k \frac{60}{2\pi}\phi\cdot I = kc \cdot \phi \cdot I
$$
essendo $c = \frac{60}{2\pi}$.

![10. Motori ed equipaggiamenti per la trazione elettrica - VIT 2024-02-07 11.48.43.excalidraw.png](/img/user/Excalidraw/10.%20Motori%20ed%20equipaggiamenti%20per%20la%20trazione%20elettrica%20-%20VIT%202024-02-07%2011.48.43.excalidraw.png)


Si può quindi graficare la [[Università/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/03. Sostentazione e locomozione#Caratteristica meccanica di trazione\|caratteristica meccanica]] del motore elettrico in CC essendo
$$
\begin{cases}
C = k c \phi I \\
n = \dfrac{U-R_{c}I}{k \phi}
\end{cases}
$$
Se aumenta la corrente $I$, aumenta la coppia $I$ e diminuisce il numero di giri $n$.

```ad-note
title: Osservazione
L'andamento della caratteristica meccanica del motore in CC si avvicina molto a quello di un'iperbole. Nel caso di iperbole avremmo proprio potenza costante, e quindi caratteristica ideale.

Questa in realtà è più decrescente di quella ideale: a parità di numero di giri $n$, la coppia è minore di quella corrispondente all'iperbole.

```

Si noti che l'andamento della curva deve essere limitato sia superiormente che inferiormente:
- La coppia deve essere compatibile a rispettare i limiti di aderenza
- Il numero di giri non può superare la resistenza dei componenti meccanici del motore
- È necessario un meccanismo di **regolazione**: spostare la caratteristica nel piano $C,n$ in relazione alle varie condizioni di moto.


❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ Problema di avviamento e reostato
❗❗❗❗❗❗❗❗❗❗❗❗❗


### Rotore

Il **rotore**, o indotto, è costituito da **lamierini di ferro** e da **conduttori di rame** all'interno dei quali circola la corrente.
I conduttori sono a forma di spira le cui estremità terminano sull'albero.

L'insieme di tutti i contatti elettrici di tutte le spire del rotore prende il nome di **collettore**.

Il contatto elettrico tra l'albero (estremità delle spire) e la sorgente di alimentazione fissa, essendo il primo in movimento rispetto a quest'ultime, è assicurato mediante **SPAZZOLE** striscianti sul collettore.

Questo è uno dei punti deboli del motore CC in quanto le spazzole e il collettore sono soggetti a usura meccanica.


### Statore

Lo statore è costituito da un cilindro di ferro al cui interno ruota il [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Rotore\|#Rotore]].

La funzione dello statore è di creare il campo magnetico in cui è immerso il rotore. All'interno dello statore si trova pertanto una serie di spire collegate alla sorgente di corrente elettrica.

I circuiti delle spire dello statore e del rotore possono essere lo stesso circuito e quindi collegati in serie oppure in parallelo. A seconda del tipo di collegamento, cambia la [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Caratteristica meccanica\|#Caratteristica meccanica]] del motore.


## Motore Asincrono in corrente Alternata Trifase


<iframe width="560" height="315" src="https://www.youtube.com/embed/7O_dxw1RXxg?si=a5iFr6C0SbpUsD41" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

https://youtu.be/7O_dxw1RXxg?si=X-v7FChN0vhAdfu8

Si tratta di un tipo diverso di motore dal [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Motore in Corrente Continua\|#Motore in Corrente Continua]]. Uno dei vantaggi principali è quello di non avere contatti elettrici fisici tra elementi fissi e in movimento (non ha spazzole) e questo garantisce una maggiore durabilità.

Si tratta di un motore **asincrono** alimentato in **corrente alternata trifase**.

I sistemi di alimentazione elettrica nelle reti ferroviarie oggi sono però in CC o in AC monofase. Occorre pertanto installare, a bordo, una macchina elettrica, statica o dinamica, che trasformi la corrente continua in alternata trifase.

Questa operazione è eseguita da un dispositivo chiamato [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Inverter\|#Inverter]]. Quest'ultimo interrompe periodicamente la corrente continua in ingresso regolando la durata delle fasi di interruzione e di quelle di conduzione in modo che la corrente risultante sia alternata.

![Pasted image 20240207120922.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Pasted%20image%2020240207120922.png)

Il motore è detto **asincrono** in quanto la velocità angolare del rotore è inferiore alla velocità di rotazione del campo magnetico generato dallo statore.

In genere lo statore presenta un numero pari di avvolgimenti. Per un motore trifase ci saranno quindi almeno 6 avvolgimenti in tutto. In questo caso, le coppie polari sono sfasate a 120° fisicamente ed elettricamente.

Negli avvolgimenti dello statore si verifica il passaggio di correnti (alternate) le quali inducono un campo magnetico complessivo che ruota nello spazio.

Questo campo magnetico induce nel rotore una f.e.m. e quindi il passaggio di correnti elettriche che, a loro volta, inducono anche nel rotore un campo magnetico rotante.

Nel rotore è presente un certo numero di fasi chiuse in corto circuito --> **rotore a gabbia di scoiattolo**.

La rotazione del campo magnetico di **statore** avviene a una velocità fissa $n$ legata alla frequenza di alimentazione $f$. Questa velocità è detta **velocità di sincronismo**.

Il rotore ruota a velocità $n_{1}$. Quindi, il campo magnetico di rotore ruota, rispetto a quello di statore, a una velocità relativa $n-n_{1}$. In questa condizione, i campi di rotore e di statore, ruotano in maniera **sincrona**. Questa è una condizione limite in cui non vi sono forze elettromotrici e dunque la coppia motrice è nulla.

In realtà, la velocità di rotazione del rotore $n_{1}$ è sempre leggermente **minore** di quella di sincronismo --> **Scorrimento** (s) che consente la produzione di coppia.

![Pasted image 20240207141456.png|650](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Pasted%20image%2020240207141456.png)

La caratteristica meccanica del motore asincrono trifase, dipende da
- **Tensione** di alimentazione
- **Frequenza** di alimentazione
- **Numero di coppie polari** che creano il campo magnetico
Fissati questi parametri, si può tracciare la caratteristica meccanica di questo motore in funzione della velocità di rotazione (grafico sopra).

```ad-note
title: Osservazione
Rispetto al [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Motore in Corrente Continua\|#Motore in Corrente Continua]] questo presenta due vantaggi sostanziali:
- La coppia ha valore finito a velocità nulla --> non sono necessarie particolari regolazioni in avviamento
- La velocità ha valore finito a coppia nulla --> è impossibile che la velocità possa andare oltre il limite di resistenza del motore (fuori giri)

```

Si noti però che, a parte questi elementi, questa caratteristica meccanica non è adatta alla trazione. Infatti, non consente un adattamento della velocità a condizioni diverse di marcia (praticamente è a **velocità costante**) a meno di non intervenire sui parametri dell'alimentazione (frequenza e tensione).

Per questo, il motore asincrono viene regolato in 2 fasi:
- **Forza costante**: con un [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Inverter\|#Inverter]] si fa variare la frequenza e la tensione per avere una coppia costante
- **Tensione costante**: con un [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Inverter\|#Inverter]] si fa variare la frequenza e quindi la coppia

![Pasted image 20240207142159.png|650](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Pasted%20image%2020240207142159.png)

## Motore Sincrono in Corrente Alternata Trifase


## Disposizione dei motori in un carrello

![Schermata 2024-02-07 alle 14.26.59.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/allegati/Schermata%202024-02-07%20alle%2014.26.59.png)

![Schermata 2024-02-07 alle 14.27.09.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/allegati/Schermata%202024-02-07%20alle%2014.27.09.png)

## Azionamenti per la trazione elettrica

```ad-Definizione
title: Azionamenti

Si definisce **azionamento** l'insieme costituito dai motori elettrixi di trazione edalle relative **apparecchiature di controllo e regolazione**. 

```

Gli azionamenti hanno la funzione principale di esercire il mezzo di trazione nelle varie condizione di moto  approssimando il più possibile la caratteristica ideale a potenza costante.

### Azionamenti in Corrente Continua

Inizialmente i [[#Motore in Corrente Continua]] erano eccitati in serie (stessa corrente su rotore e statore).
La regolazione in questi motori avveniva storicamente modificando sia il circuito interno della macchina elettrica sia il circuito in cui essa era inserita.

Si parla pertanto di [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Regolazione circuitale o a contattori\|#Regolazione circuitale o a contattori]]. Tale tipo di regolazione da luogo a **caratteristiche discrete**.

#### Regolazione circuitale o a contattori

Questa regolazione si basa su **pacchi di resistenze** che vengono gradualmente escluse con l'aumento della velocità al fine di controllare la corrente e quindi la **coppia** (**regolazione reostatica**).
Altrimenti, nel caso di più motori a bordo, usando diverse combinazioni si possono variare, a parità di corrente, la tensione e la velocità (**regolazione in serie/parallelo**).

![Schermata 2024-02-07 alle 14.47.58.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/allegati/Schermata%202024-02-07%20alle%2014.47.58.png)

#### Chopper

La disponibilità di tiristori al silicio ha consentito la realizzazione di **convertitori elettronici (statici)** in grado di **regolare** il valore della tensione in un circuito di potenza in CC.

Nacque così un convertitore elettronico di alta potenza chiamato **chopper** o **frazionatore**.

Questo è capace di regolare la velocità in modo continuo, eliminando gli strappi che si verificano nella [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Regolazione circuitale o a contattori\|#Regolazione circuitale o a contattori]].

Inoltre, questo tipo di azionamento migliora il rendimento energetico, non essendoci energia dissipata in resistenze.



Vantaggi del chopper
- Regolazione **continua**
- Risparmio di **ingombro**, **peso** e **usura**
- I motori possono essere configurati nella combinazione corrispondente alla massima tensione sostenibile


##### Principio di funzionamento del chopper

Si hanno a disposizione:
- Una **sorgente di tensione continua** $V_{1}$
- Un **interruttore** $K$
- Un **carico** $C$

SI può immaginare di aprire e chiudere l'interruttore $K$ con una opportuna **temporizzazione** variando la tensione tra $V_{1}$ e $0$.

Si ottiene una forma di onda fatta da una successione di **impulsi rettangolari** - come se l'interruttore avesse tagliato a fette (chop) la tensione di alimentazione.

Si distingueranno quindi:
- $T_{ON} -$ **Intervallo di conduzione**
- $T_{OFF} -$ **Intervallo di interdizione** o di **blocco**

L'intervallo $T_{ON} + T_{OFF}$ è detto **periodo**.

Il chopper, a seconda che la tensione in uscita sia superiore o inferiore a quella in ingresso può essere **elevatore** o **abbassatore**.

### Azionamenti in corrente alternata

Il [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Motore Asincrono in corrente Alternata Trifase\|#Motore Asincrono in corrente Alternata Trifase]] presenta alcune problematiche
- Caratteristica meccanica stabile solo in un campo ristretto
- Valore della coppia di avviamento molto minore della coppia max
- Coppia che varia col quadrato della tensione --> soggetta alle frequenti variazioni di tensione della linea di contatto

La regolazione di questo motore si effettua mediante un dispositivo chiamato [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Inverter\|#Inverter]]

#### Inverter












