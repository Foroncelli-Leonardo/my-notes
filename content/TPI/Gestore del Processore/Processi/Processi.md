Ogni processo è costituito da due parti:

- **Codice:** composto dalle istruzioni.
    
- **Dati del programma:** a loro volta suddivisi in:
    
    - Variabili globali, allocate nella RAM nell’area dati globali.
        
    - Variabili locali e non locali memorizzate in uno stack.
        
    - Variabili temporanee introdotte dal compilatore (tra cui PC o IP) caricate nei registri del processore.
        
    - Variabili allocate dinamicamente durante l’esecuzione, memorizzate in un heap*.

E’ possibile avere in esecuzione contemporaneamente più istanze di un programma, ossia più processi originati dallo stesso codice. I processi possono essere:

- **Indipendenti:** un processo può evolvere autonomamente senza necessità di scambiare dati con altri processi.
    
- **Cooperanti:** due o più processi per evolvere necessitano di scambiarsi informazioni.
    
- **Competitori:** due processi possono ostacolarsi a vicenda, per usare la medesima risorsa, compromettendo la terminazione delle loro elaborazioni.
    

Un programma può generare più processi, ma ogni processo è associato ad un solo programma.

**Processo utente:** processo generato da un programma scritto dall’utente.

**Processo supervisore:** processo generato da un programma del SO (es. gestore dell’attività).

I processi supervisori in esecuzione sulla CPU (in background) hanno un’importanza maggiore rispetto ai processi utente.

Quando un programma va in esecuzione viene creato il processo (memorizzato in memoria centrale).

Ogni processo ha un [[Ciclo di vita di un processo]]

**Descrittore del processo**
Il SO per ogni processo deve mantenere delle informazioni, che istante per istante tengano traccia di cosa sta “facendo il processo”. L’insieme di queste informazioni è detto descrittore di processo.