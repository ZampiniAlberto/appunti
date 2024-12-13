- La **paginazione** è una tecnica di gestione della memoria che divide sia la memoria fisica che la memoria logica (usata dai programmi) in blocchi di dimensioni fisse.
- Le **pagine logiche** (blocchi di memoria del programma) sono mappate in **pagine fisiche** (blocchi di memoria della RAM).
- Ogni programma è suddiviso in **pagine logiche** di dimensione fissa, mentre la memoria fisica è suddivisa in **pagine fisiche** di uguale dimensione.
#### Obiettivi:
1. **Ottimizzare l'uso della memoria**:
    - Non è necessario caricare l’intero programma in memoria, si caricano solo le pagine necessarie.
2. **Supporto per la memoria non contigua**:
    - Le pagine logiche non devono essere caricate in blocchi contigui, migliorando l’efficienza nell’utilizzo della memoria.
#### Gestione del Caricamento in Memoria:
1. **Se le pagine logiche sono minori delle pagine fisiche**:
    - Il programma può essere caricato interamente in memoria fisica.
2. **Se le pagine logiche sono maggiori delle pagine fisiche**:
    - Il programma viene caricato solo parzialmente. Le pagine non immediatamente necessarie vengono caricate più tardi.
#### Page Fault:
- Un **page fault** si verifica quando un processo cerca di accedere a una pagina che non è presente in memoria fisica.
- Quando si verifica un page fault, il sistema operativo carica la pagina mancante dalla memoria secondaria (disco) in memoria fisica.
#### Tecnica dello Swap-in:
- **Swap-in**: Quando una pagina è richiesta e non è presente in memoria, una delle pagine già caricate viene sostituita (spostata su disco), liberando spazio per la nuova pagina.
- Viene scelto generalmente il frame più vecchio o meno utilizzato nella memoria fisica da sostituire.
#### Ruolo della Memory Management Unit (MMU):
- La **MMU** è un componente hardware che si occupa di tradurre gli indirizzi **logici** (virtuali) in **indirizzi fisici** nella memoria.
- Gestisce la mappatura delle pagine logiche alle pagine fisiche.
- In caso di **page fault**, la MMU informa il sistema operativo affinché carichi la pagina richiesta.
#### Vantaggi della Paginazione:
1. **Isolamento tra i processi**:
    - Ogni processo ha il proprio spazio di memoria virtuale separato, prevenendo interferenze tra i processi.
2. **Flessibilità e gestione dinamica della memoria**:
    - La memoria può essere allocata in modo non contiguo, sfruttando meglio lo spazio disponibile.
3. **Efficienza nell'uso della memoria**:
    - Lo swap dinamico delle pagine consente di utilizzare la memoria in modo più efficiente e flessibile.
4. **Facilità di gestione**:
    - Il sistema operativo gestisce la suddivisione e la mappatura delle pagine, automatizzando il processo e riducendo il carico per il programmatore.