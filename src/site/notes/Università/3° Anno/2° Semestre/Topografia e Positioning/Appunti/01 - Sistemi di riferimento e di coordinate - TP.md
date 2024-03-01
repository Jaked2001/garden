---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/topografia-e-positioning/appunti/01-sistemi-di-riferimento-e-di-coordinate-tp/"}
---

# [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP\|01 - Sistemi di riferimento e di coordinate - TP]]

# Sistema di riferimento

Un sistema di riferimento può essere definito (almeno per ciò che è di nostro interesse) in 1, 2 o 3 dimensioni:

```ad-Definizione
title: Sistema di riferimento

Un **sistema di riferimento** è un insieme di scelte che individuano univocamente la posizione di un punto in un prefissato ambito dimensionale.

Le *scelte*, sono quelle che bloccano **tutti e soli** i [[02. Cinematica dei corpi rigidi#Gradi di Libertà|gradi di libertà (g.d.l.)]] di un corpo rigido in quell'ambito dimensionale

```

Potremo parlare di:
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento 2D\|#Sistema di riferimento 2D]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento 3D\|#Sistema di riferimento 3D]]
- [[Università/3° Anno/2° Semestre/Topografia e Positioning/Appunti/01 - Sistemi di riferimento e di coordinate - TP#Sistema di riferimento 1D\|#Sistema di riferimento 1D]]

| Ambito dimensionale | g.d.l. T | g.d.l. R   |
| ------------------- | -------- | ---------- |
| 1D                  | 1        | 0          |
| 2D                  | 2        | 1          |
| 3D                  | 3        | 3          |
|                     | Origine  | Assi/piani |



## Sistema di riferimento 2D

Immaginiamo di trovarci sul piano.
Un corpo rigido sul piano ha 3 gradi di libertà: 2 alla Traslazione e 1 alla Rotazione.

Vogliamo definire la posizione di un generico punto $P$.

Possiamo, per prima cosa, eliminare i gradi di libertà alla Traslazione, fissando un origine di un sistema di riferimento, $O$.

Successivamente, andremo a tracciare un asse $x$ il quale permette di bloccare il rimanente grado di libertà alla Rotazione.

Se si è fatta l'ipotesi di scegliere gli assi come ortonormali, basterà tracciare un unico asse. L'altro sarà infatti identicamente determinato, dovendo passare per $O$ e dovendo essere perpendicolare all'asse-$x$.

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-01 12.03.56.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-01%2012.03.56.excalidraw.png)


Per definire la posizione di un punto in uno spazio a 2 dimensioni, è **necessario** e **sufficiente** fissare:
- Un'origine
- Un asse passante per l'origine

## Sistema di riferimento 3D

Un Corpo Rigido in 3 Dimensioni ha 6 [[Università/2° anno/1° Semestre/Scienza delle costruzioni/Appunti/02. Cinematica dei corpi rigidi#Gradi di Libertà\|g.d.l.]]: 3T + 3R

- Fisso un'Origine O
- Fisso un asse $z$ (tolgo 2 gradi di libertà)
	- L'asse obbliga la giacitura del piano $x-y$
- Fisso un generico piano appartenente al **fascio proprio** di piani passante per l'asse $z$
Quest'ultimo piano identifica una retta nel piano $x-y$ che identifica l'asse $x$.

![01 - Sistemi di riferimento e di coordinate - TP 2024-03-01 18.26.13.excalidraw.png](/img/user/Excalidraw/01%20-%20Sistemi%20di%20riferimento%20e%20di%20coordinate%20-%20TP%202024-03-01%2018.26.13.excalidraw.png)



## Sistema di riferimento 1D

In uno spazio mono-dimensionale, un Corpo Rigido possiede 1 [[Università/2° anno/1° Semestre/Scienza delle costruzioni/Appunti/02. Cinematica dei corpi rigidi#Gradi di Libertà\|g.d.l.]]: 1T 

Per definire la posizione di un punto è sufficiente:
- Fissare un'origine O


# Sistema di coordinate


