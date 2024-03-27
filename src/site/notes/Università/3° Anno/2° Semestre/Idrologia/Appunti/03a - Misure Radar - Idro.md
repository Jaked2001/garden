---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/idrologia/appunti/03a-misure-radar-idro/"}
---

# [[Università/3° Anno/2° Semestre/Idrologia/Appunti/03a - Misure Radar - Idro\|03a - Misure Radar - Idro]]




Stimare il campo di pioggia nello spazio da remoto.

Cambia il paradigma: 
Quando misuriamo l'altezza di pioggia, misuriamo con lo strumento l'altezza.
Col radar, misuriamo un'altra grandezza e da quello ricaviamo indirettamente le misure di pioggia.

Da una parte recuperiamo il dato spaziale, dall'altra commettiamo un errore maggiore perché misuriamo una grandezza indiretta.

Permette di ottenere il campo di pioggia in un'area molto vasta e possiamo quindi ridurre i tempi di gestione di un evento potenzialmente pericoloso.

```ad-Definizione
title: Radar
RADAR = RAdio Detection And Ranging

È uno strumento elettromagnetico *attivo* e *indiretto* con *misura reale*: un'antenna che emette e riceve.

```

Le gocce d'acqua presenti nell'atmosfera, ci fanno capire, sulla base di come il segnale elettromagnetico viene riflesso, come la quantità d'acqua in sospensione presente nell'atmosfera.

Il RADAR deve essere posto in punto abbastanza alto. Se nella linea visiva del radar c'è un ostacolo, nasconde tutto quello che c'è dietro

Il radar gira ogni minuto.

![Schermata 2024-03-19 alle 08.27.58.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2008.27.58.png)

Il raggio d'azione del radar dipende dalla potenza. Più andiamo lontano, più occorre potenza.

$$
P = \frac{CLZ}{r^{2}}
$$
dove:
- $C:$ costante che dipende dalle caratteristiche del radar
- $L:$ frazione perduta per attenuazione
- $Z:$ fattore di riflittività del radar

Per questo il radar è messo o a terra o su un veicolo.

Quando il radar intercetta il nubifragio, il segnale viene modificato. L'antenna è in grado di capire a che distanza è la modifica del segnale e a capire qual è l'energia riflessa.

Il RADAR non è orizzontale. Non vede pioggia al suolo: vede acqua condensata nell'atmosfera. Non sa se è pioggia, acqua che condensa o acqua che evapora.

Ha un piccolo raggio verticale di $1\div 1.5 °$. Più siamo lontani, più investiga una grande porzione di atmosfera e a quote più elevate.

Più ci si allontana dal radar, meno è precisa la misura --> La misura a grandi distanze è più incerta.

### Bande di funzionamento

![Schermata 2024-03-19 alle 08.35.44.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2008.35.44.png)

Quelli della [[Protezione Civile\|Protezione Civile]] sono in banda C.

Quelli portatili sono in banda X e sono più piccoli. Quelli in Banda S sono usati prevalentemente in USA.

COSA MISURA?
- Riflettività del segnale
- Velocità doppler
- Dispersione della velocità doppler
- Riflettività differenziale

Dobbiamo trovare un modo di trasformare quello che misuriamo effettivamente e la pioggia che noi pensiamo cada al suolo.

### Formula Z-R di Marshall & Palmer

Applichiamo un filtro. 

È una legge di potenza, detta formula di Marshall & Palmer

$$
Z = aR^{b}
$$
dove:
- $Z:$ Fattore di reflittività
- $R:$ Intensità
- $a$ e $b:$ fattori di calibrazione, che dipendono dal tipo di nubifragio

#### Metodo analitico di calibrazione del radar

Si contano le gocce.

In applicabile su grande scala

#### Fattori di errore delle misure radar

Dobbiamo conoscere l'incertezza con cui raccogliamo le misure, e il grado di incertezza.

Primo fattore di incertezza:
- Misuriamo in aria ma siamo al suolo
- Ground Clutter: riflessione dei lobi secondari di radiazione emessi intorno al radar

![Schermata 2024-03-19 alle 08.52.07.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2008.52.07.png)

![Schermata 2024-03-19 alle 08.56.22.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2008.56.22.png)

Fonti di errore:
1. Il fascio è più alto della nube a grande distanza
2. Ciò che evapora da terra (laghi) è letto come precipitazione
3. Si perde le informazioni sui rilievi
4. Bright-band (riflessione dovuta al ghiaccio): blocca la radiazione e non si vede oltre
5. Sottostima dell'intensità della pioggia debole a causa dell'assenza di gocce grandi
6. Propagazione anomala: tipo miraggio del deserto
![Schermata 2024-03-19 alle 08.59.05.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-03-19%20alle%2008.59.05.png)

Usando le stazioni pluviografiche presenti al suolo, calibro il radar in modo che restituisca, nei punti in cui misuro direttamente la pioggia, i valori corretti (con il minor scarto possibile).
![Schermata 2024-03-19 alle 09.01.42.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2009.01.42.png)

Al suolo, usiamo modelli idrologici in coordinate cartesiane. Il radar, restituisce valori in coordinate polari.

Per evitare alcuni problemi, si può pensare di mettere i radar sul satellite.

Satelliti geostazionari: guardano sempre lo stesso punto della Terra. Ruotano solidalmente alla Terra. Per essere in orbita geostazionaria però devono stare a 36000km

A quelle distanze un radar classico non funziona: il satellite misura solo le cose che accadono più in quota nell'atmosfera. Permette di capire un'evoluzione, ma non dice nulla di dove al suolo stia piovendo.

![Schermata 2024-03-19 alle 09.19.09.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-03-19%20alle%2009.19.09.png)

Altri sturmenti:
- Radiometri - misurano i livelli degli specchi d'acqua o l'umidità al suolo









