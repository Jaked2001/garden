---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/idrologia/appunti/05a-deflusso-di-base-idro/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Idrologia/Appunti/05a - Deflusso di base - Idro\|05a - Deflusso di base - Idro]]

```ad-Definizione
title: Deflusso di base

Il **deflusso di base** è il deflusso dovuto ai contributi sotterranei delle sorgenti, quello cioè presente sempre, anche nei periodi non influenzati dalle piogge.

```

Esso sostiene la [[Università/3° Anno/2° Semestre/Idrologia/Appunti/05 - Deflussi - Idro#Portata\|portata]] del bacino quando non piove - cioè nel 90% del tempo.

Quando non piove, il bacino è fortemente influenzato dalle attività dell'uomo: la quantità d'acqua
deve essere quindi gestita nel modo ottimale al fine di soddisfare i bisogni dell’uomo ma anche nell’ottica di mantenere l’equilibrio ecologico.

Si parla pertanto di **deflusso ecologico**: ossia la portata che bisogna mantenere nel corso d’acqua per mantenere l’equilibrio ambientale (portata ecologicamente compatibile).

![Schermata 2024-05-03 alle 17.37.40.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-03%20alle%2017.37.40.png)

Si distinguono inoltre periodi di **magra** e periodi di **piena**.

Siamo particolarmente interessati ai periodi di magra. Durante questi periodi infatti dobbiamo commisurare la quantità d'acqua che preleviamo per la salvaguardia del corpo d'acqua.

Si noti infatti come a Roma dal 1925 in poi le portate minime del Tevere stiano diminuendo anno dopo anno (almeno in termini di trend). Questo è dovuto al fatto che da quegli anni abbiamo cominciato a prelevare, lungo tutto il fiume, quantità maggiori di acqua.

![Schermata 2024-05-03 alle 17.40.31.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-03%20alle%2017.40.31.png)

Lo studio statistico del [[Università/3° Anno/2° Semestre/Idrologia/Appunti/05 - Deflussi - Idro#Deflusso\|deflusso]] richiede la ricostruzione delle portate naturali $Q_{n}$:
$$
Q_{n}(t) = Q_{m}(t) + P(t)
$$
dove:
- $Q_{n}(t):$ Portata naturale
- $Q_{m}(t):$ Portata misurata
- $P(t):$ Prelievi

Occorre pertanto la ricostruzione storica dei prelievi.

## Curve di durata

```ad-Definizione
title: Curva di durata

Una **curva di durata** è realizzata a partire dal grafico delle portate nel tempo. Di ogni valore di portata si riporta quante volte è stato superato o uguagliato in un anno e la serie così ottenuta è ordinata in ordine decrescente. 

Gode delle seguenti caratteristiche:
- Tutti i giorni ($D(Q) = 365$) è verificata la portata $Q_{min}$
- Un solo giorno si verifica la portata $Q_{max}$


```


Le curve di durata sono un utile strumento di diagnosi dei corpi d'acqua.
In particolare:
- **Curva piatta:** corso con comportamento stabile - portata quasi costante nell'anno
- **Curva ripida:** corso con comportamento pericoloso

Per ogni giorno dell'anno si vede quante volte si è raggiunto un valore di portata.

La curva di durata raffigura per quanto tempo è rispettata una data portata. 

![Schermata 2024-05-03 alle 17.50.24.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-03%20alle%2017.50.24.png)


La curva è chiaramente sempre **monotona decrescente**.

![Schermata 2024-05-03 alle 17.52.37.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-03%20alle%2017.52.37.png)

Vediamo che la portata massima di picco si è verificata una sola volta. La seconda portata massima si è verificata 2 volte: Quando il picco è stato proprio quello e quando si è verificato il primo picco. E così via...

Occorre una legge di probabilità delle portate minime: userò una distribuzione appropriata a modellare i valori estremi. Si considerano le portate minime di tutti gli anni di osservazione come realizzazione di un'unica variabile casuale.

Si usa la Distribuzione del minimo valore di tipo EV3 ([[Distribuzione di Weibull\|Distribuzione di Weibull]]):
$$
\mathcal{P}(X\ge x) = 1- \mathcal{P}(x) = 1 - e^{- \left( \dfrac{x-x_{0}}{\varepsilon- x_{0}} \right)^\frac{1}{\lambda}}
$$
Notiamo che ci sono 3 parametri:
- $\lambda$
- $\varepsilon$
- $x_{0}:$ soglia sotto la quale il corso d'acqua non arriva (può essere 0 nel caso di corsi **intermittenti**)

In merito agli indici statistici:
- $\mu = x_{0} + (\varepsilon-x_{0})\Gamma\left( 1+ \frac{1}{\alpha} \right):$ [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Valore atteso o media\|media]]
- $\sigma = \dfrac{\varepsilon-x_{0}}{B(\alpha)}:$ [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Deviazione Standard\|deviazione standard]]
- $\gamma = \dfrac{\mu_{3}}{\sigma^{3}} = f[\Gamma(\alpha), B(\alpha)]:$ [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Coefficiente di asimmetria\|coefficiente di asimmetria]]


Per lo studio delle portate minime bisogna fare attenzione alla carta idrogeologica.

## Curva di esaurimento

Per stimare le portate minime si fa uso delle **curve di esaurimento** - costituiscono la seconda parte dell'idrogramma di piena.

Durante il periodo non influenzato dalla pioggia, le portate d'esaurimento alle sorgenti dipendono dal grado di riempimento delle falde (come le falde restituiscono acqua alla superficie nel periodo non influenzato).

La **curva d'esaurimento** serve a valutare la portata al tempo $t_{2}$ nota la portata al tempo $t_{1}$, se non piove.

![Schermata 2024-05-04 alle 16.45.03.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-04%20alle%2016.45.03.png)

La curva di esaurimento è utile ad esempio a capire se, durante i mesi estivi, l'acqua di un corso sarà sufficiente alle nostre necessità.

### Tracciamento della curva d'esaurimento

La curva di esaurimento si basa su un'ipotesi schematica: la derivata temporale della portata dipende unicamente dalla portata:
$$
\frac{dQ}{dt} = f(Q)
$$
Infatti:
- La portata dipende solo dal riempimento della falda
- La variazione del riempimento deriva solo dalla portata
- La variazione della portata dipende solo dalla portata

Andando a scrivere un'**equazione di bilancio** otteniamo:
$$
\frac{dW(t)}{dt} = I_{e}(t) - D(t) - F(t)
$$
dove:
- $t:$ tempo
- $W_{t}(t):$ il volume totale invasato nell'acquifero
- $I_{e}(t):$ *Infiltrazione efficace*
- $D(t):$ Il *deflusso superficiale di base* nei corsi d'acqua alimentati dall'acquifero
- $F(t):$ Lo *scambio sotterraneo* con altri acquiferi e le *perdite in mare*

L'equazione
$$
\frac{dQ}{dt} = f(Q)
$$
può avere come soluzione:
- Esponenziale: $Q(t) = Q_{0}e^{- \frac{t-t_{0}}{k}}$
- Potenziale: $Q(t) = Q_{0}[ 1-a(t-t_{0})]^{k}$
- Esponenziale multipla:

Le curve di esaurimento quindi rappresentano l'andamento nel tempo del deflusso di un corso d'acqua dopo un evento di pioggia.

Come capire da dove comincia il **deflusso di base** nell'idrogramma di piena? Conviene usare il log naturale della portata. In questo modo, la parte finale risulterà rettilinea. La parte rettilinea è dove comincia il deflusso di base


```ad-note
title: Osservazione

La curva di esaurimento è tipica di un certo corso d'acqua, indipendente dalla portata di picco. Quindi, eventi diversi, avranno comunque curve di esaurimento con andamento uguale.
```

-

```ad-note
title: Risposte di ChatGPT
In idrologia, le curve di esaurimento (o curve di recessione) rappresentano l'andamento nel tempo del deflusso di un corso d'acqua dopo un evento di pioggia o fusione di neve. Queste curve descrivono come il flusso d'acqua diminuisce gradualmente nel tempo fino a ritornare alle condizioni di base.

Il deflusso di base è la componente del deflusso fluviale che proviene dalle sorgenti sotterranee, ossia l'acqua che si infiltra nel suolo e riemerge lentamente nelle acque superficiali. È il flusso minimo che mantiene il corso d'acqua durante periodi di assenza di piogge significative.

Le curve di esaurimento sono strettamente legate al deflusso di base in quanto, durante la fase di recessione, il flusso d'acqua nel fiume tende progressivamente a ridursi fino a raggiungere il deflusso di base. L'andamento della curva di esaurimento può quindi essere utilizzato per stimare la quantità e la durata del deflusso di base.


**Da che punto dell'idrogramma di piena inizia la curva di esaurimento?**

La curva di esaurimento inizia dal punto di massimo dell'idrogramma di piena, noto come il picco di piena. Questo punto rappresenta il momento in cui il deflusso del corso d'acqua raggiunge il suo massimo livello a seguito di un evento di pioggia o fusione di neve. Dopo il picco, il deflusso inizia a diminuire gradualmente, segnando l'inizio della fase di recessione o esaurimento. La curva di esaurimento segue questo andamento decrescente del deflusso fino a stabilizzarsi sul deflusso di base.

**Mentre l'esaurimento cos'è?**
ChatGPT
In idrologia, l'esaurimento si riferisce alla fase del ciclo idrologico durante la quale il flusso di un corso d'acqua diminuisce dopo aver raggiunto il picco di piena. Questa fase di riduzione del deflusso avviene a seguito di un evento di precipitazione o fusione di neve che ha aumentato temporaneamente il livello dell'acqua nel fiume o nel torrente.

L'esaurimento è caratterizzato da una progressiva riduzione del volume d'acqua che scorre, influenzata principalmente da due processi principali:

Ricarica delle falde acquifere: Parte dell'acqua inizia a infiltrarsi nel suolo e a ricaricare le falde acquifere sotterranee.
Riduzione del deflusso superficiale: L'acqua che scorre in superficie diminuisce man mano che le sorgenti temporanee di deflusso (come l'acqua piovana o il disgelo) si esauriscono.
La durata e la forma della curva di esaurimento possono variare a seconda di diversi fattori, come la morfologia del bacino idrografico, la permeabilità del suolo, la vegetazione e le condizioni climatiche.


**In che punto finisce la curva di esaurimento e inizia la curva del deflusso di base?**

La curva di esaurimento termina e inizia la curva del deflusso di base nel punto in cui il deflusso del corso d'acqua si stabilizza e raggiunge un valore minimo relativamente costante, che rappresenta il flusso sostenuto principalmente dalle acque sotterranee. Questo punto non è sempre facile da individuare esattamente, ma in generale si verifica quando l'effetto degli eventi di pioggia o di fusione della neve è completamente smaltito, e il flusso del fiume è mantenuto solo dalle sorgenti sotterranee.

In sintesi:

Curva di esaurimento: Rappresenta la fase di diminuzione del deflusso dopo il picco di piena.
Deflusso di base: Il flusso minimo costante che rimane dopo che le acque superficiali generate dall'evento di piena si sono esaurite, sostenuto principalmente dalle acque sotterranee.
La transizione tra queste due fasi è continua e graduale, e il punto di separazione è dove il deflusso non mostra più una significativa diminuzione con il tempo e si stabilizza su un valore costante.

```


![Schermata 2024-05-04 alle 16.53.01.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-04%20alle%2016.53.01.png)
