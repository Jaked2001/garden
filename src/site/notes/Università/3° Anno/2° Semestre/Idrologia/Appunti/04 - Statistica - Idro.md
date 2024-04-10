---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/idrologia/appunti/04-statistica-idro/"}
---

# [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro\|04 - Statistica - Idro]]

## Esperimento casuale




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/universita/2-anno/2-semestre/probabilita-e-statistica/appunti/02-misura-e-probabilita/#spazio-di-probabilita" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">



## Spazio di probabilità


```ad-Definizione
title: Spazio di probabilità
Uno spazio di probabilità è l'insieme $\Omega$ di tutti i possibili risultati, esaustivi e mutualmente esclusivi, di un dato esperimento casuale.

$
(\Omega, \mathcal{A}, P)
$
Dove
- $\Omega =$ Insieme eventi elementari
- $\mathcal{A} =$ "$\sigma$-Algebra indotta da $\Omega$" --> Insieme di tutti gli eventi ai quali possiamo essere interessati
- $P=$ Probabilità: $P: \mathcal{A} \to [0,1]$


```

$\sigma$-algebra è indotta da Omega. Si ottiene per chiusura di $\Omega$.

```ad-summary
title: Esempio: dado regolare

Nell'esempio del dado regolare abbiamo:
$\Omega = \{ 1,2,3,4,5,6 \}$  l'insieme degli eventi elementari

Se volessimo calcolare la probabilità che esca un numero $k$ otterremmo:

$
P(D=k) = 
\begin{cases}
\frac{1}{6} &\, k \in \Omega \\
0 &\, k \in \Omega^{c}
\end{cases}
\,\,\,\, k \in \mathbb{Z}
$

La probabilità che esca un numero pari è invece:
$
P(D \in \{ 2,4,6 \}) = P(\{2,4,6\}) = \frac{3}{6} = \frac{1}{2} = \frac{|\{ 2,4,6 \}|}{|\Omega|}
$

L'insieme di tutti gli eventi ai quali possiamo essere interessati è invece $\mathcal{A}$:
$
\mathcal{A} = \{ \Omega, \emptyset, \{1,2\},..., \{ 1,2,3\}, ... \}
$
Si ha poi che:
$P(\Omega) = 1$
$P(\Omega^{c}) = 0$


```


___
[[_Giornaliera/2023-03-03\|2023-03-03]]
___

$\mathcal{A}$: $\sigma$-algebra indotta da $\Omega$ si ottiene per chiusura rispetto a:
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Unione\|#Unione]]: Dati $E_{1}, E_{2} \Rightarrow E_{1} \cup E_{2}$
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Intersezione\|#Intersezione]]: Dati Dati $E_{1}, E_{2} \Rightarrow E_{1} \cap E_{2}$
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/04 - Statistica - Idro#Passaggio a complementare\|#Passaggio a complementare]]: Dato $E \Rightarrow E^{c}$ oppure $\overline E$

```ad-question

Un insieme chiuso è un insieme che contiene tutti i suoi punti di accumulazione. La chiusura di un insieme X è il più piccolo insieme chiuso che contiene X.
Un insieme chiuso può avere un numero finito di elementi? $\mathcal{A}$ ha sempre un numero infinito di elementi?

```

Chiusura rispetto a un'operazione e non rispetto a un altro insieme.

```ad-summary
title: Esempio: Dado

$
\mathcal{A} = \left\{ \Omega, \Omega^{c} = \emptyset, \{1\}, \{1\}^{c}, \{1,2\} = \{1\} \cup \{2\}, \{1\} = \Omega \smallsetminus \{2,3,4,5,6, ...\}  \right\}
$


```

### Assiomi

```ad-Teo
title: Assiomi probabilità

**A.1**: Gli eventi sono sottoinsiemi di $\Omega$ e formano $\mathcal{A}$

**A.2**: $\forall A \in \mathcal{A}$ è associato un numero $P(A) \in [0,1]$

**A.3**: $\mathcal{P}(\Omega) = 1$

**A.4**: Se $A \cap B = \emptyset \Rightarrow \mathcal{P}(A \cup B) = \mathcal{P}(A) + \mathcal{P}(B)$

**A.5**: Se $\{ A_{n}\}_{n \in \mathbb{N}}$ è decrescente e $\lim\limits_{n \to \infty} A_{n} = \emptyset \Rightarrow \lim\limits_{n \to \infty} \mathcal{P}(A_{n}) = 0$

```

#Dubbio


</div></div>


## Evento

```ad-Definizione
title: Evento

Dato uno [[02. Misura e Probabilità#Spazio di probabilità|Spazio di probabilità]] $\Omega$ relativo ad un [[#Esperimento casuale]], un **evento** è sempre un sottoinsieme di $\Omega$.

Tuttavia:
- Se $\Omega$ è costituito da un numero finito o da un'infinità numerabile di punti campionari, è evento ogni sottoinsieme $A$ di $\Omega$
- Se invece $\Omega$ è costituito da un'infinità non numerabile di punti non tutti i possibili sottoinsiemi di $\Omega$ ma soltanto i cosiddetti *sottoinsiemi ammissibili* di $\Omega$.
```


# Statistica e tempo di ritorno


