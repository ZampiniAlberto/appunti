La **segmentazione** è un metodo di gestione della memoria che suddivide la memoria centrale in **segmenti** logici di dimensioni variabili, ciascuno associato a una parte specifica del programma o a un modulo software, che svolge una funzione precisa (ad esempio, **StampaDati**, **EstraiDati**). Ogni segmento rappresenta una struttura di dati o una sezione del codice che ha una propria semantica (come il codice eseguibile, le variabili globali o le risorse condivise).
#### Caricamento dei Segmenti
- Ogni **segmento** viene caricato su un **frame** di memoria centrale. I frame sono blocchi di memoria fisica di dimensioni fisse, che possono contenere un segmento, ma la dimensione del segmento può variare.
- I segmenti di un processo non devono essere contigui in memoria. Questo significa che i segmenti possono essere distribuiti in **frame non contigui**, migliorando la flessibilità nella gestione della memoria.
- Quando un segmento non è in uso, o la memoria centrale è piena, può essere spostato nell'**area di swap** (una porzione di memoria su disco), per fare spazio ad altri segmenti attivi. L'area di swap permette di liberare memoria fisica senza perdere i dati contenuti nei segmenti.
#### Traduzione degli Indirizzi
- Gli **indirizzi logici**, ossia quelli generati dal programma (ad esempio, i riferimenti a variabili o istruzioni), devono essere tradotti in **indirizzi fisici** (cioè quelli effettivi che corrispondono alla posizione nella memoria centrale).
- Questo processo di traduzione avviene attraverso la **Tabella dei Segmenti**, una struttura che mappa ogni segmento del programma alla sua posizione in memoria fisica. La tabella contiene informazioni su dove sono collocati i segmenti in memoria, la loro dimensione, e altre proprietà come la protezione dell'accesso.
### Vantaggi della Segmentazione
1. **Gestione delle Strutture di Dati Dinamiche**:
    - La segmentazione facilita la gestione di strutture di dati che crescono o diminuiscono durante l'esecuzione del programma, come **array dinamici**, **liste collegate** e **code**. La dimensione variabile dei segmenti permette di allocare memoria in modo efficiente, adattandosi alle necessità del programma.
2. **Facilitazione della Condivisione di Segmenti**:
    - La segmentazione permette di **condividere segmenti di memoria** tra più processi. Ad esempio, più processi possono condividere lo stesso segmento di codice eseguibile o una struttura di dati comune senza duplicare le informazioni, riducendo l'uso della memoria e migliorando l'efficienza.
3. **Semplificazione del Linking di Codice**:
    - La segmentazione facilita il **linking** di **procedure compilate separatamente**. Ogni modulo o funzione può essere compilato in modo indipendente, senza necessità di conoscere la posizione fisica dei segmenti. Questo rende più facile la gestione di programmi modulari e la manutenzione del codice.
4. **Protezione Differenziata dei Segmenti**:
    - Ogni segmento può avere un tipo di protezione specifico, che consente di controllare l'accesso alla memoria. Ad esempio:
        - Il segmento che contiene il **codice eseguibile** può essere protetto in **sola lettura**, evitando modifiche accidentali o dannose.
        - I **segmenti dati** (contenenti variabili globali o strutture di dati) possono essere protetti in **lettura e scrittura**, consentendo modifiche da parte dei processi.
        - Questo tipo di protezione aiuta a evitare errori e a migliorare la sicurezza del sistema.
5. **Flessibilità nella Gestione della Memoria**:
    - Poiché i segmenti possono essere distribuiti in frame non contigui, la memoria viene utilizzata in modo più efficiente, evitando la necessità di allocazioni di memoria continue. Questo può ridurre il **fragmentation** (frammentazione della memoria) e migliorare le prestazioni complessive del sistema.