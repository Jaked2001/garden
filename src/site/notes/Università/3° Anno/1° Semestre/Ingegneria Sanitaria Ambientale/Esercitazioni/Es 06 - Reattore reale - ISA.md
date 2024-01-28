---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/ingegneria-sanitaria-ambientale/esercitazioni/es-06-reattore-reale-isa/"}
---

# Es 6 - Reattore reale - ISA

Graficando i dati otteniamo un andamento che sembra essere esponenziale e che sembra tendere a 100, il valore di ingresso.

Posso pensare che la prima parte, che corrisponde a un ritardo, potrebbe essere un PFR. La seconda potrebbe essere un CFSTR. Oppure può essere il contrario:
PFR --> CFSTR oppure CFSTR --> PFR.
Questa è un'ipotesi. Dobbiamo verificare che l'andamento torni.

il $\theta_{H}$ del PFR sarebbe $10 \, \rm min$.

Il CFSTR ha equazione:
$$
C_{A_{u}}(t) = C_{A_{0}} (1- e^{- \frac{t}{\theta_{H_{\rm CFSTR}}}})
$$
Riscrivo in modo da poter ricavare $\theta_{H_{\rm CFSTR}}$ ($C_{A_{u}} \equiv C_{A_{u}}(t)$)
$$
e^{- \frac{t}{\theta_{H_{\rm CFSTR}}}} = 1- \frac{C_{A_{u}}}{C_{A_{0}}}
$$
poi faccio il $\ln$:
$$
- \frac{t}{\theta_{H_{\rm CFSTR}}} = \ln \left( 1- \frac{C_{A_{u}}}{C_{a_{0}}} \right)
$$
grafico con y a destra e x=t.

Poiché l'interpolazione viene abbastanza bene diciamo che abbiamo una serie di PFR e CFSTR con $\theta_{H}$ rispettivamente 10 min e 30.

NON È DETTO CHE Ciò CHE è EQUIVALENTE IDRAULICAMENTE LO SIA CHIMICAMENTE.

- [?] Che dobbiamo fare? Cos'è l'efficienza? 📅 2023-11-21 
	- Considerala come la concentrazione finale in uscita. Efficienza maggiore, significa concentrazione minore. In particolare, calcola confrontando le serie PFR-CFSTR con CFSTR-PFR


## Cinetica ordine 1

$$
k_{(1)} = 0.1 h^{-1} \qquad C_{A_{0}} = 200 \, \rm \frac{mg}{l}
$$
❗❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗❗
??? richiedi appunti

