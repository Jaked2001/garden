---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/2-semestre/travel-demand-and-behavioural-modeling/assignments/assgm-02-trip-distribution-and-modal-split-tdbm/"}
---


# [[Università/Magistrale/1° Anno/2° Semestre/Travel Demand & Behavioural Modeling/Assignments/Assgm 02 - Trip distribution & modal split - TDBM\|Assgm 02 - Trip distribution & modal split - TDBM]]

Assgm:[[Questionnaire_Distribution.pdf]]
## Q6

Discarded code that partially solves the question in matrix form:

```R
beta <- 0.2
q6_Tij <- mobs

for ( i in 1:53) {
  for (j in 1:53) {
    q6_Tij[i,j] = SD[i, "gtrips"] * SD[j,"atrips"] * exp(-beta * time[i,j])
  }
}

O_i <- matrix(0, nrow = 53, ncol = 1) # Origin marginal totals (target)
O_i <- matrix(SD$gtrips)
D_i <- matrix(0, nrow = 1, ncol = 53) # Destination marginal totals (target)
D_j <- t(matrix(SD$atrips))

o_i <- matrix(0, nrow = 53, ncol = 1) # Origin marginal totals (current)
o_i <- rowSums(q6_Tij)
d_j <- matrix(0, nrow = 1, ncol = 53) # Destination marginal totals (current)
d_j <- colSums(q6_Tij)

f_O <- matrix(0, nrow = 53, ncol = 1) # growth factor by origin

f_O = o_i/O_i
head(q6_Tij)
q6_Tij = q6_Tij * as.vector(f_O)
head(q6_Tij)


## Prova funzionamento prodotto matrice per vettore

matrice <- matrix(1, nrow = 10, ncol = 10)
vettore <- matrix(1:10, nrow = 10, ncol = 1)

prodotto <- matrice * as.vector(vettore)
head(prodotto)

```


DataFrame approach.
```{r}
source("Useful_func/Useful_Func.R")
beta <- 0.2
NDD$q6_Tij <- NDD$gen * NDD$atra * exp(-beta * NDD$ttime)

MT <- CalculateGrowthFactor(NDD, macroori, gen, q6_Tij) # Returns MT (Marginal totals with growth factor)

NDD <- left_join(NDD, MT[,c(1,4)],by=c("macroori"="macroori")) %>% data.frame()
NDD <- NDD %>% rename(q6_f = f)
NDD$q6_Tij <- NDD$q6_Tij * NDD$q6_f

par(mfrow = c(1, 2))  # 1 riga, 2 colonne
CheckInternalConsistenty(NDD, macroori, gen, q6_Tij, "target vs calculated - Origin")
CheckInternalConsistenty(NDD, macrodes, atra, q6_Tij, "target vs calculated - Des")
par(mfrow=c(1,1))
```


# Feedback

