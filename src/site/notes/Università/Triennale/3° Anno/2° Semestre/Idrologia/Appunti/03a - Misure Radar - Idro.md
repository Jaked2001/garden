---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/idrologia/appunti/03a-misure-radar-idro/"}
---

# [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03a - Misure Radar - Idro\|03a - Misure Radar - Idro]]



# RADAR

Siamo interessati a stimare il campo di pioggia nello spazio, da remoto. Possiamo usare il radar.

Rispetto a quanto visto fino ad ora cambia il paradigma: 
- Quando misuriamo l'[[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Altezza di pioggia\|altezza di pioggia]], misuriamo con lo strumento l'altezza.
- Col radar, misuriamo un'altra grandezza e da quello ricaviamo indirettamente le misure di pioggia

Questo metodo ha sia vantaggi che svantaggi:
- [p] Recuperiamo il dato spaziale su un'area **molto vasta**
	- Questo permette di ridurre i tempi di gestione di un evento potenzialmente pericoloso 
- [c] Commettiamo un errore maggiore perché misuriamo una grandezza per via indiretta

```ad-Definizione
title: Radar

**RADAR** = **RA**dio **D**etection **A**nd **R**anging

Il **radar** è uno strumento elettromagnetico *attivo* e *indiretto* con *misura areale*: un'antenna che emette e riceve.
- **attivo:** la misura viene effettuata in risposta a un segnale trasmesso
- **indiretto:** non misuro le precipitazioni direttamente, ma misuro l'acqua precipitabile
- **misura areale:** la misura avviene su un'area divisa in unità elementari

```

## Ipotesi di lavoro

```ad-tip
title: Ipotesi
- Le particelle da rilevare, le gocce di pioggia, sono approssimabili a simmetria sferica
- Tutta l'acqua precipitabile si trasforma in precipitazione e cade al suolo

```


## Misure radar di pioggia


Le gocce d'acqua presenti nell'atmosfera, ci fanno capire, sulla base di come il segnale elettromagnetico viene riflesso, **la quantità d'acqua in sospensione** presente nell'atmosfera.

Il [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03a - Misure Radar - Idro#RADAR\|#RADAR]] deve essere posto in punto abbastanza alto. Se nella linea visiva del radar c'è un ostacolo, nasconde tutto quello che c'è dietro

Il radar gira ogni minuto.


![Schermata 2024-03-19 alle 08.27.58.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2008.27.58.png)

Il raggio d'azione del radar dipende dalla potenza. Più andiamo lontano, più occorre potenza. In particolare, la **potenza $P$ assorbita da un volume elementare di pioggia** è data da:
$$
P = \frac{CLZ}{r^{2}}
$$
dove:
- $C:$ costante che dipende dalle caratteristiche del radar
- $L:$ frazione perduta per attenuazione
- $Z:$ fattore di riflettività del radar

Per questo il radar è messo o a terra o su un veicolo.

Quando il radar intercetta il nubifragio, il segnale viene modificato. L'antenna è in grado di capire a che distanza è la modifica del segnale e a capire qual è l'energia riflessa.

Il RADAR non è orizzontale. Non vede pioggia al suolo: vede acqua condensata nell'atmosfera. Non sa se è pioggia, acqua che condensa o acqua che evapora.

Ha un piccolo raggio verticale di $1\div 1.5 °$. Più siamo lontani, più investiga una grande porzione di atmosfera e a quote più elevate.

Più ci si allontana dal radar, meno è precisa la misura --> La misura a grandi distanze è più incerta.

### Bande di funzionamento

![Schermata 2024-03-19 alle 08.35.44.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2008.35.44.png)

Quelli della [[Protezione Civile\|Protezione Civile]] sono in banda C.

Quelli portatili sono in banda X e sono più piccoli. Quelli in Banda S sono usati prevalentemente in [[United States of America\|USA]].

COSA MISURA?
- Riflettività del segnale
- Velocità doppler
- Dispersione della velocità doppler
- Riflettività differenziale

Dobbiamo trovare un modo di trasformare quello che misuriamo effettivamente e la pioggia che noi pensiamo cada al suolo.

### Formula Z-R di Marshall & Palmer

Applichiamo un filtro.

```ad-Teo
title: Formula Z-R di Marshall & Palmer

La **Formula Z-R di Marshall & Palmer** è una legge di potenza:
$
Z = aR^{b}
$

dove:
- $Z:$ Fattore di reflittività
- $R:$ Intensità di pioggia(?)
- $a$ e $b:$ fattori di calibrazione, che dipendono dal tipo di nubifragio

```

#### Metodo analitico di calibrazione del radar

Si contano le gocce.

Inapplicabile su grande scala

#### Fattori di errore delle misure radar

Dobbiamo conoscere l'incertezza con cui raccogliamo le misure, e il grado di incertezza.

- Il [[Università/Triennale/3° Anno/2° Semestre/Idrologia/Appunti/03a - Misure Radar - Idro#RADAR\|#RADAR]] misura la l'acqua in sospensione e non la pioggia che effettivamente cade al suolo
- L'acqua a bassa quota può sfuggire
- La pioggia che si forma ad alta quota potrebbe non arrivare mai al suolo

Ci sono poi una serie di **fattori di disturbo**:
- Falsi eco dovuti alla evaporazione della pioggia dal suolo
- Riflessione del suolo - **Ground Clutter**
- Aumento di riflettività dovuto agli strati atmosferici con elevato contenuto di ghiaccio


![Schermata 2024-03-19 alle 08.52.07.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2008.52.07.png)

![Schermata 2024-03-19 alle 08.56.22.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2008.56.22.png)

Fonti di errore:
1. Il fascio è più alto della nube a grande distanza
2. Ciò che evapora da terra (laghi) è letto come precipitazione
3. Si perde le informazioni sui rilievi
4. Bright-band (riflessione dovuta al ghiaccio): blocca la radiazione e non si vede oltre
5. Sottostima dell'intensità della pioggia debole a causa dell'assenza di gocce grandi
6. Propagazione anomala: tipo miraggio del deserto

![Schermata 2024-03-19 alle 08.59.05.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-03-19%20alle%2008.59.05.png)

Usando le stazioni pluviografiche presenti al suolo, calibro il radar in modo che restituisca, nei punti in cui misuro direttamente la pioggia, i valori corretti (con il minor scarto possibile).

![Schermata 2024-03-19 alle 09.01.42.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2009.01.42.png)

Al suolo, usiamo modelli idrologici in coordinate cartesiane. Il radar, restituisce valori in coordinate polari.


### Mosaicatura radar

![Schermata 2024-07-14 alle 10.17.49.png](/img/user/Schermata%202024-07-14%20alle%2010.17.49.png)

Per aumentaer l'accuratezza dei dati radar, si cerca di far si che ogni porzione del territorio sia investito da almeno 3 radar. Si avranno quindi:
- Zone a **mosaicatura parziale** (verde)
- Zone a **mosaicatura completa** (rosso)

Si effettua così il *data fusion*

### Misure satellitari

Per evitare alcuni problemi, si può pensare di mettere i radar sul satellite.

Satelliti geostazionari: guardano sempre lo stesso punto della Terra. Ruotano solidalmente alla Terra. Per essere in orbita geostazionaria però devono stare a 36000km

A quelle distanze un radar classico non funziona: il satellite misura solo le cose che accadono più in quota nell'atmosfera. Permette di capire un'evoluzione, ma non dice nulla di dove al suolo stia piovendo.

![Schermata 2024-03-19 alle 09.19.09.png](/img/user/Universit%C3%A0/Triennale/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2009.19.09.png)

Altri sturmenti:
- Radiometri - misurano i livelli degli specchi d'acqua o l'umidità al suolo









