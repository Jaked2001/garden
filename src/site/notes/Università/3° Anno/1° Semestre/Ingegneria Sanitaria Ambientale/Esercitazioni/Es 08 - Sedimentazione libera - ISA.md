---
{"dg-publish":true,"permalink":"/universita/3-anno/1-semestre/ingegneria-sanitaria-ambientale/esercitazioni/es-08-sedimentazione-libera-isa/"}
---


# Es 08 - Sedimentazione libera - ISA

## Riferimenti teorici

Ricordo [[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/06. Sedimentazione#Equazione di Newton\|Equazione di Newton]]
$$
v_{s} = \sqrt{\frac{4}{3} \dfrac{\rho_{s}-\rho_{L}}{\rho_{L}} \dfrac{gD}{C_{D}}}
$$
[[Università/3° Anno/1° Semestre/Ingegneria Sanitaria Ambientale/Appunti/06. Sedimentazione#Equazione di Stokes\|Equazione di Stokes]] ($\rm Re < 0.3$)
$$
v_{s} = \frac{1}{18} \dfrac{(\rho_{s}-\rho_{L})gD^{2}}{\mu} = \frac{1}{18}\dfrac{(\gamma_{s}-\gamma_{L})D^{2}}{\mu}
$$
con
$$
\mathrm{Re} = \frac{\varphi\rho_{L}v_{s}D}{\mu} = \frac{\varphi v_{s}D}{\nu}
$$

$\varphi:$ fattore di forma: fattore di correzione per passare da particella di forma qualunque a forma sferica
$$
C_{D} =\rm \frac{24}{Re} + \frac{3}{\sqrt{Re}} + 0.34
$$
Cerchiamo di capire se posso applicare Stokes o se devo applicare Newton.

Prima applico Stokes. Verifico il valore di Reynolds calcolato con la velocità della formula di Stokes. Se $\rm Re<0.3$ va bene. Senno applico metodo di Newton (vd. teoria).

I gamma sono dati in chilogrammi forza!!! vanno convertiti in newton


...

Vogliamo l'efficienza di rimozione. Serve il grafico P-vs.
Serve la percentuale di passante. Noi abbiamo il trattenuto.

Efficienza di rimozione è
$$
E = 100 - P_{OR} + \frac{1}{v_{OR}} \int_{0}^{P_{OR}} v_{S}  \, dP
$$
