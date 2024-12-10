**Codice rilocabile:** Quando un programma viene caricato in memoria, gli indirizzi relativi (logici) sono trasformati in indirizzi assoluti (fisici).

- **Rilocazione statica:** calcolo fatto al caricamento del programma, sommando l'indirizzo base agli offset.
    
- **Rilocazione dinamica:** durante l'esecuzione, ogni indirizzo logico è sommato al valore del registro base.

Per caricare un processo, la memoria deve avere spazio contiguo e sufficiente. Problemi:

- Programmi grandi che superano la RAM.
    
- Frammentazione dovuta al continuo caricamento e scaricamento di processi.
    
- Solo alcune istruzioni sono realmente eseguite.
    

Soluzioni:

1. **Swapping:** spostare processi inattivi su disco (rallentamenti possibili).
    
2. **Caricamento dinamico:** caricare solo le parti del programma necessarie.
    
3. **Overlay:** frazionare il programma e caricare le parti in memoria alternandole.
    
4. **Partizionamento:** dividere la memoria in blocchi di dimensioni [[Partizione Fisse]] o [[Partizioni variabili]].

**Memoria virtuale:** Permette di ridurre la frammentazione, caricando in memoria centrale solo le parti del programma in uso.

**Paginazione:**
La memoria è divisa in frame (fisici) e pagine (logiche) della stessa dimensione. Page fault: avviene quando una pagina necessaria non è in memoria e il SO la carica dal disco.

Ogni programma ha una tabella delle pagine che indica quali sono in RAM e quali su disco (bit di validità: 1 se in memoria, 0 altrimenti).

**Segmentazione:**
La memoria è divisa in segmenti di dimensioni variabili, associati a funzioni del programma (codice, dati, stack). Ogni segmento ha un indirizzo base e un limite. Segmentazione fault: avviene se un indirizzo supera il limite del segmento.

**Segmentazione con paginazione:**
Combina i vantaggi di entrambe. Ogni segmento è suddiviso in pagine logiche, caricate in frame fisici senza frammentazione. Gli indirizzi logici hanno tre componenti: segmento, pagina, spiazzamento, tradotti in frame e spiazzamento fisico tramite [[MMU]] e tabelle.

**Context switching:** è un concetto fondamentale nella gestione dei processi di un sistema operativo multitasking. Si verifica quando la CPU sospende l’esecuzione di un processo per passare a un altro. Durante questo passaggio, lo stato del processo interrotto viene salvato, in modo che possa riprendere l’esecuzione esattamente da dove era stato interrotto in un momento successivo.