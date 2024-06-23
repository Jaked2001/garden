---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/elettrotecnica/appunti/07-proprieta-generali-delle-reti-elettriche-et/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET\|07 - Proprietà generali delle reti elettriche - ET]]

## Risolvere una rete


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/3-anno/2-semestre/elettrotecnica/appunti/03-introduzione-allo-studio-delle-reti-elettriche-et/#rete-elettrica" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Rete elettrica

```ad-Definizione
title: Rete elettrica

Una **rete elettrica** o **circuito elettrico** costituisce il modello semplificato di un qualsiasi sistema in cui avvengono fenomeni di tipo elettrico.

```

Ci sono delle ipotesi alla base delle reti elettriche:

```ad-hint
title: Ipotesi di una rete elettrica

- Lungo i conduttori, la carica elettrica si muove liberamente e i conduttori sono equipotenziali
- Lo spazio all'esterno dei bipoli (o n-poli) e dei conduttori è isolante
- All'esterno dei bipoli (o n-poli) il campo elettrico è conservativo
- All'esterno dei bipoli (o n-poli) non vi è accumulo di carica
```


</div></div>


```ad-Definizione
title: Risolvere una rete

**Risolvere una [[03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica|rete elettrica]]** significa determinare le tensioni e le correnti su tutti i [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipoli]].

```

## Topologia delle reti elettriche

```ad-Definizione
title: Topologia delle reti elettriche

La **topologia delle [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica\|reti elettriche]]** è la descrizione delle interconnessioni esistenti tra i bipoli della rete

```

![07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.02.47.excalidraw.png](/img/user/Excalidraw/07%20-%20Propriet%C3%A0%20generali%20delle%20reti%20elettriche%20-%20ET%202024-06-15%2013.02.47.excalidraw.png)


### Lato

```ad-Definizione
title: Lato ($l$)

![07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.08.39.excalidraw.png](/img/user/Excalidraw/07%20-%20Propriet%C3%A0%20generali%20delle%20reti%20elettriche%20-%20ET%202024-06-15%2013.08.39.excalidraw.png)
%%[[07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.08.39.excalidraw.md|🖋 Edit in Excalidraw]]%%

Un **lato** è un tratto di rete che rappresenta un [[03 - Introduzione allo studio delle reti elettriche - ET#Bipolo|bipolo]] con i conduttori ideali direttamente collegati ai suoi terminali.
```

- $l:$ Il numero di **lati** di una rete

### Nodo

```ad-Definizione
title: Nodo ($n$)

![07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.10.02.excalidraw.png](/img/user/Excalidraw/07%20-%20Propriet%C3%A0%20generali%20delle%20reti%20elettriche%20-%20ET%202024-06-15%2013.10.02.excalidraw.png)
%%[[07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.10.02.excalidraw.md|🖋 Edit in Excalidraw]]%%

Un **nodo** è un punto di interconnessione di almeno 3 [[#Lato|lati]].

```

- $n:$ Il numero di **nodi** di una rete
### Grafo

```ad-Definizione
title: Grafo

![07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.11.18.excalidraw.png](/img/user/Excalidraw/07%20-%20Propriet%C3%A0%20generali%20delle%20reti%20elettriche%20-%20ET%202024-06-15%2013.11.18.excalidraw.png)
%%[[07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.11.18.excalidraw.md|🖋 Edit in Excalidraw]]%%

Il **grafo** è una descrizione grafica della rete, ottenuta indicando i [[#Nodo|nodi]] per mezzo di punti e i [[#Lato|lati]] per mezzo di segmenti curvilinei.


```

Si parla di **grafo piano** quando tutta la rete può essere rappresentata senza che ci siano sovrapposizioni di lati.

### Maglia


```ad-Definizione
title: Maglia

![07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.13.20.excalidraw.png](/img/user/Excalidraw/07%20-%20Propriet%C3%A0%20generali%20delle%20reti%20elettriche%20-%20ET%202024-06-15%2013.13.20.excalidraw.png)
%%[[07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.13.20.excalidraw.md|🖋 Edit in Excalidraw]]%%

Una maglia è un insieme di [[#Lato|lati]] tali da costruire un percorso chiuso nel [[#Grafo]] che tocca ciascun [[#Nodo]] una sola volta.

```


### Albero

```ad-Definizione
title: Albero

![Schermata 2024-06-15 alle 16.45.13.png|450](/img/user/Schermata%202024-06-15%20alle%2016.45.13.png)

Un **albero** è un insieme di [[#Lato|lati]] che collegano tutti i [[#Nodo|nodi]] del [[#Grafo]] senza formare alcuna [[#Maglia]].

In un grafo si possono definire più alberi.


```

### Coalbero


```ad-Definizione
title: Albero

![Schermata 2024-06-15 alle 16.58.47.png|450](/img/user/Schermata%202024-06-15%20alle%2016.58.47.png)

Un **coalbero** è l'insieme di [[#Lato|lati]] complementari ad un dato [[#Albero]].

Si possono definire tanti coalberi quanti sono gli alberi

```


## Leggi di Kirchhoff

A partire dalle proprietà dei campi vettoriali per tensioni e correnti valgono alcune leggi fondamentali alla base dello studio delle [[03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica|reti elettriche]]:


### Legge di Kirchhoff delle Correnti (LKC)


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/legge-di-kirchhoff-delle-correnti-lkt/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

<div class="markdown-embed-title">

# LKT

</div>



# [[Legge di Kirchhoff delle Correnti (LKT)\|Legge di Kirchhoff delle Correnti (LKT)]]

```ad-Teo
title: Legge id Kirchhoff delle Correnti (LKC)

La **Legge di Kirchhoff delle Correnti (LKC)** dice che, in una rete di $n$-poli, la somma algebrica delle correnti dei [[#Lato|lati]] appartenenti ad un qualsiasi insieme di taglio orientato è uguale a zero in ogni istante:
$
\sum i(t) = 0
$

Vale anche in forma simbolica:
$
\sum\limits \overline{I} = 0
$
```

![07 - Proprietà generali delle reti elettriche - ET 2024-06-15 17.30.32.excalidraw.png](/img/user/Excalidraw/07%20-%20Propriet%C3%A0%20generali%20delle%20reti%20elettriche%20-%20ET%202024-06-15%2017.30.32.excalidraw.png)






</div></div>

### Legge di Kirchhoff delle Tensioni (LKT)


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/legge-di-kirchhoff-delle-tensioni-lkt/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">

<div class="markdown-embed-title">

# LKT

</div>



# [[Legge di Kirchhoff delle Tensioni (LKT)\|Legge di Kirchhoff delle Tensioni (LKT)]]


```ad-Teo
title: Legge di Kirchhoff delle Tensioni (LKT)

La **Legge di Kirchhoff delle Tensioni (LKT)** afferma che, in una rete di $n$-poli, la somma algebrica delle tensioni dei lati appartenenti ad una qualsiasi maglia orientata è uguale a zero in ogni istante:
$
\sum v(t) = 0
$
Vale anche in forma simbolica:
$
\sum\limits \overline{V} = 0
$
```

![07 - Proprietà generali delle reti elettriche - ET 2024-06-15 17.35.34.excalidraw.png](/img/user/Excalidraw/07%20-%20Propriet%C3%A0%20generali%20delle%20reti%20elettriche%20-%20ET%202024-06-15%2017.35.34.excalidraw.png)


</div></div>

## Sistemi di equazioni topologiche

Le equazioni di [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Legge di Kirchhoff delle Correnti (LKC)\|#Legge di Kirchhoff delle Correnti (LKC)]] e [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Legge di Kirchhoff delle Tensioni (LKT)\|#Legge di Kirchhoff delle Tensioni (LKT)]] sono dette **equazioni topologiche della rete**. 

Per [[Università/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete\|#Risolvere una rete]] è necessario risolvere il sistema costituito da tutte le equazioni topologiche indipendenti.

In particolare ci saranno, in una rete di $n$ nodi e $l$ lati:
- $p := n-1:$ LKC indipendenti
- $m := l-p:$ LKT indipendenti (maglie indipendenti)


Un sistema di equazioni indipendenti sarà pertanto costituito da $p$ equazioni ai nodi (LKC) e $m$ equazioni alle maglie (LCT)

