**Definizione generale:** Il passaggio dall’indirizzo logico a quello fisico è una parte essenziale nella gestione della memoria di un sistema operativo. Questo processo permette di tradurre gli indirizzi utilizzati dai programmi (logici) in indirizzi effettivi nella memoria fisica (RAM) per consentirne l’esecuzione.
### **Rilocazione Statica:**
- **Cosa significa:** Avviene prima dell’esecuzione del programma.
- **Descrizione del processo:** Il programma, originariamente salvato su memoria secondaria, viene trasferito nella memoria RAM. In questa fase, l’indirizzo logico è convertito in un indirizzo fisico stabile.
- **Esempio pratico:** Se un programma è caricato in un indirizzo fisso della RAM, non potrà essere spostato durante l’esecuzione.
### **Rilocazione Dinamica:**
- **Cosa significa:** Avviene durante l’esecuzione del programma.
- **Descrizione del processo:** Gli indirizzi delle istruzioni o dei dati vengono tradotti dinamicamente in indirizzi fisici. Questo processo è gestito dalla **MMU (Memory Management Unit)**.
    - La MMU si occupa della traduzione tra indirizzo logico e fisico ogni volta che il processore accede alla memoria.   
- **Vantaggi:**
    - Flessibilità: Il programma può essere spostato all’interno della RAM durante l’esecuzione.
    - Ottimizzazione dell’uso della memoria.
### **Ruolo della MMU (Memory Management Unit):**
- **Funzione principale:**
    - Esegue la mappatura dinamica degli indirizzi.
    - Garantisce l’isolamento tra i processi e la sicurezza nell’utilizzo della memoria.
- **Processo:** Ogni indirizzo logico generato dal programma passa attraverso la MMU, che lo converte in un indirizzo fisico utilizzabile.