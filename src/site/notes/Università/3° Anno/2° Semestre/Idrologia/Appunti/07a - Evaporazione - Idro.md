---
{"dg-publish":true,"permalink":"/universita/3-anno/2-semestre/idrologia/appunti/07a-evaporazione-idro/","tags":["UNI"]}
---

# [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07a - Evaporazione - Idro\|07a - Evaporazione - Idro]]

L'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Evaporazione\|evaporazione]] è una [[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro\|perdita idrologica]].

# Metodi di stima dell'evaporazione

- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07a - Evaporazione - Idro#Metodo energetico\|#Metodo energetico]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07a - Evaporazione - Idro#Metodo aerodinamico\|#Metodo aerodinamico]]
- [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07a - Evaporazione - Idro#Metodo combinato di Penman-Monteith\|#Metodo combinato di Penman-Monteith]]

## Metodo energetico

Dato un corpo idrico in quiete eseguo un bilancio energetico:

![07 - Evaporazione - Idro 2024-05-05 10.58.39.excalidraw.png](/img/user/Excalidraw/07%20-%20Evaporazione%20-%20Idro%202024-05-05%2010.58.39.excalidraw.png)


Accumulo di calore interno = scambi di calore con l'esterno
$$
\rho WC\Delta T = R_{n} - H_{S}-H_{l}-H_{g}
$$
dove:
- $W:$ Volume del corpo idrico
- $\rho:$ Densità dell'acqua
- $C:$ Calore specifico dell'acqua
- $\Delta T$: Variazione di temperatura dell'acqua nell'intervallo $\Delta T$
- $R_{n}:$ Flusso d'energia **radiante netta** in $\Delta t$
- $H_{S}:$ Flusso di **calore sensibile** dall'acqua all'atmosfera in $\Delta t$
- $H_{l}:$ Flusso di **calore latente** dell'acqua evaporata in $\Delta t$
	- Dovuto al passaggio di stato del liquido
- $H_{g}:$ Flusso di **calore trasmesso alla terra** in $\Delta t$

Sotto l'ipotesi di **fenomeno stazionario** ($\Delta T= 0$), il termine al primo membro risulta nullo. Inoltre posso trascurare $H_{g}$. Ottengo così:
$$
R_{n} - H_{S} - H_{l} = 0
$$
Noi siamo interessati al flusso di calore latente d'acqua evaporata ($H_{l}$) in quanto questo contiene l'informazione su quanta acqua sta evaporando.

Posso ricavare $R_{n}$ con la seguente:
$$
R_{n} = R(1-\alpha) - R_{p}
$$
dove:
- $R:$ Radiazione solare diretta o quella diffusa o riflessa dal cielo e dalle nuvole
- $\alpha:$ [[Università/3° Anno/2° Semestre/Idrologia/Appunti/01 - Atmosfera#Albedo\|albedo]]
- $R_{p}:$ Radiazione propria della superficie evaporante

Posso ricavare $H_{l}$ con la seguente:
$$
H_{l} = \lambda_{e} \Phi_{\nu,z} = \lambda_{e}\rho E
$$
dove:
- $\Phi_{\nu,z}:$ Flusso verticale della massa di vapore
	- È dato proprio da $\rho E$ dove $E$ è l'[[Università/3° Anno/2° Semestre/Idrologia/Appunti/06 - Perdite - Idro#Altezza di evaporazione\|altezza di evaporazione]]
- $\lambda_{e}:$ Calore latente di evaporazione

Posso sostituire $H_{l}$ nell'equazione di bilancio e dividerla tutta per $H_{l}$
$$
\begin{align}
R_{n} - H_{S} - H_{l} &= 0 \\
R_{n} - H_{S} - \lambda_{e}\rho E &= 0 \\
\frac{R_{n}-H_{S}-\lambda_{e}\rho E}{\lambda_{e}\rho E} &= 0
\end{align}
$$
Che posso spezzare:
$$
1 = \frac{R_{n}}{\lambda_{e}\rho E} - \frac{H_{S}}{\lambda_{e}\rho E} = \frac{E_{r}}{E} - \beta
$$
dove:
- $E_{r}=\frac{R_{n}}{\lambda_{e}\rho}:$ evaporazione che avrebbe luogo se il flusso di calore sensibile fosse trascurabile
- $\beta= \dfrac{H_{S}}{\lambda_{e}\rho E} = \dfrac{H_{S}}{\lambda_{e}\Phi_{\nu,z}}:$ **Rapporto di Bowen** tra il flusso di calore sensibile e quello latente

Si ricava quindi che:

```ad-Teo
title: Metodo dell'Evaporazione

$
E = \frac{E_{r}}{1+\beta}
$
dove:
- $E_{r}$ è un termine che deriva dall'irraggiamento: è l'evaporazione che avrebbe luogo se il flusso di calore sensibile fosse trascurabile ($H_{s} = 0$). Con $H_{s}=0$, $\beta= 0$
```


![Schermata 2024-05-05 alle 11.31.08.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-05-05%20alle%2011.31.08.png)

![Schermata 2024-05-05 alle 11.31.36.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-05-05%20alle%2011.31.36.png)

![Schermata 2024-05-05 alle 11.31.44.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/allegati/Schermata%202024-05-05%20alle%2011.31.44.png)

![Schermata 2024-05-05 alle 11.32.09.png](/img/user/Universit%C3%A0/3%C2%B0%20Anno/2%C2%B0%20Semestre/Idrologia/Appunti/allegati/Schermata%202024-05-05%20alle%2011.32.09.png)

## Metodo aerodinamico

❗❗❗❗❗❗❗❗❗❗❗❗
❗❗❗ COMPLETARE ❗❗❗
❗❗❗❗❗❗❗❗❗❗❗❗

## Metodo combinato di Penman-Monteith

Il [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07a - Evaporazione - Idro#Metodo energetico\|#Metodo energetico]] tiene conto dell'evaporazione dovuta all'irraggiamento.
Fornisce:
$$
E = \frac{E_{r}}{1+\beta }
$$

Il [[Università/3° Anno/2° Semestre/Idrologia/Appunti/07a - Evaporazione - Idro#Metodo aerodinamico\|#Metodo aerodinamico]] tiene conto dell'evaporazione dovuta agli effetti del vento.

È necessario combinare i due effetti per avere una valutazione completa dell'evaporazione. Si ottiene così

$$
E = \frac{\gamma E_{a}-\Delta_{e}E_{r}}{\gamma + \Delta_{e}}
$$
