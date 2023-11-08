# chat_gruppo6

**Tecnologie utilizzate**
  - Socket
  - Thread


**casi d'uso del client**
 - Connessione client: Mi connetto al server
 - Disconnessione client: Avverto il server della disconnessione
 - Invio messaggio / ricezione messaggio

**Casi d'uso del server**
  - Connessione server: Avverto connessione stabilita
  - Disconnessione di un client: Avverto tutti i client della disconnessione di uno di loro
  - Invio in broadcast: invio a tutti i client
  - invio singolo: invio ad un determinato client


**Diagramma delle Classi server**
  App: 
    - server : ServerSocket  
    - socket : Socket 
    - thread : MioThread
    - clients :   ArrayList
    Funzioni : 
      - Invio singolo (mittente, destinatario)
      - Invio in broadcast (Mittente)
    
  MioThread : 
    - Run () 
    - input : BufferedReader
    - output : DataOutputStream


**Diagramma della Classi client**
// da fare



**Messaggi client** 
  - 1 : invio singolo
  - 2 : invio broadcast
  - d : disconnessione

**Messaggio server**
  - a : notifica connesione nuovo client
  - d : notifica disconnesione client   
