Quando è creato un nuovo processo, gli viene assegnato un identificatore (PID, Process Identifier) e viene inserito nell’elenco dei processi pronti. Quando gli viene assegnata la CPU, il processo passa nello stato di esecuzione, dal quale può uscire per tre motivi:

- Termina la sua esecuzione.
    
- Termina il suo tempo di CPU, cioè il quanto di tempo a sua disposizione.
    
- Gli manca la disponibilità di una risorsa: per poter evolvere necessita di una risorsa al momento non disponibile e quindi il processo si sospende e passa nello stato di attesa formando.
    

Dallo stato di sospeso (in WL) un processo esce solo quando ottiene la risorsa attesa.