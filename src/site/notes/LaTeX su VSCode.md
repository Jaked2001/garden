---
{"dg-publish":true,"permalink":"/la-te-x-su-vs-code/","dg-note-properties":{"aliases":["Download LaTeX","Come uso LaTeX","Usare LaTeX","LaTeX offline"],"Tipo":"Tutorial","Stato":null,"Parents":["[[LaTeX\|LaTeX]]"],"Children":null,"Siblings":["[[VSCode\|VSCode]]"],"tags":null}}
---

# [[LaTeX su VSCode\|LaTeX su VSCode]]

Questa nota è scritta basandosi sull'installazione su MacOS Monterey (12.7) ma, in linea di principio, lo stesso procedimento può essere seguito anche su Windows.

Moltissime persone usano LaTeX da browser. Al sito [OverLeaf](https://www.overleaf.com/) è possibile registrarsi e iniziare a usare LaTeX senza necessità di installare nulla. Per quanto vantaggioso e semplice, questo metodo non permette di lavorare ai documenti in assenza di una connessione a internet.

Io preferisco usare [[LaTeX\|LaTeX]] all'interno di [[VSCode\|VSCode]]. Per farlo, è necessario installare una versione di LaTeX sul computer.

La versione base è disponibile [questo link](https://www.latex-project.org/get/). 

Una volta installato, occorre installare un'estensione su VSCode: [[LaTeX Workshop\|LaTeX Workshop]]



## Problemi

Certo! Ecco lo stesso contenuto senza indicazioni su Markdown, così puoi copiarlo direttamente come testo per una nota in Obsidian o altrove.

---

### 🛠️ Forzare VSCode a usare TeX Live invece di TinyTeX (macOS)

## 🔍 Problema iniziale

Durante la compilazione di un file LaTeX in VSCode con l'estensione **LaTeX Workshop**, ottenevo un errore del tipo:

```
! LaTeX Error: File `subcaption.sty` not found.
```

Anche se avevo installato **TeX Live**, il sistema usava **TinyTeX**, che non conteneva tutti i pacchetti necessari.

---

## ✅ Soluzione: sostituire il link simbolico di `pdflatex`

### 1. Verificare quale `pdflatex` viene usato

Nel terminale:

```
which pdflatex
```

Output:

```
/usr/local/bin/pdflatex
```

Poi:

```
ls -l /usr/local/bin/pdflatex
```

Output:

```
/usr/local/bin/pdflatex -> /Users/matteomeloni/Library/TinyTeX/bin/universal-darwin/pdflatex
```

Questo indica che stava usando TinyTeX, non TeX Live.

---

### 2. Rimuovere il vecchio link simbolico

```
sudo rm /usr/local/bin/pdflatex
```

(Chiede la password di amministratore)

---

### 3. Creare un nuovo link simbolico verso TeX Live

```
sudo ln -s /usr/local/texlive/2024/bin/universal-darwin/pdflatex /usr/local/bin/pdflatex
```

---

## 💡 Note aggiuntive

- Se necessario, ripetere la stessa procedura anche per altri comandi come `latexmk`, `xelatex`, ecc.
    
- TinyTeX si trova di solito in `~/Library/TinyTeX/`
    
- TeX Live è in `/usr/local/texlive/YEAR/`
    

---

## 📁 Riferimenti utili

- TeX Live: [https://www.tug.org/texlive/](https://www.tug.org/texlive/)
    
- TinyTeX: [https://yihui.org/tinytex/](https://yihui.org/tinytex/)
    
- LaTeX Workshop – VSCode extension: [https://github.com/James-Yu/LaTeX-Workshop](https://github.com/James-Yu/LaTeX-Workshop)
    

---

Fammi sapere se vuoi aggiungere anche una sezione su come aggiornare TeX Live o gestire i pacchetti!