---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/06-cartografia-tp/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP\|06 - Cartografia - TP]]

## Piano delle rappresentazione cartografica

Spesso si è interessati a rappresentare lo spazio su un piano cartografico. Questo comporta alcune problematiche. Infatti è impossibile distendere perfettamente un ellissoide su un piano, almeno senza introdurre delle deformazioni.

![06 - Cartografia - TP 2024-06-10 14.09.04.excalidraw.png](/img/user/Excalidraw/06%20-%20Cartografia%20-%20TP%202024-06-10%2014.09.04.excalidraw.png)


In particolare, si avranno sempre le seguenti deformazioni
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Modulo deformazione lineare\|Deformazioni lineari]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Modulo deformazione areale\|Deformazioni areali o di superficie]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Deformazione angolare\|Deformazioni angolari]]

#### Rappresentazione afilattica

```ad-Definizione
title: Rappresentazione afilattica

Una rappresentazione si dice **afilattica** quando cerca di minimizzare tutte le deformazioni

```

In particolare risulta afilattica una rappresentazione in scala in cui, proprio per via della scala, le deformazioni non sono percepibili.

### Modulo deformazione lineare

```ad-Definizione
title: Modulo di deformazione lineare ($m_{l}$)

Il **modulo di deformazione lineare** è definito come il rapporto:
$
m_{l} = \frac{dS_{r}}{dS_{e}}
$
dove:
- $dS_{r}:$ Distanza infinitesima sul piano cartografico
- $dS_{e}:$ Distanza infinitesima sull'ellissoide

```

$m_{l}$ misura il livello di contrazione o distensione che le distanze subiscono quando le si misurano sull'ellissoide o sul piano cartografico.
$$
\begin{cases}
0 \le &m_{l} < 1 \Longrightarrow \text{Contrazione} \\
&m_{l} > 1 \Longrightarrow \text{Distensione}
\end{cases}
$$


### Modulo deformazione areale

```ad-Definizione
title: Modulo di deformazione areale o superficiale ($m_{A}$)

Il modulo di deformazione areale è definito come il rapporto:
$
m_{A} = \frac{dA_{r}}{dA_{e}}
$
dove:
- $dA_{r}:$ Superficie infinitesima sul piano cartografico
- $dA_{e}:$ Superficie infinitesima sull'ellissoide


```

$m_{l}$ misura il livello di contrazione o distensione che le superici subiscono quando le si misurano sull'ellissoide o sul piano cartografico.

#### Rappresentazione equivalente

```ad-Definizione
title: Rappresentazione equivalente

Una rappresentazione si dice **equivalente** quando, in ogni punto di essa, si ha che il [[#Modulo deformazione areale]] $m_{l}=1$.

```

La [[Proiezione conica equivalente di Albers\|Proiezione conica equivalente di Albers]] è una rappresentazione equivalente.

### Deformazione angolare

```ad-Definizione
title: Deformazione angolare ($\delta$)

La **deformazione angolare** è definita come la differenza tra:
$
\delta = \delta_{r}-\delta_{e}
$
dove:
- $\delta_{r}:$ angolo tra due segmenti sul piano cartografico
- $\delta_{e}:$ angolo tra i due segmenti corrispondenti sull'ellissoide


```

#### Rappresentazione conforme

```ad-Definizione
title: Rappresentazione conforme

Una rappresentazione si dice **conforme** quando, in ogni punto di essa, si ha che la [[#Deformazione angolare]] $\delta = 0$

```

Sono rappresentazioni conformi:
- La [[Carta di Cassini-Soldner\|Carta di Cassini-Soldner]]
- La [[Carta di Mercatore\|Carta di Mercatore]]

## Piano della carta disegnata

Ai fini pratici è necessario disporre di rappresentazioni in scala. Si ha a che fare quindi con 2 piani:
- Il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano delle rappresentazione cartografica\|#Piano delle rappresentazione cartografica]]
- Il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano della carta disegnata\|#Piano della carta disegnata]]

![06 - Cartografia - TP 2024-06-10 15.00.43.excalidraw.png](/img/user/Excalidraw/06%20-%20Cartografia%20-%20TP%202024-06-10%2015.00.43.excalidraw.png)


Nel diagramma sopra
- $P_{r}:$ il punto che è stato trasformato dall'ellissoide al [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano delle rappresentazione cartografica\|#Piano delle rappresentazione cartografica]]
- $P_{c}:$ il punto rimpicciolito nel [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano della carta disegnata\|#Piano della carta disegnata]]

```ad-note
title: Osservazione

Nel passaggio dal [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano delle rappresentazione cartografica\|#Piano delle rappresentazione cartografica]] al [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano della carta disegnata\|#Piano della carta disegnata]] si compie una **trasformazione isotropa**, ossia priva di qualsisasi deformazione.

```

### Limite di graficismo

Quando si passa al [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano della carta disegnata\|#Piano della carta disegnata]] l'oggetto che si vuole andare a rappresentare potrebbe, successivamente alla contrazione dovuta alla scala, diventare talmente piccolo che non siamo tecnicamente in grado di rappresentarlo.

Per esempio, dato un quadrato sul [[#Piano delle rappresentazione cartografica]] di lato $1\,\rm m$, se lo si volesse rappresentare sul [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano della carta disegnata\|#Piano della carta disegnata]] con un fattore di scala di $1:100\,000$, questo dovrebbe avere un lato di $10^{-5}\,\rm m = 0.02 \,\rm mm$. Gli strumenti di stampa a nostra disposizione semplicemente non sono in grado di disegnare oggetti così piccoli.

```ad-Definizione
title: Limite di graficismo ($\varepsilon$)

Il limite di graficismo è la grandezza più piccola che può essere rappresentata sul [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Piano della carta disegnata\|#Piano della carta disegnata]].

Si tratta di un valore convenzionale, generalmente pari a
$
\varepsilon=0.2 \,\rm mm
$

```

Quando l'oggetto che si vuole rappresentare risulta più piccolo del limite di graficismo, si usa un simbolo detto **segno convenzionale**.

Inoltre, qualora le deformazioni risultino, nel [[#Piano della carta disegnata]], minori del limite di graficismo, queste non saranno registrate. Il limite di graficismo è pertanto anche usato per definire il **limite di piccolezza** delle deformazioni.

#### Precisione dell'informazione sul piano della carta disegnata

Il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Limite di graficismo\|#Limite di graficismo]] sul [[#Piano della carta disegnata]] definisce la precisione che si può ottenere ricavando una grandezza da una carta in scala.

In particolare, sia la carta in scala $1:x$, sia $\varepsilon$ il limite di graficismo, la precisione massima dell'informazione ricavabile dalla carta è:
$$
x\cdot \varepsilon \times 10^{-3} \,\rm m
$$

## Rappresentazione di Gauss

```ad-Definizione
title: Rappresentazione di Gauss

La **rappresentazione di Gauss** è una [[#Rappresentazione conforme]] della Terra.

```

![06 - Cartografia - TP 2024-06-10 15.35.25.excalidraw.png](/img/user/Excalidraw/06%20-%20Cartografia%20-%20TP%202024-06-10%2015.35.25.excalidraw.png)


La rappresentazione di gauss consiste nel:
- Scegliere un meridiano di riferimento
- Costruire un cilindro a base ellittica tangente nel meridiano scelto
- Proiettare i punti dell'ellissoide sul cilindro

I punti sono proiettati considerando la semiretta avente origine nel centro dell'ellissoide. Questa semiretta incontra il punto $P_{e}$ sull'ellissoide e interseca il cilindro nel punto $P_{r}$.

```ad-note
title: Osservazione
I punti che giacciono sull'asse del cilindro, vengono proiettati sulla superficie laterale del cilindro a distanza infinita.

I punti che giacciono sul meridiano di tangenza vegnono proiettati su se stessi.

```

il [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Modulo deformazione lineare\|#Modulo deformazione lineare]] è pertanto limitato tra:
$$
\begin{align}
m_{l} &= 1: \quad \text{In corrispondenza del meridiano di tangenza} \\
m_{l} &= \infty: \quad \text{In corrispondenza dell'asse del cilindro}
\end{align}
$$
```ad-note

In questa configurazione ci sono solamente [[#Modulo deformazione lineare|deformazioni lineari]] per **dilatazione**:
$
m_{l} > 1
$

```

Bisogna cercare di costruire una [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione afilattica\|#Rappresentazione afilattica]], dove cioè le deformazioni siano abbastanza ridotte.

Osserviamo che le deformazioni sono molto vicine a $m_{l}=1$ per punti vicini al meridiano di tangenza. In particolare, la rappresentazione si può considerare [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione afilattica\|afilattica]] entro circa $3\degree$.

La rappresentazione di Gauss gode quindi delle seguenti proprietà:

```ad-tip
title: Proprietà della rappresentazione di Gauss
- È una [[#Rappresentazione conforme]]
- È una [[#Rappresentazione afilattica]] entro $\pm 1.5\degree$ dal meridiano di tangenza
- Ha [[#Modulo deformazione lineare]] sempre di **dialtazione**: $1 \le m_{l}< \infty$

```

### Rappresentazione di Gauss contratta

![06 - Cartografia - TP 2024-06-10 15.58.07.excalidraw.png](/img/user/Excalidraw/06%20-%20Cartografia%20-%20TP%202024-06-10%2015.58.07.excalidraw.png)


La rappresentaizone di Gauss Contratta è di fatto una [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione di Gauss\|#Rappresentazione di Gauss]] in cui il cilindro che si prende in considerazione risulta non essere più tangente all'ellissoide terrestre, ma **secante**

Questo fa si che ci siano dei punti le cui proiezioni subiscono una <mark style="background: #FF5582A6;">dilatazione</mark> (quelli sugli archi rossi) e altri che subiscono invece una <mark style="background: #ADCCFFA6;">contrazione</mark>.

In questo modo, il limite di piccolezza è rispettato per una fascia maggiore di ampiezza non più 1.5 ma ben
$$
\pm3\degree
$$
raddoppiando rispetto alla classica [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione di Gauss\|#Rappresentazione di Gauss]].

#### Coefficiente di contrazione

Nel passaggio da una [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione di Gauss\|#Rappresentazione di Gauss]] a una [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione di Gauss contratta\|#Rappresentazione di Gauss contratta]], come dice il nome stesso, si ha la contrazione delle distanze. Il fattore di contrazione è detto **Coefficiente di contrazione** e vale circa $k = 0.996$.

In particolare, quando si passa dalle coordinate in [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione di Gauss contratta\|#Rappresentazione di Gauss contratta]] ($X,Y$) alle coordinate in [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione di Gauss\|#Rappresentazione di Gauss]] classica ($X^{*},Y^{*}$), si devono rispettare le seguenti relazioni:
$$
\begin{cases}
X^{*} &= kX \\
Y^{*} &= kY
\end{cases}
$$

#### Sistema UTM

Il sistema UTM deriva direttamente dalla [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione di Gauss contratta\|#Rappresentazione di Gauss contratta]]. Come si è detto infatti questa è [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Rappresentazione afilattica\|afilattica]] solo in una fascia di ampiezza pari a $6\degree$ centrati nel meridiano di tangenza. Per fare in modo di rappresentare tutta la Terra, si è divisa quest'ultima in fasce ognuna ampia $6\degree$ (arrivando così a $\frac{360}{6} = 60$). Ogni fascia è detta **fuso**. Sulla Terra si contano quindi in tutto 60 fusi.

I fusi si contano a partire dall'anti meridiano di Greenwich. Pertanto, il fuso con [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/Sistemi di coordinate fondamentali#Longitudine\|longitudine]] compresa tra 0 e $6\degree$ è il fuso 31.

![06 - Cartografia - TP 2024-06-10 16.15.47.excalidraw.png](/img/user/Excalidraw/06%20-%20Cartografia%20-%20TP%202024-06-10%2016.15.47.excalidraw.png)



L'Italia è compresa nei fusi: 32, 33, 34.

I fusi in realtà non sono presi completi dal Polo Sud al Polo Nord. Infatti qui i fusi diventano molto stretti e per descrivere oggetti relativamente piccoli a latitudini molto elevate sarebbe necessario un numero consistente di fusi. Pertanto si è deciso di considerare delle zone attorno a entrambi i poli con caratteristiche omogenee che vengono rappresentate su delle proiezioni a parte:
- Il polo nord cerca di includere tutte le aree non occupate da terre emerse. Si arriva alla LAT $84\degree\,\rm N$
- Il polo sud cerca di includere tutte le terre emerse dell'Antartide. Si arriva alla LAT $80\degree\,\rm S$

La rappresentazione di un fuso assume quindi il seguente aspetto:

![06 - Cartografia - TP 2024-06-10 17.30.50.excalidraw.png](/img/user/Excalidraw/06%20-%20Cartografia%20-%20TP%202024-06-10%2017.30.50.excalidraw.png)



##### Coordinate Est-Nord


![06 - Cartografia - TP 2024-06-10 17.30.50.excalidraw.png](/img/user/Excalidraw/06%20-%20Cartografia%20-%20TP%202024-06-10%2017.30.50.excalidraw.png)


Per semplicità, si vuole fare in modo che le coordinate dei punti siano sempre positive all'interno di un fuso.

Ogni fuso del [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/06 - Cartografia - TP#Sistema UTM\|#Sistema UTM]] è identificato dal meridiano centrale.

Le coordinate cartografiche di un punto sono la $X$ e la $Y$ del punto, i cui zeri sono rispettivamente sul meridiano centrale e sull'Equatore.

Questo però fa si che tutti i punti dell'emisfero australe e tutti i punti a ovest del meridiano centrale abbiano coordinate Y e X negative.

Posso però pensare di prendere il punto più a sud ($\color{green} B$) e quello più a ovest $\color{orange} A$ e sommare alle coordinate di tutti i punti dei valori in modo tale che questi abbiano coordinate positive. Il valore che si somma è detto **falsa origine**. In questo modo si otterrebbe che:
$$
\begin{cases}
E = kX + E_{fo} \\
N = kY + N_{fo}
\end{cases}
$$
Dove
- $E,N$ sono le coordinate Est e Nord (rispettive di $X$ e $Y$ ma sempre positive)
- $E_{fo}, N_{fo}:$ sono le false origini
- Si è eseguita la contrazione con $k$

Il sistema UTM prevede le seguenti convenzioni:
$$
\begin{cases}
E_{fo} = 500\,\rm km  \\
N_{fo} =
\begin{cases}
0\,\rm km \quad \text{in emisfero boreale} \\
10\,000 \,\rm km \quad \text{in emisfero australe}
\end{cases}
\end{cases}
$$

```ad-attention
title: Attenzione

Per come si sono definite le false origini adesso ci saranno dei punti che nei due emisferi hanno le stesse coordinate.

Inoltre, se non si indica in quale fuso ci si trova, conoscendo solo le coordinate Est e Nord è impossibile risalire alla posizione globale di un punto.
```

### Rappresentazione Gauss-Boaga


FUSO OVEST
$$
\begin{cases}
E_{fo} = 1500\,\rm km  \\
N_{fo} =
\begin{cases}
0\,\rm km \quad \text{in emisfero boreale} \\
10\,000 \,\rm km \quad \text{in emisfero australe}
\end{cases}
\end{cases}
$$


FUSO OVEST
$$
\begin{cases}
E_{fo} = 2520\,\rm km  \\
N_{fo} =
\begin{cases}
0\,\rm km \quad \text{in emisfero boreale} \\
10\,000 \,\rm km \quad \text{in emisfero australe}
\end{cases}
\end{cases}
$$


❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

## Calcolo di distante

