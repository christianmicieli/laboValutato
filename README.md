# Labo-String: CLI per Utilità su Stringhe

Questo progetto fornisce una base per una semplice Command-Line Interface (CLI) Node.js che offre diverse utilità per la manipolazione di stringhe.

## Nota Importante per lo Studente - Setup Iniziale del Progetto

Benvenuto/a a `labo-string`!

Questo repository è un **template di partenza** per il tuo laboratorio valutato. Come avrai modo di leggere nelle istruzioni del laboratorio, una parte fondamentale del tuo lavoro iniziale (Esercizio 1) consisterà nell'analizzare attentamente la struttura e la configurazione corrente di questo progetto.

**Potresti notare che alcuni aspetti della configurazione iniziale – inclusa questa stessa documentazione (`README.md`), il file `package.json` e la gestione dei file da ignorare (`.gitignore`) – sono stati volutamente lasciati incompleti o potrebbero non seguire tutte le best practice per un progetto Node.js.**

Il tuo primo compito sarà proprio quello di identificare queste aree di miglioramento e apportare le necessarie correzioni e completamenti, come dettagliato nelle istruzioni del laboratorio, per portare il progetto a uno standard qualitativo superiore.

Buona analisi e buon lavoro!

## Funzionalità Principali (Previste)

* Inversione di una stringa.
* Verifica se una stringa è palindroma.
* Troncamento di una stringa a una lunghezza massima specificata.
* Conteggio delle occorrenze di ciascun carattere in una stringa.

## Installazione e Avvio

### Setup

- Per clonare il repository in locale:


git clone https://github.com/christianmicieli/laboValutato.git

cd laboValutato

- Per installare le dipendenze: 

npm install

### Avvio 

node index.js

---
# TEST


Il progetto utilizza Jest per i test unitari. Le funzioni di utilità in `stringUtils.js` sono completamente testate con una copertura del 100%.

### Eseguire i test

- Per eseguire i test unitari:

npm test

# CI

### Continuous Integration (CI) con GitHub Actions

Abbiamo integrato un workflow di GitHub Actions per automatizzare l’esecuzione dei test unitari e la generazione del report di coverage ad ogni modifica sul branch main.

### Scopo:
- Assicurare che ogni modifica al codice sia testata automaticamente.
- Monitorare la qualità del codice tramite il report di coverage.
- Rendere facilmente accessibile il report HTML di coverage come artefatto del workflow.

### Il workflow si attiva automaticamente su:
- push sul branch main
- pull request verso il branch main

### Viene eseguito un job che:
- Clona il repository
- Configura Node.js con caching delle dipendenze npm
- Installa le dipendenze con npm ci
- Esegue i test con Jest includendo la generazione del report di coverage
- Carica la cartella coverage/ come artefatto, contenente il report HTML completo

### Visualizzazione del report di coverage

Dopo l’esecuzione del workflow, è possibile scaricare il report di coverage in formato HTML direttamente dalla pagina Actions di GitHub, aprendo il file index.html presente nella cartella scaricata (coverage/lcov-report/index.html).


*Suggerimento: Presta particolare attenzione ai requisiti dell'Esercizio 1 del laboratorio per completare e correggere questo README e gli altri file di configurazione.*
