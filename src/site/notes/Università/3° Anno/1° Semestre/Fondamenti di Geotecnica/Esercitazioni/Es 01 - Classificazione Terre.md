---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/fondamenti-di-geotecnica/esercitazioni/es-01-classificazione-terre/"}
---

 

# Esercitazione 1 - Classificazione Terre



![[Recording 20231002152747.webm]]


# Esercitazione
- [x] [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Esercizio 1\|#Esercizio 1]]
- [x] [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Esercizio 2\|#Esercizio 2]]
- [x] [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Esercizio 3\|#Esercizio 3]]
- [x] [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Esercizio 4\|#Esercizio 4]]

## Esercizio 1
## Esercizio 2
## Esercizio 3

## Esercizio 4
Sarà giusto?



PDF: [[Esercitazione 1 - classificazione terre.pdf]]


# Teoria
## Classificazione granulometrica


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#granulometria" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



# Granulometria

[[Università/2° anno/1° Semestre/Geologia applicata/Esercitazioni/Esercitazione 5 - Diagramma Granulometrico\|Esercitazione Diagramma Granulometrico]]
In base alla loro dimensione, gli ammassi di rocce si dividono in:

|                         |   |                          |
| -----------------------: | :-------: | :------------------------ |
| v                       | Argille | $< 2 \, \mathrm{\mu m}$  |
| $2 \, \mathrm{\mu m} <$ | Limi    | $< 60 \, \mathrm{\mu m}$ |
| $60 \, \mathrm{\mu m}$  | Sabbie  | $< 2 \, \mathrm{mm}$     |
| $< 2 \, \mathrm{mm}$    | Ghiaie  | $< 20 \, \mathrm{mm}$    |
| $< 20 \, \mathrm{mm}$ | Ciottoli        |                          |

### Setacciatura

![Pasted image 20230113103945.png|500](/img/user/Universit%C3%A0/2%C2%B0%20anno/1%C2%B0%20Semestre/Geologia%20applicata/Esercitazioni/allegati/Pasted%20image%2020230113103945.png)

Metodo adottato per particelle con diametro $D > 2\, \mathrm{mm}$

I detriti vengono setacciati in una serie di setacci. I più grandi vengono trattenuti dal primo e man mano vengono trattenuti i più piccoli:
#### Trattenuto
La parte che rimane nel setaccio
#### Passante
La parte che non rimane nel setaccio

### Sedimentazione
Metodo adottato per particelle con diametro $D < 2\, \mathrm{mm}$
Disperdo le particelle in un fluido e misuro quelle che cadono sul fondo (le più pesanti cadranno per prime)

## Nomenclatura

![Drawing 2023-01-31 12.17.04.excalidraw.png](/img/user/Excalidraw/Drawing%202023-01-31%2012.17.04.excalidraw.png)

## Coefficienti
### Coefficiente di Uniformità

```ad-Teo
title: Coefficiente di Uniformità ($\text{U}$)

$
\mathrm{U} = \frac{d_{60}}{d_{10}}
$

Dove $d_{i} =$ Diametro al $i\%$ di passante


```

### Coefficiente di Curvatura

```ad-Teo
title: Coefficiente di Curvatura ($\text{C}$)

$
\mathrm{C} = \frac{d_{30}^{2}}{d_{60}d_{10}}
$

```



</div></div>


### Curva granulometrica

Si traccia dopo la [[Università/2° anno/1° Semestre/Geologia applicata/Esercitazioni/Esercitazione 5 - Diagramma Granulometrico#Setacciatura\|setacciatura]].

![IMG_2A256313DB1E-1.jpeg](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Fondamenti%20di%20Geotecnica/Esercitazioni/allegati/IMG_2A256313DB1E-1.jpeg)

Da $60 \, \micro m$ in su si riescono a distinguere i grani
Limo, toccandolo, si percepiscono i  grani
Argilla, non si sentono i grani neanche al tatto

```ad-hint
title: Figo, non lo sapevo!

L'argilla si usa per fare le maschere al viso perché entra nei pori.

```


Chiamiamo 
- $Q =$ Quantità di terreno soggetta alla prova
- $T_{d_{j}} =$ Il trattenuto al diametro $d_{j}$
- $P_{d_{j}} =$ Il passante al diametro $d_{j}$
- $q_{i} =$ Il trattenuto nel setaccio $i-$esimo.

$$
\begin{align}
T_{d_{j}} = \sum\limits_{i = 1}^{j} \frac{q_{i}}{Q} \cdot 100 \\
P_{d_{j}} = \sum\limits_{i = 1+j}^{n} \frac{q_{i}}{Q} \cdot 100
\end{align}
$$
$$
T+P = 100
$$



## Classificazione sui Limiti di Atterberg


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/1-semestre/geologia-applicata/lezioni/05-le-rocce-sedimentarie/#argille" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Argille

##### Contenuto d'acqua




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#contenuto-d-acqua" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Contenuto d'acqua

```ad-Teo
title: Contenuto d'acqua ($w$)

$
w = \frac{P_{w}}{P_{s}}
$

```

Per un'[[Università/2° anno/1° Semestre/Geologia applicata/Lezioni/05. Le Rocce Sedimentarie#Argille\|argilla]], si può avere $w = 300\%$. o anche fino al 600 nei casi più estremi.

Per misurare il contenuto d'acqua peso il campione naturale, poi lo asciugo e lo peso di nuovo. 

```ad-Teo
title: Gamma Sommerso

$
\gamma' = \gamma_{\text{sat}} - \gamma_{w}
$

dove $\gamma_{w} = 1 \, \mathrm{\frac{g}{cm^{3}}}$

```




</div></div>


### Limiti di Atterberg

![Drawing 2023-01-27 12.47.16.excalidraw.png](/img/user/Excalidraw/Drawing%202023-01-27%2012.47.16.excalidraw.png)

#### Limite di ritiro o di liquidità
<-- [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Argille\|#Argille]]
$\omega_l$: Il [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Contenuto d'acqua\|#Contenuto d'acqua]] al di sotto del quale, togliendo acqua, non varia più il volume.

Per verificarlo, faccio dei solchi e vedo quanti colpi servono.
Il valore tale che la fessura si richiude dopo 25 colpi.
Si fa con il cucchiaio di casagrande.

#### Limite di Plasticità
<-- [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Argille\|#Argille]]
$\omega_{p}$

Si calcola a mano.
Si lavora il materiale a mano.
si prende un pezzetto di materiale e fa uno spaghettino.
- Se viene uno spaghettino molto molto fino si sta ancora in campo plastico --> si continua a impastare
- Se lo spaghetto si rompe subito si è entrati troppo nel campo del solido --> si ricomincia

Il limite plastico è il contenuto d'acqua tale che i bastoncini si rompono a $3 \, \mathrm{mm}$.

#### Indice di Plasticità
<-- [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Argille\|#Argille]]
```ad-Definizione
title: Indice di Plasticità ($I_{p}$)

$
I_{p} = \omega_{l} - \omega_{s}
$

Un valore elevato di questo coefficiente indica un terreno molto resistente all'acqua

```


#### Indice di Consistenza
<-- [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Argille\|#Argille]]
```ad-Definizione
title: Indice di Consistenza ($I_{c}$)

$
I_{c} = \frac{\omega_{l} - \omega_{n}}{I_{p}}
$

dove $\omega_{n}$ è la condizione di campo.
$
0<I_{c}<1
$
- $I_{c} < 0$: Liquido
- $I_{c} \sim 0.1$: Plastico
- $I_{c} > 1$: Solido-Semisolido


```

L'indice di consistenza mette insieme grandezze intrinseche ([[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Limite di Plasticità\|#Limite di Plasticità]] e [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Limite di ritiro o di liquidità\|#Limite di ritiro o di liquidità]]) con grandezze sullo stato del materiale ([[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Contenuto d'acqua\|#Contenuto d'acqua]]).
#### Diagramma di Casagrande

![Pasted image 20230127130330.png](/img/user/Universit%C3%A0/2%C2%B0%20anno/1%C2%B0%20Semestre/Geologia%20applicata/Lezioni/allegati/Pasted%20image%2020230127130330.png)

Un terreno si dice argilloso anche se c'è un $20 \div 30 \%$ di argilla.

La maggior parte dei materiali si trova intorno alla linea diagonale-

### Attività

```ad-Definizione
title: Attività $A$

$
A = \frac{I_{p}}{CF}
$
dove $CF$ è il Clay Factor (la $\%$ di argilla)

```

![Drawing 2023-01-27 13.05.59.excalidraw.png](/img/user/Excalidraw/Drawing%202023-01-27%2013.05.59.excalidraw.png)



</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/3-anno/1-semestre/fondamenti-di-geotecnica/appunti/00-caratteristiche-generali-delle-terre/#peso-specifico-dei-granuli" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



##### Peso specifico dei granuli

```ad-Teo
title: Peso specifico del granulo


$
\gamma_{s} = \frac{P_{s}}{V_{s}}
$


```

Si misura col picnometro. Ad esempio un [[Università/2° anno/1° Semestre/Geologia applicata/Lezioni/07. Proprietà Fisiche delle Rocce#Picnometro ad Elio\|picnometro ad elio]].


</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/3-anno/1-semestre/fondamenti-di-geotecnica/appunti/00-caratteristiche-generali-delle-terre/#peso-dell-unita-di-volume-del-terreno" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



##### Peso dell'unità di volume del terreno
```ad-Teo
title: Peso dell'unità di volume del terreno

$
\gamma = \frac{P}{V} = \left[ \frac{\mathrm{kN}}{\mathrm{m^{3}}} \right]
$

```

Per terreno molto porosi si aggira intorno a 13
Per terreni molto densi si aggira intorno a 22
Per singoli granuli si varia tra $25 / 26 \frac{\mathrm{kN}}{m^{3}}$ fino a anche 42...
Per l'acqua: $\gamma_{w} = 10 \frac{\mathrm{kN}}{\mathrm{m^{3}}}$


</div></div>


Altre grandezze utili all'esercitazione:

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/3-anno/1-semestre/fondamenti-di-geotecnica/appunti/00-caratteristiche-generali-delle-terre/#indice-dei-vuoti" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



##### Indice dei vuoti


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#indice-dei-vuoti" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



#### Indice dei vuoti

```ad-Teo
title: Indice dei vuoti ($e$)

$
\begin{align}
e = \frac{V_{v}}{V_{s}} && 0 < e < \infty
\end{align}
$

```


</div></div>


Esistono materiali con indici dei vuoti molto alto, come 10 ecc.

Questi materiali necessitano di una speciale struttura della parte solida.
I granuli sono come delle carte disposte in modo da occupare il più spazio possibile:

![IMG_B8C141E7CBA1-1.jpeg](/img/user/Universit%C3%A0/3%C2%B0%20Anno/1%C2%B0%20Semestre/Fondamenti%20di%20Geotecnica/Appunti/allegati/IMG_B8C141E7CBA1-1.jpeg)

Questi materiali sono generalmente molto delicati ma a volte, grazie a precipitazione di alcuni minerali che agiscono da colla (come il carbonato di calcio), possono essere molto resistenti


Se faccio vibrare riduco i vuoti: causo un addensamento della terra. Se l'addensamento è basso ho [[Università/3° Anno/1° Semestre/Fondamenti di Geotecnica/Esercitazioni/Es 01 - Classificazione Terre#Indice dei vuoti minimo\|#Indice dei vuoti minimo]]. 

###### Indice dei vuoti minimo
$e_{min}$
###### Indice dei vuoti massimo
$e_{max}$

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/3-anno/1-semestre/fondamenti-di-geotecnica/appunti/00-caratteristiche-generali-delle-terre/#grado-di-saturazione" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



##### Grado di saturazione

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#grado-di-saturazione" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



#### Grado di saturazione

```ad-Teo
title: Grado di Saturazione ($S_{r}$)

$
\begin{align}
S_{r} = \frac{V_{w}}{V_{v}} && 0 < S_{r} < 1
\end{align}
$

```

Campione:
- Completamente saturo: $S_{r} = 1$
- Completamente asciutto: $S_{r} = 0$

</div></div>





<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/1-semestre/geologia-applicata/lezioni/07-proprieta-fisiche-delle-rocce/#contenuto-d-acqua" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



### Contenuto d'acqua

```ad-Teo
title: Contenuto d'acqua ($w$)

$
w = \frac{P_{w}}{P_{s}}
$

```

Per un'[[Università/2° anno/1° Semestre/Geologia applicata/Lezioni/05. Le Rocce Sedimentarie#Argille\|argilla]], si può avere $w = 300\%$. o anche fino al 600 nei casi più estremi.

Per misurare il contenuto d'acqua peso il campione naturale, poi lo asciugo e lo peso di nuovo. 

```ad-Teo
title: Gamma Sommerso

$
\gamma' = \gamma_{\text{sat}} - \gamma_{w}
$

dove $\gamma_{w} = 1 \, \mathrm{\frac{g}{cm^{3}}}$

```




</div></div>


L'acqua che è capace di "legarsi" ai granuli è detta acqua **adsorbita**.

</div></div>


$$
\gamma_{d} = \frac{P_{s}}{V_{tot}} \qquad \text{Gamma dry}
$$
