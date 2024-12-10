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
    
4. **Partizionamento:** dividere la memoria in blocchi di dimensioni [Partizione Fisse] o [Partizioni variabili].

**Memoria virtuale:** Permette di ridurre la frammentazione, caricando in memoria centrale solo le parti del programma in uso.