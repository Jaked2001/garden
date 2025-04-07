---
{"dg-publish":true,"permalink":"/piano-regolatore-generale-di-roma/"}
---

# [[Piano Regolatore Generale di Roma\|Piano Regolatore Generale di Roma]]



## Come accedere

- Geoportale: [https://geoportale.comune.roma.it/](https://geoportale.comune.roma.it/)
	- Permette di visualizzare tutti i layer direttamente su browser  
- [[Web Map Service\|WMS]]: [https://geoportale.comune.roma.it/geoserver/ows?service=WMS&request=GetCapabilities](https://geoportale.comune.roma.it/geoserver/ows?service=WMS&request=GetCapabilities)
	- Permette di visualizzare tutti i layer in QGis (o simili) come file raster. Non si possono interrogare i layer  
- [[Web Feature Service\|WFS]] (versione 1.0): [https://geoportale.comune.roma.it/geoserver/ows?service=WFS&request=GetCapabilities](https://geoportale.comune.roma.it/geoserver/ows?service=WFS&request=GetCapabilities)
	- Permette di visualizzare tutti i layer in QGis (o simili) con tutti gli attributi. Si possono quindi importare i layer così come sono stati creati dal comune e li si possono interrogare 
	- IMPORTANTE: in [[QGIS\|QGis]] selezionare “Versione 1.0” in _opzioni WSF_ altrimenti non funziona

Per i WMS e WFS si devono copiare e incollare i rispettivi link nella sezione apposita di QGis. Il comune mette a disposizione una guida passo passo che allego.


