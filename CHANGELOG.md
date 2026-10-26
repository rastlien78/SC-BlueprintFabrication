# Novità

Tutte le modifiche di rilievo, versione per versione. Gli eseguibili si scaricano dalla
pagina [Releases](https://github.com/rastlien78/SC-BlueprintFabrication/releases).

## [1.1.1] — 2026-10-26

### Corretto
- **Windows**: su alcuni PC (in particolare con Windows installato da poco) il primo avvio
  non riusciva a scaricare i dati di gioco e mostrava «mancano i dati di gioco». L'app ora
  include i certificati di sicurezza necessari per collegarsi a GitHub.
- Se il download dei dati non riesce, la finestra d'errore spiega **il motivo** (nessuna
  connessione, certificato non riconosciuto, cartella non scrivibile, limite di GitHub).

## [1.1.0] — 2026-10-26

### Nuovo
- **Supporto Linux**: eseguibile nativo, con ricerca automatica del `Game.log` nei prefissi
  Wine, Lutris e Steam/Proton.
- **Svuota inventario**, con richiesta di conferma.
- **Ricalcola** spostato nella barra di stato, con scorciatoia **F5**.
- Menu con il **tasto destro** su Blueprint e Risultati.

### Migliorato
- Barre azioni riorganizzate: una per pannello, con le azioni meno frequenti nei menu a
  tendina (Spunte ▾, Possedute ▾, Altro ▾).
- Le finestre secondarie (guida «?», Localizza, Simula, Lista mancanti, Pool missioni)
  funzionano a interruttore: un secondo click le chiude e ne resta aperta una sola per tipo.
- Togliendo moduli dai risultati, spariscono dal magazzino i materiali a quantità 0 non più
  usati da nessun modulo.
- Dati di gioco aggiornati alla **patch 4.10.2**, con le nuove blueprint dell'armatura
  **Monolith** (anche Shadowflux) e della **F55 «Shadowflux» LMG**.
- Interfaccia basata su Qt for Python (PySide6).

### Corretto
- Linux/Wayland: i filtri multi-selezione si richiudevano subito dopo l'apertura.

## [1.0.0] — 2026-06-12

Prima versione.

- Inventario materiali con qualità a livelli estraibili e scorte multiple.
- Oltre 1500 blueprint craftabili con ricerca, filtri multi-selezione e badge «craftabile ora».
- Risultati con Voluti/Reali, materiali condivisi, priorità di consumo e Lista mancanti.
- Caratteristiche finali per variante, simulazione della qualità e tasto Craft.
- **Localizza**: dove minare ogni materiale, con resa e fasce colorate.
- Import delle blueprint possedute dai `Game.log`, pool missioni, esportazione CSV.
- Aggiornamento automatico dei dati di gioco all'avvio e splash screen.

[1.1.1]: https://github.com/rastlien78/SC-BlueprintFabrication/releases/tag/v1.1.1
[1.1.0]: https://github.com/rastlien78/SC-BlueprintFabrication/releases/tag/v1.1.0
