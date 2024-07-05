---
{"dg-publish":true,"permalink":"/universita/2-anno/2-semestre/gis/gis-1/elaborati/elaborato-2-uso-suolo/"}
---


###### Teoria: [[Università/2° anno/2° Semestre/GIS/GIS 1/6. Uso Suolo\|6. Uso Suolo]]

# Uso suolo
## Classi uso suolo

| ID Classe | Nome                                     | Colore |
| --------- | ---------------------------------------- | :----: |
| 1         | Urbanizzato e superfici artificiali      |   🔴   |
| 2         | Aree agricole                            |   🟡   |
| 3         | Prati, pascoli e aree aperte             |   🟢   |
| 4         | Aree boscate e con vegetazione arbustiva |  🟢⚫️  |
| 5         | Corpi idrici e zone umide                |   🔵   |



# Cambiamenti uso suolo 
Sovrappongo due layer di tipo vettoriale: 

![Pasted image 20221125085613.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/GIS/GIS%201/allegati%202/Pasted%20image%2020221125085613.png)

- Intersezione di aree: [[Operatori logici#^29fe89\|AND]]

![Pasted image 20221125085738.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/GIS/GIS%201/allegati%202/Pasted%20image%2020221125085738.png)

- Unione di aree: [[Operatori logici#^664163\|OR]]

![Pasted image 20221125085852.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/GIS/GIS%201/allegati%202/Pasted%20image%2020221125085852.png)

- Unione di aree senza intersezione: [[Operatori logici#^a9adf7\|OR]]

![Pasted image 20221125090814.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/GIS/GIS%201/allegati%202/Pasted%20image%2020221125090814.png)

- Sottrazione: NOT

![Pasted image 20221125090835.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/GIS/GIS%201/allegati%202/Pasted%20image%2020221125090835.png)

- Unione di aree della stessa categoria: Dissolving

![Pasted image 20221125090922.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/GIS/GIS%201/allegati%202/Pasted%20image%2020221125090922.png)

Sovrapporre dati con risoluzioni/MMU o altre proprietà differenti può portarci a commettere errori.

### Problemi di classificazione

Se ad esempio una categoria del sistema [[Corine Land Cover\|Corine Land Cover]] indica a bassa densità urbanizzata una densità tra il 10% e l'80% e in un'area la densità aumenta dall'11 al 79%, il cambiamento non verrebbe registrato. 
Se dal 79% passo all'81% il cambiamento viene invece registrato. 
Potrei non registrare cambiamenti per decenni, poi basta un edificio e cambio classe!

![Pasted image 20221125091443.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/GIS/GIS%201/allegati%202/Pasted%20image%2020221125091443.png)

## [[ℹ️ Simbologia IGM\|ℹ️ Simbologia IGM]]

I simboli spesso ingrandiscono la realtà:
Un edificio su carta IGM è più grande dell'edificio reale.
È bene usare l'ortofoto in questi casi

```ad-tip
title: Fare caso alle scritte
Se c'è scritto *Cava di Marmo*, è improbabile che ci sia un seminativo in quell'area 🙃
```


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/2-semestre/gis/gis-1/elaborati/elaborato-2-uso-suolo/#classi-uso-suolo" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Classi uso suolo

| ID Classe | Nome                                     | Colore |
| --------- | ---------------------------------------- | :----: |
| 1         | Urbanizzato e superfici artificiali      |   🔴   |
| 2         | Aree agricole                            |   🟡   |
| 3         | Prati, pascoli e aree aperte             |   🟢   |
| 4         | Aree boscate e con vegetazione arbustiva |  🟢⚫️  |
| 5         | Corpi idrici e zone umide                |   🔵   |




</div></div>


Dobbiamo disegnare nuovi poligoni nelle aree dove si sono registrati dei cambiamenti.

```ad-tip
title: snap
Se serve attivare lo snap.

Disattivarlo se devo disegnare un poligono vicino a un altro ma non voglio che si agganci
```

### Caratteristiche geometriche

Scala: 1:10000
MMU: 0,5 ha
Spessore minimo: 25m

```ad-warning
Questo è tecnicamente sbagliato. La [[scala nominale]] è 1:25000 e non potremmo ricavare un dato a scala maggiore. Noi però ci possiamo aiutare con l'ortofoto
```

![Schermata 2022-12-14 alle 16.04.18.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/2%C2%B0%20Semestre/GIS/GIS%201/Elaborati/allegati/Schermata%202022-12-14%20alle%2016.04.18.png)

