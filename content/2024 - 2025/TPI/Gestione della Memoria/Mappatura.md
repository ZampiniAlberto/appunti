La **mappatura** è un processo eseguito dal sistema operativo e dall'hardware del computer per tradurre un indirizzo logico, utilizzato dai programmi in esecuzione, nel corrispondente indirizzo fisico nella memoria principale. Questa traduzione è effettuata dalla **Memory Management Unit (MMU)**.
## Dettagli del processo
1. **Indirizzo logico**
    - Definito dal programma in esecuzione.
    - Utilizzato per riferirsi a una posizione di memoria virtuale.
2. **Traduzione tramite MMU**
    - L'MMU intercetta ogni accesso alla memoria.
    - Traduce l'indirizzo logico in un indirizzo fisico, utilizzando strutture dati come tabelle delle pagine (Page Tables).
3. **Indirizzo fisico**
    - Localizzazione effettiva di un dato o istruzione nella memoria principale (RAM).
    - Reso trasparente al programmatore grazie al processo di mappatura.
## Strumenti e risorse
- **Tabelle delle pagine**: Mappe che associano blocchi di memoria logica a blocchi di memoria fisica.
- **Registro base e limite**: Metodi semplici per controllare l'accesso alla memoria.
- **TLB (Translation Lookaside Buffer)**: Cache veloce che memorizza traduzioni recenti per ottimizzare le prestazioni.
## Vantaggi del processo di mappatura
- **Gestione della memoria**: Permette l'uso della memoria virtuale, consentendo programmi più grandi della memoria fisica.
- **Sicurezza**: Isola i processi, evitando che accedano a memoria non autorizzata.
- **Flessibilità**: Consente il caricamento dinamico dei processi.