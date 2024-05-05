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
- $Q_{m}(t):$ Portate misurate
- $P(t):$ Prelievi

Occorre pertanto la ricostruzione storica dei prelievi.

## Curve di durata

Le curve di durata sono un utile strumento di diagnosi dei corpi d'acqua.
In particolare:
- Curva piatta: corso con comportamento stabile
- Curva ripida: corso con comportamento pericoloso

La curva di durata raffigura per quanto tempo è rispettata una data portata. 

![Schermata 2024-05-03 alle 17.50.24.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-03%20alle%2017.50.24.png)

In particolare dice che:
- Tutti i giorni ($D(Q) = 365$) è verificata la portata $Q_{min}$
- Un solo giorno si verifica la portata $Q_{max}$

La curva è chiaramente sempre **monotona decrescente**.

![Schermata 2024-05-03 alle 17.52.37.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-03%20alle%2017.52.37.png)

Vediamo che la portata massima di picco si è verificata una sola volta. La seconda portata massima si è verificata 2 volte: Quando il picco è stato proprio quello e quando si è verificato il primo picco. E così via...

Occorre una legge di probabilità delle portate minime: userò una distribuzione appropriata a modellare i valori estremi.

Si usa la Distribuzione del minimo valore di tipo EV3:
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

## Curva di esaurimento


Per stimare le portate minime facciamo uso delle **curve di esaurimento** - costituiscono la seconda parte dell'idrogramma di piena.

Durante il periodo non influenzato, le portate d'esaurimento alle sorgenti dipendono dal grado di riempimento delle falde.

La curva d'esaurimento serve a valutare la portata al tempo $t_{2}$ nota la portata al tempo $t_{1}$, se non piove.

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

Andando a scrivere un'equazione di bilancio otteniamo:
$$
\frac{dW(t)}{dt} = I_{e}(t) - D(t) - F(t)
$$
dove:
- $t:$ tempo
- $W_{t}(t):$ il volume totale invasato nell'acquifero
- $I_{e}(t):$ infiltrazione efficace
- $D(t):$ il deflusso superficiale di base nei corsi d'acqua alimentati dall'acquifero
- $F(t):$ lo scambio sotterraneo con altri acquiferi e le perdite in mare

![Schermata 2024-05-04 alle 16.53.01.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-04%20alle%2016.53.01.png)

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

- [?] In classe parlava di traslare le curve: non ho capito come, in che senso???

