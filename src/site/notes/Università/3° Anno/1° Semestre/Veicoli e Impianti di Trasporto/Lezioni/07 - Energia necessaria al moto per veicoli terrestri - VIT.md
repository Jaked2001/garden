---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/veicoli-e-impianti-di-trasporto/lezioni/07-energia-necessaria-al-moto-per-veicoli-terrestri-vit/"}
---

# [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/07 - Energia necessaria al moto per veicoli terrestri - VIT\|07 - Energia necessaria al moto per veicoli terrestri - VIT]]




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/3-anno/1-semestre/tecnica-ed-economia-dei-trasporti/appunti/04-diagramma-elementare-del-moto-e-prestazioni-del-veicolo-isolato/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">





Altri libri di riferimento:
- Ingegneria dei sistemi ferroviari - tecnologie metodi ed applicazioni, egaf
- Orlandi Alessandro, Meccanica dei trasporti, ???
- Leuzzi V., Fondamenti di trasporti - Appunti delle lezioni, facoltà di ingegneria di Roma
- Scarponi P., Malavasi G., Fondamenti di trasporti - Applicazioni, Facoltà di Ingegneria di Roma



# Diagramma Elementare del Moto

Forze sul veicolo in movimento
- [Forze motrici]
- [Forze Frenanti]
- [[Università/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/03. Sostentazione e locomozione#Resistenze ordinarie\|Resistenze ordinarie]]
- [[Università/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/03. Sostentazione e locomozione#Resistenze Addizionali\|Resistenze addizionali]]

## Fasi di sosta

Si hanno quando
$
\begin{cases}
v = 0 \\
T- R = 0
\end{cases}
$
## Fasi di movimento

![Schermata 2024-02-08 alle 10.53.29.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Tecnica%20ed%20Economia%20dei%20Trasporti/Appunti/allegati/Schermata%202024-02-08%20alle%2010.53.29.png)

Si hanno quando 
$
v \ne 0
$
Possono quindi verificarsi 4 casi:
$
\begin{cases}
T - R = 0 &\quad v = \rm cost \\
T - R < 0 &\quad v \searrow  \\
T - R > 0 &\quad v \nearrow \\
R > 0, T = 0 &\quad \rm Deriva
\end{cases}
$
L'obiettivo è quello di risolvere l'[[Università/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/03. Sostentazione e locomozione#Equazione generale del moto\|equazione generale del moto]]:
$
T(v) - R(v) - R(s) = m_{e}a = m_{e}\frac{dv}{dt}
$
dove:
- $v, a =$ Velocità e Accelerazione
- $T(v) =$ Sforzo di trazione
- $R(v) =$ Resistenze ordinarie (rotolamento e aerodinamica)
- $R(s) =$ Resistenze addizionali (livelletta e curva)
- $m_{e} =$ Massa equivalente (che tiene conto di tutte le inerzie)
- $\delta =$ Coefficiente di maggiorazione delle masse rotanti
$
m_{e} = m_{\rm tara} (1 + \delta) + m_{\rm carico} \approx m (1+\delta)
$





```ad-question
- Perché dalla slide 92 non c'è più $R(s)$ ma poi ricompare nella 96??
	- Formule prese da fonti diverse con diverse approx. Dovrebbe esserci semrpe.
- Nella slide 96, la trazione e la resistenza sono calcolate in $v_{m}$? Se no, come posso levarle dall'integrale?????????
	- Esatto

```


## Soluzione dell'equazione generale del moto

Per conoscere il moto di un veicolo dobbiamo risolvere l'[[Università/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/03. Sostentazione e locomozione#Equazione generale del moto\|equazione generale del moto]]. Per farlo la riscriviamo nella forma:
$
\frac{T(v) - R(v) - R(s)}{m_{e}}= \frac{dv}{dt}
$
che si può risolvere per separazione di variabili:
$
{dt}= m_{e} \frac{dv}{T(v) - R(v) - R(s)}
$
Questa andrebbe quindi integrata analiticamente restituendoci la funzione $v(t)$.
In realtà è di nostro interesse conoscere la funzione $s(t)$ quindi, tenendo a mente la relazione
$
v dt = ds \Longrightarrow dt = \frac{ds}{v}
$
possiamo riscrivere
$
ds = m_{e} \frac{vdv}{T(v) - R(v) - R(s)}
$
Poiché però le resistenze e la trazione dipendono dalla velocità e di solito non conosciamo analiticamente questa dipendenza, dovremo fare uso di alcuni metodi numerici per risolvere l'equazione non analiticamente ma sfruttando metodi di risoluzione alle differenze finite.
Potremmo principalmente adoperare 3 metodi distinti:
- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/07 - Energia necessaria al moto per veicoli terrestri - VIT#Metodo $ Delta v$\|#Metodo $ Delta v$]]
- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/07 - Energia necessaria al moto per veicoli terrestri - VIT#Metodo $ Delta s$\|#Metodo $ Delta s$]]
- [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/07 - Energia necessaria al moto per veicoli terrestri - VIT#Metodo $ Delta t$\|#Metodo $ Delta t$]]

È infatti noto il diagramma $T-R$ su $V$:

![Caratteristica meccanica e resistenza al moto - 04. Diagramma Elementare del Moto e Prestazioni del Veicolo Isolato 2023-10-22 19.46.55.excalidraw.png](/img/user/Excalidraw/Caratteristica%20meccanica%20e%20resistenza%20al%20moto%20-%2004.%20Diagramma%20Elementare%20del%20Moto%20e%20Prestazioni%20del%20Veicolo%20Isolato%202023-10-22%2019.46.55.excalidraw.png)


### Metodo $\Delta v$

Consiste nel partire da intervalli finiti di velocità.
Si scelgono $\Delta v$ abbastanza piccoli in modo che tra $v_{i}$ e $v_{f}$ non vi siano variazioni troppo marcate della grandezza $T(v)-R(v)$.
Si hanno quindi le seguenti grandezze:
$
\begin{cases}
v_i \\
v_{f} = v_{i}+ \Delta v \\
v_{m} = v_{i} + \frac{1}{2} \Delta v
\end{cases}
$
Possiamo quindi ricavare il valore medio dell'accelerazione nell'intervallo 
$
\frac{\Delta v}{\Delta t} = a_{m} = \frac{T(v_{m})- R(v_{m})-R(s_{m})}{m(1+\delta)}
$
Una volta ricavata la $a_{m}$ si può facilmente trovare l'intervallo di tempo corrispondente:
$
\Delta t = \frac{{\Delta v}}{3.6 \cdot a_{m} }
$
dove il fattore $3.6$ è aggiunto per convertire da ore a secondi (Essendo la velocità espressa in $\rm \frac{km}{h}$)
Si ricava quindi anche lo spazio percorso nell'intervallo di tempo considerato:
$
\Delta s = \frac{v_{m} \Delta t}{3.6}
$

```ad-attention
title: Attenzione
Facendo questa operazione si sta considerando la velocità costante e pari a $v_m$ in ogni intervallo.

Siccome ho già supposto che l'accelerazione sia costante quando ho calcolato l'intervallo di tempo, posso pensare di trovare l'intervallo spaziale in un modo alternativo per ridurre gli errori commessi.
A partire dall'equazione generale del moto posso scrivere
$
\begin{align}
\int \Delta s &=  \frac{m_{e}}{T(v_{m})-R(v_{m})-R(s_{m})} \int_{v_{i}}^{v_{f}} \Delta v \\
\Delta s &= \frac{ m_{e}}{T(v_{m})-R(v_{m})-R(s_{m})} \frac{v_{f}^{2}-v_{i}^{2}}{2 \cdot 3.6^{2}}
\end{align}
$

```


Il procedimento si ripete andando via via avanti nel moto. Nel farlo, dobbiamo confrontare i risultati con il percorso che si suppone noto. Se un intervallo finisse per scavallare punti di rilievo (come cambio di pendenze, curve...) occorrerebbe ridurre gli intervalli in modo da ovviare a questo problema.

### Metodo $\Delta s$

Per ovviare al fatto che nel [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/07 - Energia necessaria al moto per veicoli terrestri - VIT#Metodo $ Delta v$\|#Metodo $ Delta v$]] occorra ricalibrare gli intervalli in modo da evitare le variazioni di condizioni che si verificano lungo il tracciato, posso pensare di [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/07 - Energia necessaria al moto per veicoli terrestri - VIT#Soluzione dell'equazione generale del moto\|risolvere l'equazione generale del moto]] a partire proprio dai $\Delta s$.
$
\begin{cases}
s_{i} \\
s_{f} = s_{i} + \Delta s \\
\end{cases}
$
Comincio con il trovare l'accelerazione iniziale da:
$
a_{i}= \frac{T(v_{i})-R(v_{i})}{m(1+\delta)}
$

È evidente che il metodo non è applicabile se parto con velocità iniziale nulla!!
otterrei infatti:
$
\Delta t(1) = \frac{3.6\Delta s}{v_{i}}
$
che non posso calcolare se $v_{i} = 0$.


### Metodo $\Delta t$


## Rappresentazione del moto del veicolo isolato

![Schermata 2023-10-22 alle 20.15.43.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Tecnica%20ed%20Economia%20dei%20Trasporti/Appunti/allegati/Schermata%202023-10-22%20alle%2020.15.43.png)


</div></div>


## Curve caratteristiche dei motori

```ad-Definizione
title: Curve caratteristiche dei motori

Le **curve caratteristiche dei motori** sono le curve che rappresentano l'andamento di
- Potenza
- Coppia
- Consumo specifico
in funzione della *velocità di rotazione*

```

La caratteristica meccanica del motore si lega alla [[Università/3° Anno/1° Semestre/Tecnica ed Economia dei Trasporti/Appunti/03. Sostentazione e locomozione#Caratteristica meccanica di trazione\|caratteristica meccanica di trazione]], attraverso i sistemi di trasmissione.

La velocità del veicolo è
$$
V = \frac{2\pi n_{w}}{60} r_{w}
$$
essendo
- "$w$" wheel (=ruota)

Sono necessari il **rapporto di trasmissione** $\gamma$ per cui (con "$e$" = engine)
$$
n_{w} = \frac{n_{e}}{\gamma}
$$
La velocità assume quindi la seguente espressione
$$
V = \frac{2\pi n_{e}}{60 \gamma} r_{w}
$$
La potenza erogata dal motore è trasmessa alle ruote solo in parte, a seconda del **rendimento** della trasmissione, $\eta$
$$
FV = \eta C \frac{2\pi n_{e}}{60}
$$
dove $C$ è la coppia.

 A questo punto, sostituendo $V$ e isolando $F$, la forza di trazione è data da
 $$
F = \eta\frac{C\gamma}{r_{w}}
$$

### Caratteristica di trazione ideale

La caratteristica di trazione ideale è quella che consente il **pieno sfruttamento della potenza erogata dal motore**. Dovrebbe avere quindi l'andamento di un'iperbole equilatera in quanto, in questo caso, si avrebbe costante il prodotto $P = FV$.

![Schermata 2024-02-08 alle 11.08.51.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-08%20alle%2011.08.51.png)

In realtà non esistono motori con questa caratteristica di trazione a potenza costante. Al più, il [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/10 - Motori ed equipaggiamenti per la trazione elettrica - VIT#Motore in Corrente Continua\|motore in CC]] si avvicina abbastanza a questa condizione.

Per ovviare a questo problema gli organi di regolazione cercano di approssimare per punti la caratteristica ideale generando una **caratteristica artificiale** variando con continuità le variabili di esercizio del motore.

### Caratteristica di trazione artificiale

Nei [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/08 - Motori - VIT\|motori endotermici]] la [[Università/3° Anno/1° Semestre/Veicoli e Impianti di Trasporto/Lezioni/07 - Energia necessaria al moto per veicoli terrestri - VIT#Caratteristica di trazione ideale\|#Caratteristica di trazione ideale]] è ottenuta mediante l'utilizzo del **cambio di velocità**, il quale consente di modificare il rapporto di riduzione tra il motore e le ruote.

In figura, è riportato l'andamento di una caratteristica di trazione per un veicolo con cambio a 4 marce:

![Schermata 2024-02-08 alle 11.14.33.png|650](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Veicoli%20e%20Impianti%20di%20Trasporto/Lezioni/allegati/Schermata%202024-02-08%20alle%2011.14.33.png)

### Stabilità della caratteristica di trazione


I tratti decrescenti della caratteristica di coppia o di forza di trazione sono stabili.

Se c'è un aumento di velocità, alla fine della perturbazione il sistema torna alla precedente condizione di equilibrio autonomamente. 


