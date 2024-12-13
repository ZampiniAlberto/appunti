La memoria è un componente critico nei sistemi operativi (SO). Una parte della memoria è occupata dal SO stesso, mentre il resto è destinato ai processi utente. Durante l'esecuzione, i processi devono risiedere in memoria principale, ma in determinati stati (“bloccati” o “sospesi”), possono essere spostati in una memoria esterna per liberare spazio.
### Swapping
- **Definizione**: Lo spostamento temporaneo di processi tra memoria principale e memoria esterna si chiama _swapping_.
- **Scopo**: Libera memoria principale per permettere l'esecuzione di altri processi attivi.
- **Processo**:
    - Il processo sospeso è salvato su memoria esterna (es. disco rigido).
    - Quando è necessario riattivarlo, è ricaricato in memoria principale.
- **Limiti**:
    - Introduce un sovraccarico (_overhead_) significativo.
    - Lo swapping consuma spazio e richiede tempo per lo spostamento, riducendo l'efficienza generale.
## Tecniche di Multiprogrammazione
La multiprogrammazione consente l'esecuzione di più processi in parallelo, ma richiede una gestione efficiente della memoria per evitare sprechi.
### Ottimizzazione della Multiprogrammazione
- Per ridurre l'overhead dello swapping e il tempo di _context switching_:
    - Tenere il maggior numero possibile di processi attivi in memoria principale.
    - Usare tecniche di gestione della memoria efficienti.
## Tecniche di Allocazione della Memoria
La gestione della memoria si divide principalmente in due approcci:
### Allocazione Contigua
- **Definizione**: Ogni processo occupa un blocco unico e contiguo in memoria.
- **Vantaggi**:
    - Semplice da implementare.
    - Minimo overhead nella gestione.
- **Svantaggi**:
    - Possibile spreco di memoria per frammentazione interna.
    - Difficoltà nell'adattarsi a processi di dimensioni variabili.
### Allocazione Non Contigua
- **Definizione**: La memoria assegnata a un processo può essere suddivisa in blocchi non contigui.
- **Vantaggi**:
    - Riduce il problema della frammentazione.
    - Migliore utilizzo della memoria disponibile.
- **Svantaggi**:
    - Introduce overhead nella gestione.
    - Maggiore complessità nella traduzione degli indirizzi.