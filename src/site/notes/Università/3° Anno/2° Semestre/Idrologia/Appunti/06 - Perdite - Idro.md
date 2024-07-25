---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/idrologia/appunti/06-perdite-idro/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro\|06 - Perdite - Idro]]

# Perdite idrogeologiche

```ad-Definizione
title: Perdite idrogeologiche

Le **perdite idrogeologiche** sono l'insieme dei volumi di portata che entra nel bacino e si perde durante il [[05 - Deflussi - Idro|Deflusso]] senza mai raggiungere la sezione finale.

Costituiscono perdita idrogeologica:
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione\|#Evapotraspirazione]]
- [[#Intercettazione della vegetazione]]
- [[#Invaso nelle depressioni]]
- [[07b - Infiltrazione - Idro|Infiltrazione nel suolo]]

```

Il calcolo delle perdite idrologiche ci permette di sapere qual è la quotaparte di pioggia che raggiunge la sezione finale.

### Pioggia netta

```ad-Definizione
title: Pioggia netta

La **pioggia netta** è la differenza tra la pioggia e le [[#Perdite idrogeologiche]]:
$
p(t) = i(t) - e(t) - v(t)- s(t) - f(t)
$
dove:
- $p(t):$ [[02 - Piogge Intense - Idro#Intensità di pioggia|intensità di pioggia]] netta
- $i(t):$ [[02 - Piogge Intense - Idro#Intensità istantanea di pioggia|Intensità di pioggia]] lorda
- $e(t):$ Intensità di [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione\|#Evapotraspirazione]]
- $\nu(t):$ Intensità di [[#Intercettazione della vegetazione]]
- $s(t):$ Intensità di [[#Invaso nelle depressioni]]
- $f(t):$ Intensità di [[07b - Infiltrazione - Idro|Infiltrazione]]

```


In realtà alcuni di questi termini possono essere trascurati:
$$
p(t) = i(t) - \cancel{e(t)} - \cancel{v(t)} - s(t) - f(t)
$$
Elimino:
- Su scala annuale: trascuro $v(t)$
- Negli eventi di piena: trascuro $e(t)$

In particolare quando piove e se considero una scala annuale.
$$
p(t) = i(t) - s(t) - f(t)
$$


## Evapotraspirazione

Si tratta dell'unione di due fenomeni:
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evaporazione\|#Evaporazione]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Traspirazione\|#Traspirazione]]

### Evaporazione

L'evaporazione è un fatto statistico. 

#### Intensità di evaporazione

```ad-Definizione
title: Intensità di evaporazione

L'**intensità di evaporazione** è pari alla differenza del flusso volumetrico d'acqua che passa allo stato di vapore e quello dell'acqua che passa allo stato liquido.

```


Dobbiamo infatti immaginare che allo stesso tempo ci saranno delle molecole che, dotate di un'**energia cinetica particolarmente elevata** passano allo stato di vapore e allo stesso tempo delle molecole di vapore che, **urtando la superficie libera del liquido**, lo penetrano.

Questi due flussi sono uguali quando l'aria è **satura**: in questo caso non c'è [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evaporazione\|#Evaporazione]].

#### Altezza di evaporazione

L'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evaporazione\|#Evaporazione]] si misura in termini di altezza di evaporazione:

```ad-Definizione
title: Altezza di evaporazione ($E$)

L'**altezza di evaporazione** in un intervallo di tempo $\Delta t$ è il rapporto tra il volume d'acqua evaporato e l'area della superficie evaporante:
$
E = \frac{W_{e}}{A}
$
dove:
- $W_{e}:$ Volume d'acqua evaporato
- $A:$ Area della superficie evaporante

```

Si misura per mezzo dell'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evaporimetro\|#Evaporimetro]]

L'evaporazione dipende da:
- Irraggiamento netto sulla superficie
- Stato dell'atmosfera
	- Umidità
	- Pressione
	- Temperatura
- Natura della superficie evaporante
	- Terreno nudo o con vegetazione
	- Specchio d'acqua


##### Evaporimetro

L'evaporimetro è lo strumento di misura dell'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Altezza di evaporazione\|#Altezza di evaporazione]].

Quest'ultima è data dalla diminuzione dell'altezza d'acqua negli apparecchi, cui va sommata l'altezza di precipitazione misurata da un pluviometro ad essi affiancato.

![Schermata 2024-05-04 alle 18.39.58.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-04%20alle%2018.39.58.png)

##### Formula di Conti (evaporazione laghi)

Nei casi dei laghi si adopera la Formula di Conti:
$$
E_{j} = k_{j}T_{j} \frac{p_{n}}{p_{j}}
$$
dove:
- $E_{j}:$ [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Altezza di evaporazione\|#Altezza di evaporazione]] nel mese $j-$esimo
- $T_{j}:$ Temperatura media nel mese $j-$esimo (in $\degree \rm C$)
- $p_{n}:$ Pressione normale al livello del mare
- $p_{j}:$ Pressione atmosferica media del mese $j-$esimo
- $k_{j}:$ Coefficiente sperimentale che dipende dal mese che si considera:

La formula di Conti è una legge empirica che fornisce l'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evaporazione\|#Evaporazione]] in un mese.

In Italia evapora $1 \,\rm cm$ al giorno d'acqua dai laghi.

| Mese      | $k_j$ |
| --------- | ----- |
| Gennaio   | 4.4   |
| Febbraio  | 4.5   |
| Marzo     | 5.3   |
| Aprile    | 6     |
| Maggio    | 7.5   |
| Giugno    | 6.4   |
| Luglio    | 6.3   |
| Agosto    | 5.9   |
| Settembre | 5.9   |
| Ottobre   | 5.8   |
| Novembre  | 4.7   |
| Dicembre  | 3.8   |

### Traspirazione

La traspirazione conteggia l'acqua evaporata dalle piante.

Si tratta dell'acqua usata per:
- Nuova materia organica
- Trasporto dei nutrienti
- Regolazione della temperatura

### Evapotraspirazione (Evaporazione + Traspirazione)

```ad-Definizione
title: Evapotraspirazione

L'**evapotraspirazione** è quindi la somma dei contributi di [[#Evaporazione]] e [[#Traspirazione]].

```

Distinguiamo tra
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione potenziale\|#Evapotraspirazione potenziale]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione effettiva\|#Evapotraspirazione effettiva]]



#### Evapotraspirazione potenziale

```ad-Definizione
title: Evapotraspirazione potenziale

L'**evapotraspirazione potenziale** è l'altezza di [[#Evapotraspirazione]] che si verificherebbe nel periodo considerato se la *disponibilità idrica fosse talmente elevata da non costituire un fattore limitante*

```


#### Evapotraspirazione effettiva

```ad-Definizione
title: Evapotraspirazione effettiva

L'**evapotraspirazione effettiva** è l'altezza di [[#Evapotraspirazione]] che si verifica nel periodo considerato, limitata da
- condizioni metereologiche
- disponibilità idrica
- stato della vegetazione

$
\text{evapotraspirazione}  = \text{pioggia} - \text{acqua drenata} - \text{variazione di umidità nel terreno}
$

```

.

```ad-note
title: Osservazione
L'[[#Evapotraspirazione]] è un fenomeno influenzato dal vento. 

Infatti, in presenza di vento vi è un continuo ricambio d'aria al di sopra della superficie evapotraspirante. 

Senza vento, di contro, l'aria arriva a saturazione impedendo il processo.

```


#### Misura dell'evapotraspirazione

##### Lisimetro

```ad-Definizione
title: Lisimetro

Il **lisimetro** è lo strumento adibito alla misura dell'[[#Evapotraspirazione]].

```

![Schermata 2024-05-04 alle 20.12.36.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-04%20alle%2020.12.36.png)

- Lisimetro ordinario
- Lisimetro a livello idrico costante

### Formule di evapotraspirazione

Esistono varie formule per descrivere l'[[#Evapotraspirazione]]

#### Formula di Thorntwaite

La **Formula di Thorntwaite** è usata per conteggiare l'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione potenziale\|#Evapotraspirazione potenziale]] mensile:
Lega l'[[#Evapotraspirazione]] a:
- Temperatura
- Irraggiamento diurno

#### Equazione di Penman-Monteith

L'**equazione di Penman-Monteith** è un'equazione teorica ricavata da:
- Bilancio energetico della superficie
- Aerodinamica del trasferimento del vapore

![Schermata 2024-05-04 alle 20.18.28.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-04%20alle%2020.18.28.png)

#### Formula di Turc

La **Formula di Turc** permette il conteggio dell'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione effettiva\|#Evapotraspirazione effettiva]] annua.


## Intercettazione della vegetazione

Intercettazione della vegetazione è il volume d'acqua che cade sulla vegetazione formando un velo idrico il quale successivamente evapora.
- Per fenomeni di modesta intensità e intermittenti, le perdite per intercettazione sono consistenti
- Per un singolo evento di piena le perdite per intercettazioni sono modeste.

![Schermata 2024-07-14 alle 18.16.56.png](/img/user/Schermata%202024-07-14%20alle%2018.16.56.png)

- $v(t):$ Intensità di intercettazione
- $V(t):$ Volume d'acqua accumulato dalle piante

## Invaso nelle depressioni

```ad-Definizione
title: Invaso delle depressioni

L'**invaso delle depressioni** è costituito dal volume d'acqua che si accumula nelle depressioni del terreno e non defluisce, ma dopo l'evento evapora o s'infiltra gradualmente.

```

