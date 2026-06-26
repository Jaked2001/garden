---
{"dg-publish":true,"permalink":"/universita/triennale/3-anno/2-semestre/elettrotecnica/appunti/17-conversione-elettromeccanica-dell-energia-et/","tags":["UNI"],"dg-note-properties":{"aliases":["Conversione elettromeccanica dell'energia"],"Materia":"ET","Tipo":"T","Stato":"🟢 Fatto","Slide":["[17 - Conversione Elettromeccanica dell’energia - ET.pdf](/img/user/17%20-%20Conversione%20Elettromeccanica%20dell%E2%80%99energia%20-%20ET.pdf)"],"PDF":null,"Parents":["[[🔌 Elettrotecnica]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET\|17 - Conversione elettromeccanica dell'energia - ET]]


È data una spira immersa in un campo magnetico uniforme, come in figura:

![Schermata 2024-06-30 alle 16.50.27.png](/img/user/Schermata%202024-06-30%20alle%2016.50.27.png)


## Trasformazione di potenza elettrica in potenza meccanica

Il diagramma sopra può essere rappresentato in proiezione secondo il seguente schema:

![17 - Conversione elettromeccanica dell'energia - ET 2024-06-30 16.51.07.excalidraw.png](/img/user/Excalidraw/17%20-%20Conversione%20elettromeccanica%20dell'energia%20-%20ET%202024-06-30%2016.51.07.excalidraw.png)
[[Excalidraw/Trasformazione di potenza meccanica in potenza elettrica - ET 2024-06-30 17.03.23.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/17 - Macchina elettrica - 1 coppia polare - ET 2024-06-30 18.19.19.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/17 - Linee di campo - 1 coppia polare - ET 2024-06-30 18.26.13.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/17 - 1 coppia polare - Linea di circuitazione - ET 2024-07-01 12.11.02.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/17 - Conversione elettromeccanica dell'energia - ET 2024-07-01 17.37.47.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/17 - Segnale rettangolare e addolcito - 1 coppia polare - ET 2024-07-01 17.51.52.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/17 -Macchina elettrica - 2 coppie polari - ET 2024-07-01 17.55.04.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/17 - Linee di campo - 2 coppie polari - 24-07-01 18.03.41.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/17 - Segnale rettangolare e addolcito - 2 coppie polari - ET 2024-07-01 18.08.46.excalidraw\|🖋 Edit in Excalidraw]]%%

## Alimentazione con corrente sinusoidale

Immaginiamo ora di alimentare la spira con una [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/14 - Reti in regime sinusoidale - ET#Regime sinusoidale\|corrente sinusoidale]]:
$$
i(t) = \sqrt{2}I\sin(\omega t)
$$
Il campo diventa:
$$
B_{\text{MAX}}(t) = \frac{\mu_{0}Ni(t)}{2\delta} = \frac{\mu_{0}N\sqrt{2}I}{2\delta}\sin(\omega t)
$$
A questo punto, a seconda di quante volte il filo percorre andata e ritorno (numero di polarità/2) si ha:
- $B(\theta,t) = - \dfrac{4}{\pi} \dfrac{\mu_{0}Ni(t)}{2\delta} \cos(\theta):$ per [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET#Alimentazione con 1 coppia polare\|#Alimentazione con 1 coppia polare]]
- $B(\theta,t) = - \dfrac{4}{\pi} \dfrac{\mu_{0}Ni(t)}{2\delta} \cos(2\theta):$ per [[Università/Triennale/3° Anno/2° Semestre/Elettrotecnica/Appunti/17 - Conversione elettromeccanica dell'energia - ET#Alimentazione con 2 coppie polari\|#Alimentazione con 2 coppie polari]]

$$
B(\theta,t) = - \dfrac{4}{\pi} \dfrac{\mu_{0}Ni(t)}{2\delta} \cos(p\theta)
$$
per p coppie polari





