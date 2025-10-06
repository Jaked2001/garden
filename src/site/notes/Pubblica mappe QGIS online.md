---
{"dg-publish":true,"permalink":"/pubblica-mappe-qgis-online/"}
---

# [[Pubblica mappe QGIS online\|Pubblica mappe QGIS online]]

- [[LizMap\|LizMap]]
	- Interamente configurabile tramite interfaccia grafica
	- Non semplicissimo
	- Richiede plugin QGIS
- [[QGIS Web Client2\|QGIS Web Client2]]
	- Molto moderno
	- Installazione complicata
	- Richiede conoscenza linguaggi web (javascript)
- [[G3W-Suite\|G3W-Suite]]
	- Simile a LizMap e più semplice
	- Tutte le configurazioni da web, no plugin in QGIS


# Risposta ChatGPT

Creare una mappa interattiva con **QGIS** e incorporarla in un sito web come **Google Sites** richiede l'uso di un plugin come **qgis2web** per generare una mappa interattiva. Successivamente, puoi caricarla su un servizio di hosting e integrarla tramite **iframe** in Google Sites. Ecco una guida passo-passo:

---

### **1. Crea la Mappa in QGIS**

1. **Prepara il Progetto**:
    
    - Aggiungi e stila i layer che vuoi includere.
    - Assicurati che i dati siano proiettati in un sistema di riferimento adatto al web mapping, come **EPSG:3857 (Web Mercator)**.
2. **Salva il Progetto**:
    
    - Salva il tuo progetto QGIS per assicurarti di non perdere il lavoro.

---

### **2. Esporta la Mappa con QGIS2Web**

1. **Installa il Plugin qgis2web**:
    
    - Vai su **Plugins** > **Gestisci e Installa Plugin**.
    - Cerca **qgis2web** e clicca su **Installa**.
2. **Esporta la Mappa**:
    
    - Vai su **Web** > **qgis2web** > **Crea Web Map**.
    - Configura i parametri di esportazione:
        - **Formato**: Scegli tra **Leaflet** o **OpenLayers** (Leaflet è più leggero e ampiamente supportato).
        - **Popup**: Configura i popup per visualizzare le informazioni dei layer (se necessario).
        - **Estensione della mappa**: Verifica che l'estensione sia quella desiderata.
        - **Stili**: Scegli se vuoi mantenere gli stili del layer di QGIS.
    - Fai clic su **Esporta** e scegli una cartella dove salvare i file.
3. **Output**:
    
    - Verranno generati diversi file (HTML, CSS, JavaScript, ecc.) nella cartella selezionata.

---

### **3. Carica i File su un Servizio di Hosting**

Poiché Google Sites non permette l'upload diretto di file HTML, devi utilizzare un servizio di hosting per rendere la mappa accessibile online.

#### Opzioni di Hosting:

1. **GitHub Pages** (gratuito):
    
    - Crea un repository su GitHub e carica i file della mappa.
    - Vai su **Settings** > **Pages** e abilita GitHub Pages scegliendo la cartella dove sono i file.
    - Otterrai un URL pubblico come `https://tuo-username.github.io/mappa/`.
2. **Netlify** (gratuito):
    
    - Crea un account su [Netlify](https://www.netlify.com/).
    - Trascina la cartella con i file della mappa nella dashboard di Netlify.
    - Netlify genererà un URL pubblico come `https://nome-progetto.netlify.app`.
3. **Google Drive**:
    
    - Comprimi i file della mappa in un archivio `.zip`.
    - Carica il file su Google Drive e usa un servizio di "web hosting" per Google Drive (es. [DriveToWeb](https://drv.tw/)).

---

### **4. Incorpora la Mappa in Google Sites**

1. **Ottieni l'URL della Mappa**:
    
    - Dopo aver pubblicato la mappa sul servizio di hosting, copia l'URL pubblico (es. `https://tuo-username.github.io/mappa/`).
2. **Incorpora l'URL in Google Sites**:
    
    - Vai su **Google Sites** e apri il tuo sito.
    - Clicca su **Inserisci** > **Incorpora** > **Inserisci URL**.
    - Incolla l'URL della mappa e clicca su **Aggiungi**.
    - Posiziona la mappa nella pagina e regola le dimensioni.
3. **Salva e Pubblica**:
    
    - Salva le modifiche al tuo sito Google Sites e pubblicalo per renderlo accessibile.

---

### **5. Testa la Mappa**

- Apri il sito pubblicato e verifica che la mappa interattiva sia visibile e funzionante.
- Se riscontri problemi, controlla che i file siano correttamente hostati e che l'URL sia accessibile pubblicamente.

---

Se hai bisogno di aiuto con un passaggio specifico, fammi sapere! 😊

<iframe width="700" height="400" src="https://jaked2001.github.io/MappaCiclabiliRoma/" title="Titolo" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
