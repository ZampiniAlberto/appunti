1. **Funzioni principali del Livello 2:**
    - Consente agli stati superiori di accedere ai supporti di trasmissione per inoltrare i dati.
    - I livelli superiori rimangono ignari del protocollo utilizzato a livello data.
    - Accetta i pacchetti di livello 3 (ad esempio IP) e li incapsula in frame di livello 2, aggiungendo le informazioni necessarie per l'instradamento e la consegna corretta.
    - Controlla il posizionamento e la ricezione corretta dei dati sui mezzi di trasmissione (supporti), utilizzando tecniche come il controllo degli errori e il flusso.
    - Gestisce lo scambio di frame attraverso il supporto di rete tra punti terminali, assicurandosi che ogni frame raggiunga la destinazione corretta.
2. **Concetti chiave:**
    - **End Point:** Dispositivi terminali coinvolti nella comunicazione, come computer, stampanti o server. Gli end point rappresentano l'origine e la destinazione dei dati nella rete.
    - **Supporti:** Mezzi di trasmissione utilizzati per inviare i dati, come ad esempio cavi in rame (Ethernet), fibre ottiche o connessioni wireless.
    - **Incapsulamento:** Processo di confezionamento dei dati ricevuti dai livelli superiori in frame, aggiungendo header e trailer specifici del livello 2.
### Topologie di Rete
1. **Definizione di Topologia:** La topologia di rete si riferisce alla disposizione fisica o logica dei nodi e delle connessioni in una rete. La scelta della topologia influisce direttamente sulle prestazioni, sull'affidabilità e sulla scalabilità della rete.
2. **Tipi principali di topologie:**
    - **Topologia a bus:**
        - Tutti i dispositivi sono collegati a un unico cavo principale (bus).
        - Economica e semplice da implementare, ma soggetta a problemi di collisione e difficoltà di manutenzione.
    - **Topologia a stella:**
        - I dispositivi sono collegati a un dispositivo centrale, come uno switch o un hub.
        - Offre alta affidabilità, poiché un guasto a un singolo dispositivo non influenza l'intera rete, ma il dispositivo centrale rappresenta un punto critico.
    - **Topologia ad anello:**
        - I dispositivi sono collegati in una struttura circolare, con i dati che viaggiano in un'unica direzione.
        - Efficienza nel controllo del flusso dei dati, ma vulnerabile ai guasti di un singolo nodo o collegamento.
    - **Topologia a maglia:**
        - Ogni dispositivo è connesso a uno o più altri dispositivi, creando percorsi ridondanti.
        - Altamente affidabile grazie alla presenza di percorsi alternativi, ma costosa e complessa da implementare.
    - **Topologia ibrida:**
        - Combinazione di due o più tipologie di topologie standard, adattabile a esigenze specifiche.
3. **Considerazioni pratiche:**
    - L'efficienza della trasmissione dipende dalla topologia scelta.
    - La manutenzione e il costo variano in base alla complessità della topologia.
    - Le esigenze specifiche della rete, come la velocità, l'affidabilità e la scalabilità, influenzano la scelta della topologia.
### Ethernet
1. **Cos'è Ethernet?** Ethernet è una tecnologia di rete utilizzata per connessioni cablate. È uno degli standard più diffusi per la comunicazione dati nelle reti locali (LAN).
2. **Caratteristiche principali:**
    - Funziona principalmente a livello 2, ma può interagire anche con il livello fisico (Livello 1).
    - Utilizza frame per la trasmissione dei dati, che includono campi per l'indirizzo MAC di origine e di destinazione, il tipo di protocollo e i dati stessi.
    - Supporta diverse velocità di trasmissione, da 10 Mbps fino a 100 Gbps o più nelle implementazioni moderne.
    - Può operare su diverse topologie, in particolare su stella e ibrida, adattandosi alle esigenze delle reti aziendali e domestiche.
    - Implementa protocolli per il controllo delle collisioni, come CSMA/CD (Carrier Sense Multiple Access with Collision Detection), per garantire un utilizzo efficiente del supporto condiviso.
3. **Vantaggi di Ethernet:**
    - Semplicità e standardizzazione, che lo rendono compatibile con una vasta gamma di dispositivi.
    - Prestazioni elevate e costi contenuti rispetto ad altre tecnologie di rete.
    - Affidabilità e scalabilità, ideali sia per reti di piccole dimensioni che per grandi infrastrutture aziendali.