---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/veicoli-e-impianti-di-trasporto/lezioni/04-dinamica-dei-veicoli-vit/"}
---



# [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/04 - Dinamica dei veicoli - VIT\|04 - Dinamica dei veicoli - VIT]]

## Marcia in curva

Quando un treno percorre una curva, si genera una forza, detta **forza centrifuga** esprimibile come:
$$
F_{c} = m a_{c} = m\frac{v^{2}}{R}
$$
dove
- $v =$ Velocità del veicolo
- $R=$ Raggio della curva
- $a_{c}=$ Accelerazione centripeta

La forza centrifuga ha le seguenti caratteristiche:
- Agisce sulla rotaia esterna
- È diretta verso l'esterno della curva
- Tende a ribaltare il veicolo verso l'esterno
- Riduce il comfort dei passeggeri

## Stabilità a sbandamento e ribaltamento


### Stabilità allo sbandamento - senza sovralzo

![Schermata 2024-02-06 alle 16.01.34.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2016.01.34.png)

Dato un veicolo che percorre una curva di raggio $R$ a velocità $V$, su di questo agiscono le seguenti forze:
- $P = mg$ - Forza peso
- $F_{c} = \frac{P}{g} \frac{v^{2}}{R}$ - Forza centrifuga
- $R_{1}, R_{2}$ - Reazioni verticali
- $T_{1}, T_{2}$ - Reazioni trasversali

Affinché il veicolo percorra la curva a velocità costante, si possono scrivere le seguenti equazioni di equilibrio delle forze e dei momenti:
$$
\begin{cases}
X: \qquad R_{1} + R_{2} - mg = 0 \\
Y: \qquad T_{1} + T_{2} - F_{c} = 0 \\
M_{O}: \quad F_{c}h + R_{1}s - mg \frac{s}{2} = 0
\end{cases}
$$
che diventa, esplicitando la forza centrifuga
$$
\begin{cases}
X: \qquad R_{1} + R_{2} - mg = 0 \\
Y: \qquad T_{1} + T_{2} - m \frac{v^{2}}{R} = 0 \\
M_{O}: \quad F_{c}h + R_{1}s - mg \frac{s}{2} = 0
\end{cases}
$$
Ricordando inoltre le condizioni di [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/01 - Introduzione - VIT#Aderenza\|aderenza]], ipotizzando il coefficiente di aderenza uguale per tutte le ruote:
$$
T_{1} \le \varphi R_{1} \qquad T_{2} \le \varphi R_{2}
$$
L'equazione di equilibrio orizzontale può essere riscritta
$$
T_{1} + T_{2} = m \frac{v^{2}}{R} \le \varphi(R_{1}+R_{2})
$$
Da cui si ottiene il **limite** imposto alla velocità dallo **sbandamento**:

```ad-Teo
title: Limite allo sbandamento - senza sovralzo

$$
\frac{v^{2}}{R} \le \varphi g
$$

```

dove si è usata l'equazione all'equilibrio verticale.
Si possono inoltre ricavare le reazioni alle due ruote:
$$
\begin{cases}
R_{1} = P \left( \dfrac{1}{2} - \dfrac{v^{2}h}{Rsg} \right) \\
R_{2} = P \left( \dfrac{1}{2} + \dfrac{v^{2}h}{Rsg} \right)
\end{cases}
$$
da cui si evince che il carico aumenta all'esterno e diminuisce all'interno. Occorre quindi imporre un ulteriore limite, al fine di evitare il [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/04 - Dinamica dei veicoli - VIT#Stabilità al ribaltamento - senza sovralzo\|ribaltamento]]

### Stabilità al ribaltamento - senza sovralzo

![Schermata 2024-02-06 alle 16.01.34.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2016.01.34.png)

Poiché il vincolo di appoggio della ruota sulla via non è bidirezionale (reagisce solo a compressione) occorre imporre che la reazione vincolare non cambi segno rispetto a quello ipotizzato e cioè che sia non negativa:
$$
R_{1} \ge 0
$$
Ricordando il valore della reazione interna:
$$
R_{1} = P \left( \dfrac{1}{2} - \dfrac{v^{2}h}{Rsg} \right)
$$
vogliamo quindi
$$
\frac{1}{2} \ge \dfrac{v^{2}h}{Rsg}
$$
Questo impone la condizione
$$
\frac{v^{2}}{R} \le \frac{sg}{2h}
$$
Si osservi che $\dfrac{s}{2h}$ può essere riscritto come la tangente dell'angolo $\alpha$:

```ad-Teo
title: Limite al ribaltamento - senza sovralzo

$$
\frac{v^{2}}{R} \le g\tan\alpha 
$$

```

### Stabilità allo sbandamento con sovralzo

![Schermata 2024-02-06 alle 16.13.36.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2016.13.36.png)

```ad-Teo
title: Limite allo sbandamento - con sovralzo

$$
\frac{v^{2}}{R} \le g\varphi \frac{1+ \tan\left( \frac{\gamma}{\varphi} \right)}{1- \varphi\tan\left( \gamma \right)}
$$

```


### Stabilità al ribaltamento - con sovralzo


![Schermata 2024-02-06 alle 16.13.36.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2016.13.36.png)

```ad-Teo
title: Limite allo sbandamento - con sovralzo

$$
\frac{v^{2}}{R} \le g \tan(\alpha+\gamma)
$$

```

## Sovralzo

```ad-Definizione
title: Sovralzo

Il **sovralzo** è una sopraelevazione della rotaia esterna rispetto a quella interna. In curva si realizza elevando la quota della rotaia esterna in modo che la forza peso possa compensare la forza centrifuga.

```

Il sovralzo ha delle limitazioni dovute a:
- differenze di velocità tra i treni che percorrono la linea
- Il fatto che un veicolo deve potersi fermare in curva senza ribaltarsi

In Italia, il valore massimo del sovralzo è di $160 \, \rm mm$.

Il sovralzo in realtà ha una duplice funzione. Oltre ad aumentare la velocità massima in curva, assicura un miglior comfort dei passeggeri. Vengono infatti limitate:
- La componente dell'accelerazione centrifuga parallela al piano del ferro (**accelerazione non compensata**) $a_{nc}$
- La componente dell'accelerazione centrifuga parallela al pavimento del veicolo (**accelerazione laterale del passeggero**) $a_{lp}$
Se si suppone che il pavimento del treno si mantenga parallelo al piano del ferro, si può dire che
$$
a_{nc} = a_{lp}
$$
Sotto questa ipotesi, i viaggiatori sono sottoposti a una forza laterale $F_{lp}$ pari alla forza non compensata $F_{nc}$.
$$
F_{lp} = F_{nc} = F'_{c} - P' = m \frac{v^{2}}{R} \cos{\alpha} - mg \sin{\alpha}
$$
Dove si sono considerate solo le componenti orizzontali di ciascuna forza, essendo $\alpha$ l'inclinazione del piano di binario. Considerando $\cos \alpha \approx 1$ si ha che
$$
a_{lp} = a_{nc} = \frac{v^{2}}{R} - g \sin\alpha = \frac{v^{2}}{R} - g \frac{h}{s}
$$
Fissato il valore massimo di accelerazione non compensata che può subire un passeggero, e fissato il sovralzo massimo sulla base dei limiti descritti prima, si può trovare la velocità massima in funzione del raggio della curva:
$$
v = \sqrt{a_{nc} + g \frac{h}{s}} \cdot \sqrt{R}
$$
Sulla base di queste considerazioni, in funzione dell'accelerazione max che il treno può subire, si definisce il [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/04 - Dinamica dei veicoli - VIT#Rango\|#Rango]] del treno.

### Rango

![Schermata 2024-02-06 alle 16.44.42.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2016.44.42.png)

### Treni ad assetto variabile

Alcuni treni possono modificare il proprio assetto in curva per diminuire l'accelerazione trasmessa ai passeggeri rispetto a quella non compensata dal treno.s
I treni ad assetto variabile permettono infatti l'inclinazione di un ulteriore angolo $\beta$ verso l'interno della curva del pavimento. 

![Schermata 2024-02-06 alle 16.47.59.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2016.47.59.png)


## Stabilità allo svio

In ferrovia, più che alla [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/04 - Dinamica dei veicoli - VIT#Stabilità a sbandamento e ribaltamento\|stabilità allo sbandamento]] si è interessati alla stabilità allo svio.
Nella [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/03 - Architettura dei veicoli ferroviari - VIT#Ruota Ferroviaria\|ruota ferroviaria]] infatti il bordino rappresenta un fine corsa nello spostamento laterale della [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/03 - Architettura dei veicoli ferroviari - VIT#Sala montata\|sala montata]].

![Schermata 2024-02-06 alle 16.53.13.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2016.53.13.png)

Si guardi al punto di contatto bordino-rotaia
La ruota trasmette alla rotaia due forze:
- $Q=$ Peso gravante sulla ruota
- $Y =$ Forza orizzontale dovuta alla forza centrifuga
La somma vettoriale di $Q$ e $Y$ fornisce la forza $F$ trasmessa dalla ruota alla rotaia.

Nel punto di applicazione, la forza $F$ può essere scomposta in due componenti, una tangenziale ($T$) e una normale ($N$) alla superficie di contatto:
$$
\begin{align}
T = Y \cos{\beta} - Q\sin\beta \\
N = Y \sin\beta+ Q \cos\beta
\end{align}
$$
essendo $\beta$ l'inclinazione della superficie di contatto rispetto all'orizzontale.

Una prima forma della **condizione di stabilità allo svio** prevede che la componente tangenziale **non** sia superiore alla forza di attrito che può nascere al contatto:
$$
T \le fN
$$
che si esplicita:
$$
Y \cos{\beta} - Q\sin\beta \le f
(Y \sin\beta+ Q \cos\beta)
$$
Questo nell'ipotesi in cui la forza tangenziale sia diretta verso l'alto (diagramma di SX).

### Formula di Pochet-Nadal

![Schermata 2024-02-06 alle 16.53.13.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2016.53.13.png)

La formula di Pochet-Nadal offre un criterio più prudenziale di stabilità

Supponendo di trovarci già nella condizione in cui il bordino sia già risalito rispetto alla rotaia, e che la forza tangenziale sia diretta verso il basso, impongo che la forza tangenziale sia maggiore dell'attrito
$$
T \ge fN
$$
ovvero, esplicitando
$$
Y \cos{\beta} - Q\sin\beta \ge f
(Y \sin\beta+ Q \cos\beta)
$$
la quale può essere espressa nella forma:

```ad-Teo
title: Formula di Pochet-Nadal
$$
\frac{Y}{Q} \le \frac{\tan\beta-f}{1+f \tan\beta}
$$
dove $\frac{Y}{Q}$ è detto **coefficiente di svio**
```

L'<mark style="background: #BBFABBA6;">usura del bordino</mark> aumenta $\beta$, migliorando la stabilità allo svio --> accentua però il consumo del bordino e della rotaia
Con <mark style="background: #BBFABBA6;">rotaie bagnate</mark> il coefficiente di svio aumenta, perché la maggiore scivolosità riduce la forza di attrito la quale consente l'arrampicamento della ruota lungo la parete laterale del fungo.

## Utilizzazione dell'aderenza in trazione

L'aderenza degli pneumatici assume rilevanza
- In curva
- In frenatura
- In trazione

In particolare, in trazione, risulta particolarmente rilevante nei casi di accelerazione in salita.
Trascurando tutte le resistenze naturali al moto, la forza di trazione applicata alle ruote motrici deve equilibrare, a velocità costante, la componente della gravità parallela alla via.

![Schermata 2024-02-06 alle 17.12.01.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-06%20alle%2017.12.01.png)

**TRAZIONE POSTERIORE**
Nella condizione di limite con **trazione posteriore**:
$$
R_{2}(m+n) = h \cdot P \sin\alpha + m \cdot P\cos\alpha
$$
che diventa:
$$
R_{2} = \frac{h \cdot P \sin\alpha + m \cdot P\cos\alpha}{m+n}
$$
Al limite di aderenza
$$
\varphi\cdot R_{2} = P \cdot \sin\alpha
$$
e quindi, sostituendo
$$
\varphi \frac{h \cdot P \sin\alpha + m \cdot P\cos\alpha}{m+n}  = P \sin\alpha
$$
da cui, dividendo per $\cos\alpha$ possiamo trovare la relazione
$$
\tan\alpha = \frac{m\varphi}{m+n-\varphi\cdot h}
$$
e quindi:
- Se <mark style="background: #BBFABBA6;">aumenta l'altezza del baricentro</mark> ($h$), la pendenza limite aumenta
- Se <mark style="background: #FF5582A6;">aumenta la distanza tra baricentro e ruote motrici</mark> ($m$), dato un certo passo $p$, la pendenza limite si riduce
- Se <mark style="background: #BBFABBA6;">aumenta il coefficiente di aderenz</mark>a $\varphi$, la pendenza limite aumenta

Si deve in ogni caso verificare la condizione di guidabilità, $R_{1} > 0$

**TRAZIONE ANTERIORE**
Nel caso di trazione anteriore, si trova che la pendenza limite in condizione di aderenza è
$$
\tan\alpha = \frac{\varphi (p-m)}{p + \varphi h}
$$
**TRAZIONE INTEGRALE**
$$
\tan\alpha = \varphi
$$
- La pendenza massima è **indipendente** dalla geometria del veicolo
- La pendenza limite dipende solo dal coefficiente di aderenza longitudinale $\varphi$

❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ aderenza in trazione con rimorchio
❗❗❗❗❗❗❗❗❗❗❗❗❗


## Utilizzazione dell'aderenza in frenatura

### Autovettura a 2 assi

Se le forze frenanti fossero esattamente ripartite come i carichi sulle singole ruote, la decelerazione massima ottenibile sarebbe, dato che al limite di aderenza
$$
\frac{P}{g} d = \varphi P
$$
e quindi la decelerazione massima
$$
d = \varphi g
$$

Essendo il peso dell'auto non distribuito in modo omogeneo sui due assi, calcoliamo che rapporto c'è tra la forza frenante al limite di aderenza sui due assi.
Questo rapporto, $\alpha$ sarà (si omettono i conti ottenuti tramite l'equilibrio dei momenti):
$$
\alpha = \frac{F_{1}}{F_{2}} = \frac{R_{1}}{R_{2}}
$$
Fissato il coefficiente di aderenza $\varphi$ bisogna far si che la forza frenante venga ripartita secondo $\alpha$ sui due assi.

Nelle auto tradizionali il rapporto $\alpha$ è fisso e imposto dal costruttore. Nel caso particolare in cui il coefficiente di aderenza incontrato sia effettivamente quello di progetto, si può frenare con tutte le ruote al limite di aderenza. Altrimenti solo uno dei due assi sarà al limite di aderenza, mentre l'altro si troverà al di sotto.

![04 - Dinamica dei veicoli - VIT 2024-02-07 16.32.29.excalidraw.png](/img/user/Excalidraw/04%20-%20Dinamica%20dei%20veicoli%20-%20VIT%202024-02-07%2016.32.29.excalidraw.png)


In celeste è mostrato l'andamento della decelerazione massima idealmente ottenibile quando il coefficiente di aderenza reale ($\varphi$) coincide con quello di progetto ($\varphi_{p}$)

- $\varphi<\varphi_{p}$ - decelerazione limitata dall'asse posteriore: slitta prima
- $\varphi>\varphi_{p}$ - decelerazione limitata dall'asse anteriore

Nella realtà quindi la decelerazione effettiva risulta sempre minore rispetto alla teorica massima ottenibile.

Per ovviare a questo problema ci sono dispositivi che **modificano dinamicamente il rapporto di frenatura**.

Un ulteriore problema è dovuto allo squilibrio dei carichi generato dal **rallentamento delle masse rotanti**. Anche l'enegia di queste masse va dissipata dai freni. Non ha effetto sull'aderenza ma per l'equilibrio va considerata nel calcolo di $\alpha$.






















___
___
___
- [?] Il pendolante, trascurando il problema dell'interoperabilità dell'infrastruttura, permetterebbe sovralzi maggiori?
- [ ] Vedere deragliamento AV Spagna (santiago de compostela)

metropolitana di norimberga, automatica, non ha le porte di banchina ma ha laser che individuano ostacoli sui binari e mandano in frenatura il treno.



- [?] Stiamo lavorando sempre senza altre resistenza?

[[4. Dinamica dei Veicoli - VIT.pdf#page=10&selection=153,0,153,26|4. Dinamica dei Veicoli - VIT, page 10]]
Passando da rettilineo (acc centripeta = 0), in curva c'è accelarazione. Se passiamo direttamente in curva avremmo una variazione di acc. nel tempo praticmaente infinito portando a disconfort molto alto. Il raggio della curva a livello planimetrico non è direttamente pari a R ma passa gradualmente.
Ci sono dei raccordi planimetrici. In ambito stradale di solito si usa la clodoide. In campo ferroviario la parabola cubica.
Nel caso ferroviario servirebbe anche un raccordo altimetrico per raccordare il sovralzo. 
In ferrovia si sfrutta il raccordo per variare sia la curvatura che il sovralzo. 
