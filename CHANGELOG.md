# Novità

Tutte le modifiche di rilievo, versione per versione. Gli eseguibili si scaricano dalla
pagina [Releases](https://github.com/rastlien78/SC-BlueprintFabrication/releases).

## [1.3.0] — 2026-10-29

### Nuovo
- **Gruppi di qualità nell'inventario**: un materiale con più qualità diverse diventa un
  gruppo con intestazione «▸ Nome · N qualità (Q min–max) · totale», compresso di default.
  Un clic lo apre o lo chiude; i gruppi aperti restano aperti al riavvio. Dal menu «Altro»
  si possono espandere o comprimere tutti insieme. L'intestazione si colora di rosso
  (manca qualcosa) o di verde (serve al modulo selezionato) anche da chiusa.
- **Qualità per slot**: nel dettaglio dei risultati c'è una riga per ogni slot della ricetta,
  con una tendina per scegliere quale qualità usare tra quelle che hai in quantità
  sufficiente. Come in gioco, slot diversi possono usare qualità diverse dello stesso
  materiale.
- **Colonna «Quantità»** nel dettaglio e nella Simulazione: quanto materiale usa ogni slot per
  un craft e, se ne crafti più di uno, anche il totale (es. «0.360 SCU (×3 = 1.080 SCU)»).

### Migliorato
- **«⇅ Ordina e unisci»** (prima «Ricalcola») ora sta nel pannello Inventario e diventa
  **rosso** quando ci sono righe con stesso materiale e stessa qualità da sommare. I
  conteggi dei craftabili restano automatici. Scorciatoia **F5** invariata.
- **«+ Aggiungi»** con una riga selezionata crea la nuova riga con lo stesso materiale e la
  stessa qualità: resta da inserire solo la quantità.
- **Import dai `Game.log`**: barra di avanzamento durante la lettura, numero di file letti nel
  riepilogo, avviso chiaro se non viene trovato nessun log e, se qualche file non si può
  leggere, l'elenco con il motivo.
- Dati di gioco aggiornati.

### Corretto
- Conteggio dei craft con quantità decimali: in certi casi ne veniva calcolato uno in meno.

## [1.2.0] — 2026-10-26

### Nuovo
- **Avviso di nuova versione**: all'avvio l'app controlla se è uscito un aggiornamento e, se
  c'è, mostra una finestra con le novità e il link per scaricarlo. Con la casella «Non
  avvisarmi più per questa versione» l'avviso non ricompare fino alla versione successiva.
  Senza connessione il controllo viene saltato senza disturbare.

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

[1.3.0]: https://github.com/rastlien78/SC-BlueprintFabrication/releases/tag/v1.3.0
[1.2.0]: https://github.com/rastlien78/SC-BlueprintFabrication/releases/tag/v1.2.0
[1.1.1]: https://github.com/rastlien78/SC-BlueprintFabrication/releases/tag/v1.1.1
[1.1.0]: https://github.com/rastlien78/SC-BlueprintFabrication/releases/tag/v1.1.0
