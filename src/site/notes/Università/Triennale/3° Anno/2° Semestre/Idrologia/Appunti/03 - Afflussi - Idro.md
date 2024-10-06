---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/idrologia/appunti/03-afflussi-idro/"}
---

# [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03 - Afflussi - Idro\|03 - Afflussi - Idro]]



Essendo le precipitazioni fortemente dipendenti dallo spazio, l'afflusso pluviometrico non può essere calcolato, su un intera regione, semplicemente attribuendo a tutta l'area l'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Altezza di pioggia\|altezza di pioggia]] di un'unico [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Pluviometro\|pluviometro]].

Occorre pertanto effettuare un [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03 - Afflussi - Idro#Ragguaglio spaziale delle piogge\|#Ragguaglio spaziale delle piogge]].

## Ragguaglio spaziale delle piogge

```ad-Definizione
title: Ragguaglio spaziale delle piogge

Il **ragguaglio spaziale delle piogge** è la valutazione dell’[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Altezza di pioggia\|altezza di pioggia]] media su un area a partire da quella nota in un punto

```

Permette di definire un coefficiente, detto [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03 - Afflussi - Idro#Fattore di ragguaglio\|#Fattore di ragguaglio]]

### Fattore di ragguaglio

```ad-Definizione
title: Fattore di ragguaglio ($R$ oppure $C_{R}$)

Il **Fattore - o coefficiente - di ragguaglio** è l'[[02 - Piogge Intense - Idro#Altezza di pioggia|altezza di pioggia]] media sull'area fratto quella misurata sul punto.
$
R = \frac{h_{\delta, A}}{h_{\delta}}
$
dove:
- $h_{\delta, A}:$ [[02 - Piogge Intense - Idro#Altezza di pioggia|altezza di pioggia]] media sull'area
- $h_{\delta}:$ [[02 - Piogge Intense - Idro#Altezza di pioggia|altezza di pioggia]] misurata in un punto 

Possiamo anche scrivere:
$
h_{\delta, A} = R \cdot h_{\delta}
$

```


Ipotizziamo che sia sempre $R \le 1$. È un ipotesi di lavoro che vale per frequenze basse ([[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro\|piogge intense]]).

$R$ è funzione della frequenza.

![Schermata 2024-03-18 alle 11.02.34.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-18%20alle%2011.02.34.png)

$R$ aumenta
- all'*aumentare* della **durata**
- al *diminuire* dell'**Area**
- al *diminuire* dell'intensità e quindi del **[[Tempo di ritorno\|tempo di ritorno]]** ($T_{R}$) = il tempo tra due eventi considerati estremi



Quando ho a disposizione, in un'area di interesse, più misure, posso usare tre metodi per definire un'altezza media per quell'area:
- [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03 - Afflussi - Idro#Metodo della media\|#Metodo della media]]
	- *Vincolo matematico:* Se i punti sono distribuiti nell'area in modo uniforme
	- *Vincolo fisico:* distanza dal mare, esposizione dei versanti, quota costanti nell'area
- [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03 - Afflussi - Idro#Metodo dei poligoni di Thiessen\|#Metodo dei poligoni di Thiessen]]
- [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03 - Afflussi - Idro#Metodo delle isoiete\|#Metodo delle isoiete]]

### Metodi di ragguaglio spaziale delle piogge

#### Metodo della media

Il Metodo della media è un metodo di [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03 - Afflussi - Idro#Ragguaglio spaziale delle piogge\|#Ragguaglio spaziale delle piogge]]

```ad-Teo
title: Metodo della Media

Si assume come [[02 - Piogge Intense - Idro#Altezza di pioggia|altezza di pioggia]] la media ($h_{A}$, la media delle altezze misurate ai pluviometri disponibili ($h_{i}$.

$
h_{A} = \frac{1}{N} \sum\limits_{i=1}^{N}h_{i}
$

```

Quando il terreno è molto omogeneo
$$
w_{i} = \frac{1}{N}
$$

La posso usare quando:
- L'area è vicina al mare
- Non ci sono notevoli variazioni di quota
- L'area non è esposta a versanti

#### Metodo dei topoieti


**Il Metodo dei Topoieti**, o metodo dei **Poligoni di Thiessen** (vd. anche: [[Università/Triennale/2° anno/2° Semestre/GIS/GIS 1/5. DEM#Poligoni di Thiessen\|poligoni di Thiessen - GIS]]) è un metodo di [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03 - Afflussi - Idro#Ragguaglio spaziale delle piogge\|#Ragguaglio spaziale delle piogge]].

![03 - Afflussi - Idro 2024-03-18 11.14.41.excalidraw.png](/img/user/Excalidraw/03%20-%20Afflussi%20-%20Idro%202024-03-18%2011.14.41.excalidraw.png)


I poligoni sono definiti tracciando la linea equidistante a due punti dati. Ad ogni poligono assegno poi il valore del punto noto all'interno.

![Schermata 2024-05-02 alle 15.27.27.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-05-02%20alle%2015.27.27.png)

Si assume come [[02 - Piogge Intense - Idro#Altezza di pioggia|altezza di pioggia]] media sulla regione, la media delle altezze delle stazioni adiacenti pesata in base all'area dei topoieti.

È utile quando cambia la distribuzione geometrica del territorio (distribuzione dei pluviografi) ma non le caratteristiche fisiche (morfologia del territorio)

### Metodo delle isoiete

```ad-Definizione
title: Isoiete

Le **isoiete** sono le linee a uguale pioggia

```

![Schermata 2024-03-18 alle 11.20.06.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-18%20alle%2011.20.06.png)


Si usa in presenza di un rilievo.

Si fa l'ipotesi di andamento lineare lungo i segmenti

## Controllo dei dati
### Metodo della doppia massa

Ho dubbi su un pluviometro ma non su un altro. Faccio la cumulata su quello di riferimento e su quello di cui ho dubbi. Se i dati sono a retta costante, va tutto bene. Negli eventuali tratti con cambio di pendenza, vuol dire che qualcuno ha avuto qualche problema.

![Schermata 2024-05-02 alle 15.39.30.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-05-02%20alle%2015.39.30.png)

![Schermata 2024-03-18 alle 11.25.05.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-03-18%20alle%2011.25.05.png)


❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗ FINIRE DI STUDIARE DALLE ESERCITAZIONI (7)
❗❗❗❗❗❗❗❗❗❗❗❗





