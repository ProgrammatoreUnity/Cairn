# CAIRN

**Software pensato per darti tutti gli strumenti necessari per progettare la tua idea.**

[English version](README.md)

Cairn è un'app per Windows che tiene in un unico posto tutto ciò che riguarda un progetto: le cose da fare, il piano nel tempo, i tuoi schizzi e i tuoi appunti. Funziona completamente offline. Non c'è cloud, non c'è server e non c'è account online: il tuo lavoro resta sul tuo PC.

## Per iniziare

1. Fai clic destro su `Cairn.exe` e scegli **Esegui come amministratore**. Cairn ha bisogno dei permessi di amministratore per funzionare. Non c'è nulla da installare.
2. La prima volta Cairn ti chiede di creare un account: scegli **Username** e **Password**. Vedi [Account](#account) più sotto.
3. Clicca **New Project**, dai un nome al progetto e aprilo con un doppio clic.

Tutto quello che fai viene salvato in automatico. Non c'è nessun pulsante Salva da ricordare.

L'interfaccia dell'app è in inglese: in questa guida i termini usati nell'app sono riportati in inglese, come appaiono sullo schermo.

## Il menù principale

La prima schermata è l'elenco dei tuoi progetti. Da qui puoi creare un progetto, aprirlo, cambiarne le impostazioni (**Settings**) o eliminarlo (**Delete**).

**Open Folder…** aggiunge un progetto che esiste già sul tuo disco, per esempio uno che un collega ha condiviso con te.

## Dentro un progetto

Un progetto ha tre aree. Passi dall'una all'altra dalla parte alta della finestra o dal menù **View**.

### Kanban board

La board mostra le tue attività come card, disposte in colonne come *TODO*, *In Progress* e *Done*.

- Aggiungi una card per ogni cosa da fare.
- Trascina una card in un'altra colonna quando il suo stato cambia.
- Aggiungi, rinomina, ricolora o rimuovi le colonne per adattarle al tuo modo di lavorare.
- Manda le card completate nell'**Archive** per tenere la board in ordine.

Apri una card per aggiungere i dettagli:

- **Description**, **Assignee**, **Priority** e **Tags**
- **Checklist** e **Subtasks**, con un cerchio che mostra quanto è stato completato
- le date: **Start**, **Due**, **End** e **Finish**
- i **Comments**
- i **References**, cioè i collegamenti ai documenti del progetto

Ogni card conserva anche la cronologia delle sue modifiche (**Activity**). Le modifiche a una card vengono applicate solo quando premi **Save**.

Usa i filtri e la casella di ricerca per vedere solo le card che ti interessano, per esempio solo le tue o solo quelle urgenti. Cairn ti avvisa anche quando un'attività è scaduta o vicina alla scadenza.

### Roadmap

La roadmap si apre in una finestra a parte e mostra le tue attività su una linea del tempo, così vedi cosa succede e quando.

- Le attività che hanno delle date appaiono come barre, raggruppate per tag.
- Aggiungi le **Milestones** per segnare i momenti importanti, ognuna con la sua icona.
- Aggiungi attività che esistono solo nella roadmap.
- Guarda un singolo mese, un anno intero, oppure usa la **Free View** con zoom da 7 giorni a 2 anni.

### Whiteboard

Uno spazio libero per disegnare le idee e collegarle tra loro.

- Aggiungi forme, testi, disegni e immagini, poi uniscili con i connectors.
- Collega un elemento a un'attività o a un documento.
- Segna come **Favorites** gli elementi importanti.
- Crea tutte le whiteboard che ti servono all'interno di un progetto.
- **Undo** e **Redo** sono sempre disponibili.

### Documentation

Il posto per la parte scritta del tuo progetto.

- Scrivi semplici note in **Markdown** oppure pagine formattate in **Rich Text**, con font, colori, elenchi e immagini.
- Organizza i documenti in cartelle.
- Collega i documenti tra loro. La **graph view** mostra come sono connessi.
- Un documento eliminato finisce nella cartella cestino del progetto, che puoi aprire con **Trash Folder** dal menù principale. Cairn non la svuota mai da solo.

### Pomodoro timer

Un timer nella parte alta della finestra ti aiuta a lavorare in sessioni concentrate con brevi pause. Ogni progetto ha le proprie impostazioni del timer.

## Account

Un account in Cairn è soltanto un nome, un colore e (se vuoi) un'immagine. Vive sul tuo PC: nulla viene inviato online e non serve una connessione a internet.

**Perché registrare un account?** Perché permette a Cairn di mostrare *chi ha fatto cosa*. È utile quando più persone lavorano allo stesso progetto:

- **Più persone sullo stesso PC.** Ognuno ha il proprio account. Si cambia dal menù in alto a destra (**Switch Account**).
- **Un progetto condiviso con altre persone.** Ogni collega usa il proprio account sul proprio PC, e il progetto conserva l'elenco delle persone che ci lavorano.

In entrambi i casi le attività si possono assegnare a una persona, i commenti sono firmati e la cronologia di ogni card mostra chi ha fatto ogni modifica.

**Lavori da solo?** Allora l'account è solo una formalità. Creane uno la prima volta con username e password qualsiasi: Cairn ti ricorda sul tuo PC e non te lo chiederà più.

**Il campo Email.** Puoi lasciarlo vuoto. Al momento l'email non viene usata in alcun modo: Cairn non invia messaggi e non la usa per recuperare la password.

## Dove sono i tuoi dati

Ogni progetto è una normale cartella sul tuo disco, fatta di file leggibili. Scegli la cartella quando crei il progetto, e il suo percorso è sempre visibile in basso a destra nella finestra mentre il progetto è aperto.

- **Backup:** copia la cartella.
- **Rete di sicurezza:** Cairn conserva gli ultimi 5 backup automatici di ogni board. Puoi ripristinarne uno dai **Project Settings**.

## Condividere un progetto con Git

Cairn non ha un sistema di condivisione o sincronizzazione integrato. Un progetto è solo una cartella, quindi puoi condividerlo con [Git](https://git-scm.com), come faresti con qualsiasi altra cartella di file. Ti servono Git installato e un posto dove ospitare il repository (per esempio GitHub o GitLab).

**Chi possiede il progetto:**

1. Apri un terminale nella cartella del progetto.
2. Trasformala in un repository e caricala:

   ```
   git init
   git add .
   git commit -m "Prima versione del progetto"
   git remote add origin <indirizzo del tuo repository>
   git push -u origin main
   ```

**Ogni collega:**

1. Scarica il progetto: `git clone <indirizzo del repository>`
2. In Cairn, nel menù principale, clicca **Open Folder…** e scegli la cartella scaricata.
3. La prima volta Cairn chiede come entrare nel progetto: unisciti con il tuo account, oppure fai **Login** come uno degli account già presenti.

**Giorno per giorno:**

1. Prima di iniziare a lavorare, scarica le ultime modifiche: `git pull`
2. Lavora in Cairn come al solito.
3. Quando hai finito, invia le tue modifiche:

   ```
   git add .
   git commit -m "Cosa ho cambiato"
   git push
   ```

**Consigli**

- Cairn non unisce le modifiche da solo. Se due persone modificano la stessa board nello stesso momento, Git può segnalare un conflitto. Fai pull spesso, fai push spesso e mettetevi d'accordo su chi lavora a cosa.
- Se fai pull mentre il progetto è aperto in Cairn, chiudi il progetto e riaprilo per vedere le nuove modifiche.
- Le password non vengono mai condivise in forma leggibile: il progetto ne conserva solo una versione protetta.

## Light e dark

Passa dal tema light al tema dark con il pulsante sole/luna in alto a destra, oppure con **View → Dark Mode**.

## Buono a sapersi

- Modificare un documento Markdown in modalità **Preview** lo riscrive nello stile Markdown di Cairn.
- Convertire una pagina Rich Text in Markdown fa perdere colori, font e allineamento.
- Le pagine Rich Text con molte immagini possono risultare lente durante la scrittura.
- Un collegamento a un file esterno smette di funzionare se quel file viene spostato.

## Requisiti

Windows a 64 bit.

## Crediti

Progettato e realizzato da Highshore Studio — highshore.studio@gmail.com

Icone delle milestone: [Ionicons](https://ionic.io/ionicons) (licenza MIT).
