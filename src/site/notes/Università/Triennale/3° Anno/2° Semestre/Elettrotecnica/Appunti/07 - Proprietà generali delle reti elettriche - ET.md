---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/07-proprieta-generali-delle-reti-elettriche-et/","tags":["UNI"],"dg-note-properties":{"aliases":["7 - Proprietà generali delle reti elettriche"],"Materia":"ET","Tipo":"T","Stato":"🟢 Fatto","Slide":null,"PDF":null,"Parents":["[[🔌 Elettrotecnica]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET\|07 - Proprietà generali delle reti elettriche - ET]]

## Risolvere una rete


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/03-introduzione-allo-studio-delle-reti-elettriche-et/#rete-elettrica" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



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

La **topologia delle [[03 - Introduzione allo studio delle reti elettriche - ET#Rete elettrica|reti elettriche]]** è la descrizione delle interconnessioni esistenti tra i bipoli della rete

```

![07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.02.47.excalidraw.png](/img/user/Excalidraw/07%20-%20Propriet%C3%A0%20generali%20delle%20reti%20elettriche%20-%20ET%202024-06-15%2013.02.47.excalidraw.png)
[[Excalidraw/07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.08.39.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.10.02.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.11.18.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/07 - Proprietà generali delle reti elettriche - ET 2024-06-15 13.13.20.excalidraw\|🖋 Edit in Excalidraw]][[07 - Proprietà generali delle reti elettriche - ET 2024-06-15 17.30.32.excalidraw.md|🖋 Edit in Excalidraw]][[Excalidraw/07 - Proprietà generali delle reti elettriche - ET 2024-06-15 17.35.34.excalidraw\|🖋 Edit in Excalidraw]]%%

</div></div>

## Sistemi di equazioni topologiche

Le equazioni di [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Legge di Kirchhoff delle Correnti (LKC)\|#Legge di Kirchhoff delle Correnti (LKC)]] e [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Legge di Kirchhoff delle Tensioni (LKT)\|#Legge di Kirchhoff delle Tensioni (LKT)]] sono dette **equazioni topologiche della rete**. 

Per [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/07 - Proprietà generali delle reti elettriche - ET#Risolvere una rete\|#Risolvere una rete]] è necessario risolvere il sistema costituito da tutte le equazioni topologiche indipendenti.

In particolare ci saranno, in una rete di $n$ nodi e $l$ lati:
- $p := n-1:$ LKC indipendenti
- $m := l-p:$ LKT indipendenti (maglie indipendenti)


Un sistema di equazioni indipendenti sarà pertanto costituito da $p$ equazioni ai nodi (LKC) e $m$ equazioni alle maglie (LCT)

