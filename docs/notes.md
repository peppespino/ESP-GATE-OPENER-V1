# Note Tecniche – ESP Gate Opener

Queste sono alcune informazioni utili sul progetto, sui componenti utilizzati e su come ottenere le migliori prestazioni quando si installa il sistema.


##  Telecomando BFT

- Il progetto funziona con **qualsiasi telecomando BFT**, indipendentemente dal modello.
- Sul telecomando vengono saldati due fili sottili ai contatti del pulsante che comanda l’apertura del cancello.
- Il relay simula una pressione del pulsante, quindi il comportamento resta identico a quello del telecomando originale.


##  Relay

- Tipo utilizzato: **Relay a 5V – 1 canale**
- I contatti utilizzati sono:
  - **COM**
  - **NO** (normalmente aperto)
- Il relay è alimentato direttamente dal 5V dell’ESP.


##  Microcontrollore (ESP)

- Modello utilizzato: **ESP8266**
- Funzionamento Wi-Fi identico a qualunque altro progetto ESPHome.
- Affidabile entro la distanza tipica di un normale dispositivo ESP collegato alla tua rete Wi-Fi domestica.


##  Copertura Wi-Fi

- L’ESP funziona bene finché si trova entro il raggio normale della tua rete Wi-Fi.
- È consigliabile verificare che il punto in cui installerai il dispositivo abbia una copertura adeguata.
- In caso di segnale debole, basta aggiungere un piccolo extender Wi-Fi vicino al cancello.


##  Posizionamento consigliato

Per garantire un’apertura affidabile del cancello:

- Posiziona il dispositivo **abbastanza vicino al cancello** da permettere al telecomando interno di comunicare correttamente.
- Ricorda che, anche se lo comandi via Wi-Fi, il telecomando BFT funziona come al solito:
  → se sei troppo lontano, non può inviare il segnale al cancello.
- Il dispositivo deve quindi trovarsi **nel raggio d’azione naturale del telecomando**.


##  Alimentazione consigliata

- Puoi alimentare tutto con un normale alimentatore USB da 5V.
- In alternativa, il progetto può funzionare anche tramite **powerbank**, utile nei casi in cui:
  - non c’è una presa di corrente nei pressi del cancello
  - vuoi fare un’installazione temporanea o nascosta

Se scegli il powerbank:
- utilizzane uno di buona capacità (es. 10.000 mAh o superiore)
- assicurati che possa erogare almeno **1A** stabilmente


##  Consigli finali

- Proteggi l’elettronica con una scatola stagno se la installi all’esterno.
- Mantieni corte le saldature sul telecomando (fili sottili e ben fissati).
- Se il relay scatta ma il cancello non si apre, significa che il dispositivo è **troppo lontano dal cancello**, proprio come succede con un telecomando usato da distante.
- Mantieni il firmware ESPHome aggiornato per migliore stabilità.
