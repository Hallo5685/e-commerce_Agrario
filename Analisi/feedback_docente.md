# Feedback Docente – Prenotazione Agrario

## Analisi dei Requisiti

### Prenotazione vs vendita (requisito principale)

Esplicitare nei requisiti che il sistema è un sistema di **prenotazione** e non di e‑commerce. Il pagamento e il ritiro dei prodotti avvengono **esclusivamente in sede**.
Lo stato “venduto” deve essere inteso come **prodotto prenotato/riservato**, ed è utilizzato ai fini della gestione delle scorte.

### Gestione delle scorte (requisito verificabile)

Specificare nei requisiti il comportamento del sistema nella gestione delle scorte:

* quando una quantità viene prenotata, deve essere considerata **impegnata**;
* il sistema deve gestire correttamente **prenotazioni concorrenti**;
* in caso di **mancato ritiro**, la quantità deve tornare disponibile secondo le regole definite.

### Gestione ordini: definizione degli stati

È necessario esplicitare nei requisiti gli stati della prenotazione/ordine e il loro significato, indicando in modo chiaro quali stati possono essere modificati dal sistema e quali manualmente da amministratore o collaboratore (ad esempio: Inviato, Preso in carico, Ritirato, Annullato).

### Ruoli e responsabilità: Amministratore vs Collaboratore

Nei requisiti è necessario chiarire in modo esplicito la distinzione tra il ruolo di Amministratore e quello di Collaboratore, specificando quali operazioni sono riservate esclusivamente all’amministratore e quali possono essere svolte dal collaboratore entro i permessi assegnati, definendo chiaramente il limite dei suoi poteri.

### Pagamento: requisito chiuso o decisione aperta

Nei requisiti è necessario chiarire in modo esplicito se la modalità di pagamento è una decisione già definita (pagamento esclusivamente in sede) oppure un requisito ancora aperto da validare con il cliente, mantenendo la scelta coerente in tutto il documento.

### Coerenza terminologica

Nei requisiti è necessario utilizzare una terminologia coerente e uniforme per indicare gli stessi concetti (ad esempio prenotazione/ordine, cliente/utente, venduto/prenotato), evitando l’uso di termini diversi per riferirsi alla stessa funzionalità.

### Separazione tra requisiti e soluzioni tecniche

Nei requisiti devono essere descritti esclusivamente i comportamenti e le funzionalità richieste al sistema, evitando riferimenti a tecnologie, plugin o soluzioni implementative, che devono essere trattati separatamente nell’Analisi Tecnica.

## Analisi Funzionale

### Ambito e livello dell’Analisi Funzionale

Nell’Analisi Funzionale è necessario descrivere il comportamento del sistema dal punto di vista degli utenti e dei ruoli, concentrandosi sulle funzionalità offerte e sui flussi logici, evitando riferimenti a tecnologie, plugin o soluzioni implementative.

### Attori e ruoli del sistema

Nell’Analisi Funzionale è necessario elencare in modo esplicito tutti gli attori del sistema (utente, amministratore, collaboratore, operatore agrario), chiarendo per ciascuno se interagisce direttamente con il sistema o se riceve solo comunicazioni esterne (ad esempio tramite email).

### Casi d’uso e flussi principali

Nell’Analisi Funzionale è necessario descrivere i principali casi d’uso del sistema per ciascun attore, illustrando i flussi fondamentali (ad esempio consultazione del catalogo, prenotazione, gestione del ritiro, gestione degli ordini) senza entrare nei dettagli implementativi.

### Stati e ciclo di vita della prenotazione

Nell’Analisi Funzionale è opportuno descrivere il ciclo di vita della prenotazione, indicando i possibili stati e le transizioni principali tra di essi, in modo coerente con quanto definito nei requisiti.

### Gestione delle eccezioni e dei casi limite

Nell’Analisi Funzionale è necessario considerare e descrivere i principali casi di eccezione e situazioni limite (ad esempio indisponibilità delle quantità, prenotazioni concorrenti, mancato ritiro), indicando il comportamento atteso del sistema in tali situazioni.

## Analisi Tecnica (valutazione indicativa)

### Coerenza tra requisiti, analisi funzionale e scelte tecnologiche

Nell’Analisi Tecnica è necessario motivare le scelte tecnologiche (CMS, plugin, database) in funzione dei requisiti e dei flussi descritti nell’Analisi Funzionale, evidenziando in modo chiaro la coerenza tra bisogno, funzionalità e soluzione implementativa.

### Schema logico dei dati (ER)

Nell’Analisi Tecnica è necessario includere uno schema logico dei dati (schema ER) che rappresenti le principali entità del sistema (ad esempio utenti, prodotti, prenotazioni, ordini) e le relative relazioni, in modo coerente con quanto descritto nei requisiti e nell’Analisi Funzionale.

### Gestione delle scorte e concorrenza

Nell’Analisi Tecnica è necessario descrivere come viene garantita la coerenza delle scorte in presenza di prenotazioni concorrenti, specificando la logica di aggiornamento delle quantità e i controlli previsti per evitare overbooking (ad esempio validazione in fase di conferma e aggiornamento atomico dello stock).

### Gestione degli stati e del ciclo di vita dell’ordine

Nell’Analisi Tecnica è opportuno descrivere come gli stati della prenotazione/ordine vengono gestiti a livello tecnico, indicando quali componenti del sistema ne consentono la modifica e come viene garantita la coerenza tra stato, pagamento e ritiro.

### Sicurezza, validazioni e gestione degli errori

Nell’Analisi Tecnica è opportuno indicare le principali misure di sicurezza e validazione adottate (autenticazione degli utenti, controllo degli accessi per ruolo, validazione dei dati inseriti) e come il sistema gestisce eventuali errori o situazioni anomale.

# Feedback Project Plan e Gantt

Il Project Plan mostra un miglioramento rispetto alla versione precedente e riflette meglio il lavoro effettivamente svolto dal gruppo. Sono presenti obiettivi, attività e un aggiornamento sullo stato del progetto, elementi che indicano un tentativo di pianificare e monitorare lo sviluppo nel tempo.

Tuttavia il documento mantiene ancora una struttura troppo narrativa. In diversi punti assomiglia più a una raccolta di appunti o a un diario di lavoro del gruppo che a un vero piano di gestione del progetto. Per rendere il Project Plan più chiaro e leggibile sarebbe opportuno organizzarlo in sezioni più distinte e riconoscibili.

In particolare dovrebbe emergere in modo più netto la separazione tra:
- obiettivi del progetto;
- attività da svolgere;
- milestone principali;
- organizzazione e gestione del lavoro;
- controllo dello stato di avanzamento.

Attualmente questi elementi sono presenti ma spesso risultano mescolati tra loro all’interno delle stesse parti del documento, rendendo meno immediata la comprensione della struttura del progetto.

Un ulteriore aspetto che può essere migliorato riguarda l’attenzione ai possibili rischi o criticità durante lo sviluppo (ad esempio ritardi nelle attività, dipendenze da informazioni esterne o problemi tecnici). Anche una breve sezione che identifichi i principali rischi e come il gruppo intende affrontarli contribuirebbe a rendere il Project Plan più completo e più vicino a un vero documento di pianificazione.

Nel complesso il documento mostra un buon passo avanti rispetto alla versione iniziale, ma può essere ulteriormente migliorato rendendo la struttura più ordinata e distinguendo con maggiore chiarezza le diverse componenti della pianificazione del progetto.
