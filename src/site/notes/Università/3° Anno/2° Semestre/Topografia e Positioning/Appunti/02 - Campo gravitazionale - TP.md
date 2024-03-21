---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/02-campo-gravitazionale-tp/"}
---


# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/02 - Campo gravitazionale - TP\|02 - Campo gravitazionale - TP]]



## Geoide

```ad-Definizione
title: Geoide
Il **geoide** è una particolare superficie equipotenziale della gravità terrestre
```

La conoscenza del geoide ci permette di conoscere, ad esempio, come viaggiano le correnti oceaniche.

## Campo gravitazionale

Sappiamo, dalla fisica, che il campo gravitazionale è
$$
\vec{f} = -G \frac{Mm}{r^{3}} \vec{r}
$$
D'ora in poi, per semplicità, supporrò $m=1$. Guardo quindi al campo gravitazionale della Terra di massa $M$ che interagisce con una massa unitaria.
$$
\vec{f} = -G \frac{M}{r^{3}}\vec{r}
$$
Consideriamo la situazione sottostante:

![02 - Campo gravitazionale - TP 2024-03-21 17.32.51.excalidraw.png](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-21%2017.32.51.excalidraw.png)


Prendo un punto $P$ fermo rispetto alla superficie terrestre. Questo punto subisce l'attrazione di ogni elementino della Terra, $dM$ situato nel punto $Q$.
pertanto, la forza di attrazione gravitazionale sarà data da:
$$
\vec{f} = -G \int_{\text{vol. Terra}} \dfrac{dM}{r_{PQ}}\vec{r}_{PQ}
$$

Se introduco la rotazione della Terra a velocità angolare $\vec{\omega}$ attorno a un certo asse di rotazione, devo considerare anche la forza centrifuga generata come effetto di tale rotazione:
$$
\vec{c} = \omega^{2}\vec{l_{P}}
$$
A questo punto posso definire il campo di gravità terrestre come:

### Campo di gravità terrestre

```ad-Definizione
title: Campo di gravità terrestre
Il campo di gravità terrestre è la somma dell'attrazione Newtoniana e della forza centripeta

$$
\vec{g} = \vec{f} + \vec{c}
$$
```

#### Potenziale Newtoniano

```ad-Definizione
title: Potenziale newtoniano

Posso definire la forza attrattiva per mezzo di una funzione, detta [[Potenziale Newtoniano]] e dire che
$$
\vec{f} = \vec{\rm grad} V
$$

```

```ad-note
title: Osservazione
La forza centrifuga, dipendendo da $|\vec{l_{P}}|$, è massima all'Equatore e nulla ai Poli.
Quindi la gravità varia lungo la superficie terrestre
- per direzione
- per modulo

```

Anche il campo di forza centrifuga ammette un potenziale, detto **potenziale centrifugo**, per cui
$$
\vec{c} = \vec{\rm grad}C
$$
Si può dimostrare che il potenziale Newtoniano è pari a 
$$
V = G \int _{\text{Vol. Terra}} \frac{dM}{r_{PQ}} 
$$

Si può dimostrare che il potenziale centrifugo è pari a
$$
C = \frac{1}{2} \omega^{2} l_{P}^{2}
$$

![02 - Campo gravitazionale - TP 2024-03-21 17.55.14.excalidraw.png](/img/user/Excalidraw/02%20-%20Campo%20gravitazionale%20-%20TP%202024-03-21%2017.55.14.excalidraw.png)


Posso esplicitare $r_{PQ}$ e $l_{P}$ introducendo un sistema di coordinate centrato nel baricentro della Terra.
A questo punto avremmo
$$
\begin{align}
r_{PQ} &= \sqrt{(x_{P}-x_{Q})^{2} + (y_{P}-y_{Q})^{2} + (z_{P}-z_{Q})^{2}} \\
l_{P} &= \sqrt{x_{P}^{2} + y_{P}^{2}}
\end{align}
$$




