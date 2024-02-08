---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/veicoli-e-impianti-di-trasporto/lezioni/08-motori-vit/"}
---


# [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT\|08 - Motori - VIT]]

# Motore endotermico

Esistono in generale 2 tipi di motori endotermici che sfruttano due diversi cicli:
- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT#Motore a Ciclo Otto\|#Motore a Ciclo Otto]] - Combustione comandata
- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT#Motore a Ciclo Diesel\|#Motore a Ciclo Diesel]] - Combustione spontanea

```ad-Definizione
title: Motore a combustione interna
Il **motore a combustione interna** o **motore endotermico** è un particolare motore termico nel quale avviene combustione tramite reazione tra un **carburante** (o **combustibile**: benzina, gasolio, metano, GPL, cherosene...) e un **comburente** (aria).
```


Possono essere classificati a seconda della modalità con cui la miscela viene apportata all'interno del motore:
- Motori **volumetrici** - il fluido motore agisce in maniera intermittente
	- Motori a movimento **alternativo dei pistoni**
		- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT#Motore a Ciclo Otto\|#Motore a Ciclo Otto]]
		- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT#Motore a Ciclo Diesel\|#Motore a Ciclo Diesel]]
	- Motori a movimento **rotativo del pistone**
		- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT#Motore Wankel\|#Motore Wankel]]
- Motori **continui** - il fluido motore agisce in maniera continua
	- Motori a moto **rotativo** rappresentati dalla **turbina a gas**

**Potenza effettiva** o **potenza meccanica**: La potenza disponibile sull'albero motore, detratte tutte le perdite

## Motore a Ciclo Otto

```ad-Definizione
title: Motore a Ciclo Otto o ad Accensione Comandata

Nei motori ad **accensione comandata** l'accensione è comandata attraverso una scintilla ad alta tensione che scocca nella miscela aria-combustibile all'interno del cilindro.
```

Si tratta di motori generalmente alimentati tramite un carburatore che provvede a formare la miscela di aria e di carburante nella proporzione opportuna: in generale contiene un eccesso di carburante rispetto alla quantità corrispondente al rapporto stechiometrico.

La regolazione della potenza avviene per mezzo di una valvola a farfalla che strozza il passaggio dell'aria. Si produce una perdita di carico che riduce la quantità di miscela aspirata dai pistoni nei cilindri.

In alcuni motori l'alimentazione avviene tramite iniezione tramite un iniettore nel condotto di aspirazione. Si ottiene una migliore formazione della miscela e quindi un rendimento maggiore.

La caratteristica meccanica è raffigurata nella figura sotto:

![Pasted image 20240207174106.png|650](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Pasted%20image%2020240207174106.png)

dove:
- $N=$ Potenza
- $C=$ Coppia
- $q=$ Consumo specifico
in funzione della velocità di rotazione del motore $n$.

Il motore a Ciclo Otto non è in grado di funzionare per valori di giri molto bassi né è capace di avviarsi da fermo in autonomia. Viene quindi portato a velocità di funzionamento tramite un **motorino di avviamento solitamente elettrico**.

Il consumo specifico è minimo in corrispondenza, più o meno, del valore di giri relativi alla coppia massima.

### Rendimento - Ciclo Otto

Il consumo specifico $q$ è la quantità di combustibile consumato in un'ora di funzionamento per unità di potenza resa. È anche il consumo orario di combustibile per li lavoro compiuto dalla potenza unitaria. Si può esprimere in \[massa/energia\].

- Sia $H_{i}$ il potere energetico inferiore del combustibile (energia potenziale contenuta nella massa unitaria di combustibile: \[energia/massa\]).
- Sia $N_{u}$ la potenza utile all'albero del motore erogata nel tempo $T$.
- Sia $n_{m}$ il rendimento meccanico del motore

Possiamo definire:
**COMBUSTIBILE CONSUMATO**
$$
qN_{u}T
$$
**ENERGIA TERMICA PRODOTTA**
$$
qH_{i}N_{u}T
$$
**ENERGIA MECCANICA PRODOTTA ALL'ALBERO** (energia)
$$
\eta_{m} \cdot qH_{i}N_{u}T
$$
**LAVORO UTILE PRODOTTO** (energia)
$$
N_{u}T
$$
Uguagliando le ultime due si ottiene
$$
\begin{align}
\eta_{m} \cdot qH_{i}N_{u}T = N_{u}T \\
\eta = \frac{1}{qH_{i}}
\end{align}
$$
Si trova, usando valori realistici di consumo e potere energetico, che il rendimento di un [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT#Motore a Ciclo Otto\|#Motore a Ciclo Otto]] si aggira intorno a valori
$$
\eta_{m} = 25\div 30 \%
$$


## Motore a Ciclo Diesel

```ad-Definizione
title: Motori a Ciclo Diesel o ad Accensione Spontanea
Nei motori ad **accensione spontanea** il combustibile è iniettato nell'aria compressa presente nei cilindri del motore e la combustione si innesca a causa delle condizioni di pressione e di temperatura dell'aria stessa.
```

Questi motori funzionano in realtà secondo un ciclo misto in cui la fase di combustione è in parte a **pressione costante** e in parte a **volume costante**.

La miscela si incendia per effetto della temperatura raggiunta durante la fase di compressione e brucia molto rapidamente.

Un motore Diesel presenta un ciclo a pressioni più elevate di un ciclo Otto di pari area. 

![Schermata 2024-02-08 alle 10.04.54.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-08%20alle%2010.04.54.png)

Sopra sono riportate le caratteristiche di potenza e coppia per il motore Diesel.

Si noti che la coppia è pressapoco costante col numero di giri in quanto è costante la quantità di combustibile immesso dalla pompa di iniezione in ogni fase di compressione.

La potenza invece, cresce linearmente (o quasi) con la velocità.

Al fine di realizzare caratteristiche stabili a regime però i costruttori tendono a rendere la curva di coppia più pendente.

Come i [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT#Motore a Ciclo Otto\|#Motore a Ciclo Otto]], anche quelli a Diesel hanno bisogno di un motorino di avviamento non essendo capaci di operare a bassi valori di giri.

Questi motori, rispetto a quelli a ciclo Otto, presentano rendimenti maggiori, nell'ordine di $35 \div 40\%$.

La potenza dei motori Diesel dipende dalla pressione, dalla temperatura e dall'unimidità dell'aria:
$$
N(p,p_{u}, t) = N_{0} \frac{p-p_{u}}{p_{0}-p_{u_{0}}}\cdot\frac{273+t_{0}}{273+t}
$$
dove:
- $p, p_{0}$ - Pressioni dell'aria
- $p_{u}, p_{u_{0}}$ - Pressioni parziali del vapor d'acqua corrispondenti alle temperature $t,t_{0}$

Il rendimento del motore Diesel si riduce al ridursi della coppia.

## Organi di trasmissione

### La funzione della trasmissione per i veicoli terrestri

I motori usati per la trazione sono motori rotanti. Forniscono all'albero una velocità di rotazione $\omega$ una coppia motrice $M$. La **potenza di rotazione** è pertanto $P_{\rm rotazione} = M\omega$.

Per far avanzare un veicolo occorre però una forza $F$, capace di portare il veicolo a una velocità $V$. La **potenza di traslazione** sarà pertanto $P_{\rm traslazione} = FV$.

È chiaro che occorre avere a disposizione un organo in grado di trasformare una potenza di rotazione in una di traslazione. Questo strumento è la ruota.

Si noti inoltre che il più delle volte l'asse dell'albero motore non coincide con l'asse di rotazione delle ruote. Sarà necessario interporre degli elementi in grado di "girare" la coppia fornita dal motore.

Si guarda ora invece alla velocità di rotazione delle ruote.
La velocità del veicolo infatti è data da
$$
V = \omega\frac{D}{2} = \frac{2\pi n}{60} \frac{D}{2}
$$
È chiaro quindi che, per ruote di diametro $1 \, \rm m$, per un veicolo che viaggi a $100 \, \rm \frac{km}{h}$, la velocità di rotazione delle ruote sarà $531 \, \rm rpm$. I motori, come abbiamo visto, lavorano al meglio per valori di $2000\div 3000 \,\rm rpm$. Si potrebbero costruire motori capaci di operare allo stesso numero di giri delle ruote ma dovrebbero essere estremamente più grandi e ingombranti. 
Sarà per forza di cose necessario interporre, tra il motore e le ruote degli organi capaci di variare il rapporto di trasmissione.

Il rapporto di trasmissione, al di là del cambio (che vedremo in seguito) è fisso, è detto **rapporto di trasmissione al ponte** e di solito vale 5.

❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗❗




<iframe width="560" height="315" src="https://www.youtube.com/embed/yYAw79386WI?si=TGTK-dsp5Ooua0b_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/XBjVYCD0RyQ?si=ea-L5yhnkuM1UF4h" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Pietrarsa (NA)
