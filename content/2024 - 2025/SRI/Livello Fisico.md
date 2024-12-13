**Tipi di Connessioni**
- **Cablato**: Connessione tramite cavi fisici, come rame o fibra ottica.
    - **Cavi in rame**:
        - Utilizzati comunemente nelle reti domestiche e aziendali.
        - Hanno un costo contenuto ma presentano limitazioni in termini di distanza e velocità rispetto alla fibra ottica.
        - Sono sensibili alle interferenze elettromagnetiche, che possono ridurre la qualità della trasmissione.
    - **Fibra ottica**:
        - Offre velocità elevate (fino a terabit al secondo) e trasmissione su lunghe distanze.
        - Resistente alle interferenze elettromagnetiche e al degrado del segnale.
        - Utilizzata in backbone di rete e in connessioni di rete ad alte prestazioni.
- **Wireless**: Connessione tramite onde radio, senza necessità di cavi fisici.
    - **Tecnologie wireless comuni**:
        - **Wi-Fi**: Utilizzato nelle reti locali, con copertura limitata e velocità variabili in base allo standard (ad esempio, Wi-Fi 5, Wi-Fi 6).
        - **Bluetooth**: Adatto per collegamenti a corto raggio tra dispositivi.
        - **LTE/5G**: Utilizzato per connessioni mobili a lunga distanza e ad alta velocità.
    - I dispositivi con connessioni wireless devono collegarsi a un **Access Point (AP)** o a un **router** per accedere alla rete.
**Access Point (AP):**
- Dispositivi fondamentali per reti wireless, con i seguenti componenti principali:
    - **Antenna wireless**: Trasmette e riceve segnali radio.
    - **Porte switch Ethernet**: Permettono il collegamento di dispositivi cablati.
    - **Porta internet**: Collega l’AP al modem o alla rete principale.
    - Possono essere configurati per estendere la copertura della rete wireless in ambienti grandi.
**Network Interface Card (NIC):**
- Dispositivo hardware che consente a un computer o dispositivo di connettersi a una rete.
    - **Tipi di NIC**:
        - Ethernet (per reti cablate).
        - Wi-Fi (per reti wireless).
    - Funzionalità avanzate:
        - Supporto per velocità Gigabit o superiori.
        - Funzioni di risparmio energetico.
        - Possibilità di configurazione tramite software.
**Funzione del Layer Fisico**
- **Scopo**: Permettere il trasporto di bit attraverso i supporti di rete, traducendo i dati digitali in segnali fisici e viceversa.
    - **Segnali fisici**:
        - Elettrici (nei cavi in rame).
        - Ottici (nella fibra ottica).
        - Radio (nelle connessioni wireless).
    - Gestisce aspetti come sincronizzazione, modalità di trasmissione (full-duplex, half-duplex), e adattamento ai diversi tipi di supporto fisico.
**Concetti Chiave**
1. **Collegamenti:**
    - **Larghezza di banda**: Determina la quantità di dati che possono essere trasmessi in un determinato intervallo di tempo. Influisce direttamente sulla velocità percepita dall’utente.
    - **Velocità di trasferimento**: Misurata in bit al secondo (bps), può variare in base a fattori come la qualità del supporto fisico e le condizioni ambientali.
2. **Cablaggio in rame:**
    - Comunemente usato per reti locali (LAN).
    - Include categorie di cavi come Cat5e, Cat6, e Cat7, ognuna con specifiche per velocità, schermatura e riduzione delle interferenze.
    - Richiede manutenzione periodica per prevenire deterioramenti o danni fisici.
3. **Fibra ottica:**
    - Utilizza impulsi luminosi per trasmettere dati.
    - Può raggiungere velocità elevatissime e mantenere qualità di segnale costante su lunghe distanze.
    - Richiede apparati specifici per l’installazione e la manutenzione.
4. **Codifiche:**
    - **Codifica di Manchester**: Metodo che rappresenta i bit tramite variazioni del segnale, garantendo sincronizzazione tra trasmettitore e ricevitore.
    - **Codifica di Shannon**: Basata sulla teoria dell’informazione, ottimizza l’efficienza della trasmissione minimizzando la ridondanza e aumentando la capacità di trasmissione.
5. **DNS (Domain Name System):**
    - Sebbene non appartenga direttamente al layer fisico, è essenziale per tradurre i nomi di dominio (es. www.example.com) in indirizzi IP, che rappresentano i veri destinatari dei dati sulla rete.
**Modalità di Trasmissione**
- **Simplex**: Dati trasmessi in una sola direzione.
- **Half-duplex**: Dati trasmessi in entrambe le direzioni, ma non contemporaneamente.
- **Full-duplex**: Dati trasmessi in entrambe le direzioni contemporaneamente.
**Nota Bene:** Il layer fisico è fondamentale per la trasmissione dei dati, ma collabora con altri layer per garantire una comunicazione affidabile ed efficiente.
- Ogni componente del layer fisico deve essere configurato e mantenuto correttamente per garantire prestazioni ottimali della rete.
- L’evoluzione delle tecnologie al layer fisico, come l’introduzione di nuovi standard (ad esempio, Wi-Fi 7), continua a migliorare le prestazioni e la qualità delle reti.