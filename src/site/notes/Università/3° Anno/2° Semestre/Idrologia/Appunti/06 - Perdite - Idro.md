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
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Intercettazione della vegetazione\|#Intercettazione della vegetazione]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Invaso nelle depressioni\|#Invaso nelle depressioni]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Infiltrazione nel suolo\|#Infiltrazione nel suolo]]

```

### Pioggia netta

La pioggia netta è la differenza tra la pioggia e le [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Perdite idrogeologiche\|#Perdite idrogeologiche]]:
$$
p(t) = i(t) - e(t) - v(t)- s(t) - f(t)
$$
dove:
- $p(t):$ Pioggia lorda
- $i(t):$ [[Università/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Intensità istantanea di pioggia\|Intensità istantanea di pioggia]]
- $e(t):$ Intensità di [[#Evapotraspirazione]]
- $\nu(t):$ Intensità di [[#Intercettazione della vegetazione]]
- $s(t):$ Intensità di [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Invaso nelle depressioni\|#Invaso nelle depressioni]]
- $f(t):$ Intensità di [[#Infiltrazione nel suolo]]

In realtà alcuni di questi termini possono essere trascurati:
$$
p(t) = i(t) - \cancel{e(t)} - \cancel{v(t)} - \cancel{s(t)} - f(t)
$$
in particolare quando piove e se considero una scala annuale.
$$
p(t) = i(t) - f(t)
$$

## Evapotraspirazione

Si tratta dell'unione di due fenomeni: evaporazione e traspirazione.

### Evaporazione

L'evaporazione è un fatto statistico. 

#### Intensità di evaporazione

L'intensità di evaporazione è pari alla differenza del flusso volumetrico d'acqua che passa allo stato di vapore e quello dell'acqua che passa allo stato liquido.

Dobbiamo infatti immaginare che allo stesso tempo ci saranno delle molecole che, dotate di un'**energia cinetica particolarmente elevata** passano allo stato di vapore e allo stesso tempo delle molecole di vapore che, **urtando la superficie libera del liquido**, lo penetrano.

Questi due flussi sono uguali quando l'aria è **satura**: in questo caso non c'è [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evaporazione\|#Evaporazione]].

#### Altezza di evaporazione

L'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evaporazione\|#Evaporazione]] si misura in termini di altezza di evaporazione:

```ad-Definizione
title: Altezza di evaporazione ($E$)

L'**altezza di evaporazione** in un intervallo di tempo $\Delta t$ è il rapporto tra il volume d'acqua evaporato e l'area della superficie evaporante:
$$
E = \frac{W_{e}}{A}
$$
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

L'**evapotraspirazione** è qiundi la somma dei contributi di [[#Evaporazione]] e [[#Traspirazione]].

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

$$
\text{evapotraspirazione}  = \text{pioggia} - \text{acqua drenata} - \text{variazione di umidità nel terreno}
$$

```



```ad-note
title: Osservazione
L'[[#Evapotraspirazione]] è un fenomeno influenzato dal vento. 

Infatti, in presenza di vento vi è un continuo ricambio d'aria al di sopra della superficie evapotraspirante. 

Senza vento di contro, l'aria arriva a saturazione impedendo il processo.

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

#### Formula di Thorntwaite

La **Formula di Thorntwaite** è usata per conteggiare l'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione potenziale\|#Evapotraspirazione potenziale]] mensile:
$$
E_{p,j} = 16 a_{j} \left( \frac{10}{I}T_{j} \right)^{\alpha}
$$
dove:
- $a_{j}:$ frazione di ore diurne
- $T_{j}:$ temperatura media
- $I= \sum\limits_{j=1}^{12}\left[0.09 \cdot T_{j}^{1.5} \right]$
- $\alpha = \dfrac{1.6}{100}I + 0.5$

#### Equazione di Penman-Monteith

L'**equazione di Penman-Monteith** è un'equazione teorica ricavata da:
- Bilancio energetico della superficie
- Aerodinamica del trasferimento del vapore

![Schermata 2024-05-04 alle 20.18.28.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-04%20alle%2020.18.28.png)

#### Formula di Turc

La **Formula di Turc** permette il conteggio dell'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione effettiva\|#Evapotraspirazione effettiva]] annua:
$$
E = \dfrac{h}{\sqrt{0.9+ \left( \dfrac{h}{L} \right)^{2}}}
$$
dove:
- $L= 300 + 25\cdot T + 0.05 \cdot T^{3}$
- $E:$ Altezza annua dell'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evapotraspirazione effettiva\|#Evapotraspirazione effettiva]] $[\rm mm]$
- $h:$ [[Università/3° Anno/2° Semestre/Idrologia/Appunti/02 - Piogge Intense - Idro#Altezza di pioggia\|Altezza di precipitazione]] $[\rm mm]$

## Intercettazione della vegetazione

```ad-Definizione
title: Intensità dell'intercettazione ($\nu(t)$)

$$
\nu(t) = i(t) e^{-\dfrac{h(t)}{V_{MAX}}} \quad \rm \left[ \frac{mm}{h} \right]
$$

```


## Invaso nelle depressioni

```ad-Definizione
title: Invaso delle depressioni

L'**invaso delle depressioni** è costituito dal volume d'acqua che si accumula nelle depressioni del terreno e non defluisce, ma dopo l'evento evapora o s'infiltra gradualmente.

```

### Intensità d'invaso

L'[[#Invaso nelle depressioni]] si misura in termini di **intensità di invaso**

```ad-Definizione
title: Intensità d'invaso ($s(t)$)
L'**intensità d'invaso** è dato dalla seguente:
$$
s(t) = \left[ i(t) - \nu(t) - f(t) \right] e^{- \dfrac{h(t) - V(t)-F(t)}{S_{MAX}}}
$$
```



## Infiltrazione nel suolo

