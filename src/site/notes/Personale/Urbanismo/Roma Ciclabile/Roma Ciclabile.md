---
{"dg-publish":true,"permalink":"/personale/urbanismo/roma-ciclabile/roma-ciclabile/"}
---

# [[Personale/Urbanismo/Roma Ciclabile/Roma Ciclabile\|Roma Ciclabile]]

Sto lavorando a una mappa di tutte le ciclabili di Roma. Voglio che questa mappa sia il più completa e dettagliata possibile.

## Perché

Ci sono molte risorse in giro dalle quali visualizzare le ciclabili di una città. Concentriamoci su Roma. Quelle che mi vengono in mente sono:
- [[#Google Maps]]
- [[#Open Street Maps (CycleOSM)]]
- [[#PisteCiclabili.com]]
- [[#Salvaiciclisti.it]]

Ognuna di queste però ha delle limitazioni

[[#Motivazioni personali]]
### Google Maps

Google Maps è sicuramente la prima fonte che ci viene in mente. Contiene uno strato di visualizzazione chiamato "In bicicletta":

![Google Maps.jpeg](/img/user/Personale/Urbanismo/Roma%20Ciclabile/Allegati/Google%20Maps.jpeg)

Vediamo però che ci sono alcuni problemi:
- Non distingue tra percorsi protetti e non (corsie ciclabili o piste ciclabili senza separazione fisica)
- Tiene conto di molti itinerari nei parchi, poco utili alla mobilità, che vanno però ad intasare la vista
- Evidenzia alcune strade come "Strade adatte ai ciclisti". I parametri per questa definizione sono poco chiari e a volte sembrano totalmente campate in aria. Nella foto è evidenziato un tratto di Via San Gregorio (o Via Celio Vibennia) segnato appunto come adatto ai ciclisti. Sappiamo però che questa è una strada a 4 corsie (2 per senso di marcia, con spartitraffico centrale) percorso spesso ad alta velocità dagli automobilisti, in un tratto a forte pendenza, con curva parzialmente cieca. Tutte le vie residenziali del quartiere adiacente però non sono adatte ai ciclisti...
- Non permette di scaricare le informazioni in formati utili ad essere usati in altri progetti (ad esempio su un [[GIS\|GIS]])

### CycleOSM

In questo paragrafo discuto anche i dati di OpenStreetMap

![CyclOSM_ OpenStreetMap-based bicycle map.jpeg](/img/user/Personale/Urbanismo/Roma%20Ciclabile/Allegati/CyclOSM_%20OpenStreetMap-based%20bicycle%20map.jpeg)

[[CycleOSM\|CycleOSM]] è la mia mappa preferita. È una visualizzazione dei dati forniti [[Open Street Map\|Open Street Map]] pensata proprio per le persone in bicicletta. A colpo d'occhio permette di distinguere la tipologia di infrastruttura ciclabile (pista protetta oppure no, mono-direzionale o bidirezionale), se si tratta di un percorso segregato o ciclopedonale ma anche altri aspetti che riguardano le strade ma sono di interesse ai ciclisti: tipologia di strada, limite di velocità della strada, tipo di pavimentazione, direzione di percorrenza (inclusi i sensi unici eccetto bici). Sono inoltre segnalati i parcheggi per le bici o le rastrelliere e, se l'informazione è disponibile, anche quanti posti totali ci sono.

![Capture-2025-05-08-194227.png](/img/user/Personale/Urbanismo/Roma%20Ciclabile/Allegati/Capture-2025-05-08-194227.png)

Al meglio delle mie conoscenze, questa è la mappa più dettagliata (e utile) per chiunque usi la bici in città. Come anticipazione posso dire che il mio progetto sarà ampiamente ispirato a questa mappa. Rimangono comunque alcune limitazioni:
- Per quanto sia possibile scaricare tutti i dati da Open Street Map in maniera abbastanza semplice, ci sono alcune situazioni in cui questo processo diventa quanto meno sconveniente per mappare le ciclabili di una città. Ad esempio, su OSM, quando una ciclabile è costruita adiacente alle corsie carrabili, questa non viene mappata separatamente, ma viene aggiunto un tag al tratto stradale interessato. Quando si scaricano i dati, questi tratti devono essere mappati nuovamente a mano e sono in generale complicati da gestire.
- Per evitare confusione, solo gli itinerari esistenti o in corso di realizzazione possono essere mappati. Questo però impedisce di valutare l'evoluzione della rete secondo piani programmatici quali il [[PUMS\|PUMS]].

Per questi motivi reputo che ci sia motivo di realizzare una mappa (o meglio, un insieme di mappe). Aggiungo però che OSM è stata la fonte principale per la mia mappatura sulle ciclabili già esistenti.

### Pisteciclabili.com

![Schermata 2025-05-08 alle 19.51.46.png](/img/user/Personale/Urbanismo/Roma%20Ciclabile/Allegati/Schermata%202025-05-08%20alle%2019.51.46.png)

[pisteciclabili.com](www.pisteciclabili.com) è un sito che raccoglie moltissimi itinerari ciclabili di tutta Italia. Cliccando su ogni itinerario si accede ad una pagina ad esso dedicato dove sono contenute molte informazioni su di esso. In alcuni casi si tratta solo di informazioni di base: cosa collega, lunghezza, tempo di percorrenza. Per gli itinerari più popolari sono presenti pagine più approfondite. Inoltre è possibile sempre scaricare la traccia del percorso in vari formati. 

La limitazione più grande è che la mappa base, invece di visualizzare le tracce degli itinerari, li visualizza come punti. L'utente clicca sul punto, visualizza l'itinerario e può accedere alla pagina dello stesso. Queste la rende completamente inutile se si vuole avere un'idea generale della rete della città. Inoltre manca la distinzione sulla tipologia di pista ciclabile e mappa solo gli itinerari, non i percorsi veri e propri (se un tratto presenta due piste ciclabili a senso unico nei due lati della strada, viene visualizzato un unico percorso).

### Salvaiciclisti.it

Salvaiciclisti è un'associazione romana di ciclisti urbani. Con l'obiettivo di mappare l'andamento della realizzazione del PUMS hanno realizzato una mappa in GoogleMyMaps con vari itinerari esistenti e pianificati e alcune informazioni su di essi.

GoogleMyMaps però non permette una grande personalizzazione della simbologia, rendendo la mappa poco leggibile. Inoltre, come in pisteciclabili.com, non tengono conto del percorso esatto della ciclabile, ma solo degli itinerari.

### Motivazioni personali

Ci sono anche delle motivazioni personali che mi hanno spinto a realizzare questo progetto.

All'università ho imparato a usare [[QGIS\|QGIS]]. Adoro guardare vari tipi di carte, soprattutto in ambito urbano, e con questo software posso realizzare io stesso quello che voglio. Lo trovo uno strumento utilissimo oltre che spendibile in ambito professionale. Per questo motivo, voglio fare pratica e non c'è modo migliore di farlo che realizzare un progetto incentrato proprio su di esso. 

## Come

Come dovrebbe essere chiaro a questo punto, ho deciso di realizzare il tutto su QGIS. È  un software open source e completamente gratuito, che ho imparato a usare all'università e che è perfetto per questo scopo. Permette inoltre di importare i dati direttamente da Open Street Map tramite un plugin e di realizzare dei fantastici layout di stampa, con la massima libertà sulla simbologia. L'unico vero limite è la pubblicazione delle mappe. So che Arcgis di ESRI permette di realizzare carte dinamiche e veri e interi siti web a partire da un progetto. Per usarlo però è necessaria una licenza e, almeno la versione online, non consente la stessa libertà nella simbologia.

Esiste per QGIS un plugin, [[qgis2web\|qgis2web]] che permette di esportare le carte realizzate in html, il cui codice può poi essere incorporato all'interno di un sito web. 

L'obiettivo finale è quello di realizzare un sito web dal quale visualizzare le varie mappe che verranno create con la possibilità di scaricare i livelli visualizzati. Vorrei inoltre creare delle pagine dedicate agli itinerari più importanti, con informazioni riguardo l'itinerario stesso, sia di carattere culturale che ingegneristico (ad esempio allegando i progetti, qualora siano stati pubblicati dall'amministrazione).
