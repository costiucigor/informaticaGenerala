# informaticaGenerala

Protocolul WebSocket („socket web”), descris în specificația RFC 6455, oferă posibilitatea de a face schimb de date între un browser și un server printr-o conexiune persistentă. Datele sunt transmise prin acesta în ambele direcții sub formă de „pachete”, fără întreruperea conexiunii și a solicitărilor HTTP suplimentare.

WebSocket este deosebit de bun pentru serviciile care au nevoie de comunicare constantă, 
cum ar fi jocurile online, piețele în timp real și așa mai departe.

Exemplu simplu
Pentru a deschide o conexiune web socket, trebuie să creăm un nou obiect WebSocket,
specificând protocolul special ws în url:

let socket = new WebSocket("exemplu");

Există și protocolul wss://, care folosește criptarea. Este ca HTTPS pentru socket-urile web.

preferă întotdeauna wss://
Protocolul wss:// nu numai că folosește criptarea, dar are și securitate sporită.

Acest lucru se datorează faptului că datele ws:// nu sunt criptate, vizibile pentru orice intermediar. Proxy-urile mai vechi nu știu despre WebSocket, ar putea vedea anteturi „ciudate” și închid conexiunea.
