
Il SO (sistema operativo) fa parte del software di base, inteso come insieme di programmi che consentono all’utente di utilizzare un calcolatore

Il software di base è costituito da:

- SO 
    

- editor
    
- compilatori
    
- linker
    
- loader è un componente del sistema operativo responsabile del caricamento di un programma in RAM
    
- debugger
    

funzione numero uno del SO

  

Il SO svolge la funzione di gestore di risorse hardware (le risorse sono gli elementi hardware o software del PC) Il SO supervisiona la scrittura e lettura dei dischi, la ricezione e la trasmissione dei dati attraverso tutti i dispositivi di I/O, l’esecuzione dei programmi caricando istruzioni e dati in RAM.

  

funzione numero due del SO

  

Il SO fornisce all’utente il supporto (un’interfaccia grafica o a linea di comando) per impartire i comandi necessari al funzionamento del computer. 

  

SO architettura a cipolla

Il kernel è un insieme di programmi del SO che:

● permette l’interazione tra HW e SW 

● è l’unico autorizzato ad accedere direttamente all’hardware, 

● gestisce le risorse HW nel modo più efficiente possibile controllandone tutti gli accessi 

● è responsabile dei driver più importanti 

● è responsabile per la trasmissione e la mediazione dei comandi

  

le funzioni sono:

● [[Gestione della memoria]]

● [[Gestore del processore]]

● Interagire coi Driver del dispositivo: si occupa dell’intermediazione tra l’hardware e i processi. 

● Gestire chiamate di sistema: accetta richieste di servizio dai processi.

  

l’utente può accedere alle chiamate di sistema grazie alla shell (interfaccia grafica) che avvolge il kernel per proteggerlo, l’interfaccia può essere grafica (GUI) o a linea di comando (CUI).