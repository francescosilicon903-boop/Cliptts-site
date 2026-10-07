# ClipTTS — Manuale Utente

## Il concetto fondamentale

ClipTTS ascolta la tua clipboard. Copi un testo da qualunque app (browser, Obsidian, editor di testo, chat), ClipTTS se ne accorge e torna in primo piano, pronto a leggerlo. Non devi aprire niente, non devi ricordare scorciatoie.

Se il comportamento di "torna in primo piano ad ogni copia" ti disturba, puoi disattivarlo dal menu tray icon.

Puoi anche andare oltre e attivare l'**autoplay**: copi un testo, e ClipTTS lo legge da solo — senza che tu debba aprire l'interfaccia né premere PLAY. Non serve nemmeno la tray icon per questo: basta copiare, e parla.

---

## I pulsanti principali

### PLAY
Legge il testo che è attualmente nella clipboard. Se la clipboard è vuota, non accade nulla.

### STOP
Interrompe la riproduzione istantaneamente.

### PAUSA
Mette in pausa la riproduzione. Quando ripremi, riprende dal punto esatto dove ti sei fermato — a fine frase.

### VIS
Apre un popup che mostra **tutto** il contenuto della clipboard, esattamente come lo leggerà ClipTTS — e puoi modificarlo lì dentro. Due pulsanti: "Salva negli appunti" (salva le modifiche nella clipboard, senza riprodurre) o "Riproduci" (salva e fa partire subito la lettura del testo corretto).

### MOD
Corregge la pronuncia di una singola parola al volo. **Copia la parola** (non serve aprire nessuna finestra apposta), poi premi MOD: si apre un popup già precompilato con quella parola, cursore pronto subito dopo il segno "=" per scrivere la correzione (es. "Accento" diventa "Accentó"). Premi Invio o clicca Salva. Se avevi copiato più di una parola, MOD prende solo la prima. Funziona anche con sinonimi, acronimi, o parole che non c'entrano nulla — utile se vuoi che ClipTTS legga "NASA" come "Enne-A-Esse-A" o un nome come "Marco" con una pronuncia particolare.

### T=T
Apre il dizionario delle pronunce. Qui puoi aggiungere regole permanenti, oppure semplicemente guardare e modificare quelle che hai già salvato con MOD.

### REC
**Registra tutto in WAV, in un solo passaggio.** Copia il testo che vuoi registrare, poi premi REC una volta sola: ClipTTS sintetizza l'intero testo in silenzio, in background — non lo senti mentre genera. Al termine, salva automaticamente il file e apre WavPlayer da solo.

Se premi REC di nuovo **mentre sta ancora generando**, annulli l'intera registrazione: non viene salvato nulla.

Accanto al file WAV, ClipTTS salva anche un file di testo gemello con lo stesso nome, contenente il testo originale — utile per ritrovare di cosa parlava una registrazione senza doverla riascoltare.

---

## Selezioni e controlli

### Voce
Scegli tra le voci disponibili. Puoi cambiarla in qualunque momento, anche durante la riproduzione.

### Velocità
Regola la velocità di lettura (default: 1.2x). Valori più bassi rallentano, più alti accelerano.

### Lingua
ClipTTS supporta 31 lingue. Seleziona quella del testo che stai per far leggere. Cambia pure mentre stai ascoltando.

### Sfondo
Personalizza il tema visivo. Sono disponibili 14 temi diversi. Scegli quello che preferisci.

### Parole per gruppo (default: 10)
Parametro tecnico che controlla la velocità di attacco della riproduzione: più basso è il numero, prima parte l'audio dopo aver premuto Play. Con il valore predefinito parte in meno di 3 secondi, indipendentemente dalla lunghezza del testo — girando solo su CPU, nessuna GPU richiesta. Alza il valore se preferisci un discorso più fluido fin dal primo gruppo, a scapito di un attacco leggermente più lento.

---

## Comportamenti speciali

### Trascinamento file
Puoi trascinare direttamente un file sulla finestra di ClipTTS. Il contenuto viene letto automaticamente e copiato nella clipboard. Funziona su qualunque punto dell'interfaccia.

Formati supportati: **.docx**, **.pdf**, e testo piano in tutte le sue varianti comuni — **.txt, .md, .markdown, .csv, .log, .json, .py, .js, .html, .htm, .xml, .yaml, .yml, .ini, .cfg, .srt**. File di codice, sottotitoli, configurazioni: se è testo leggibile, ClipTTS lo apre.

Il pulsante PLAY lampeggia brevemente di verde se il file è stato letto correttamente, di rosso se qualcosa è andato storto — senza popup che interrompono quello che stai facendo.

### Clipboard vuota
Se la clipboard è vuota, ClipTTS lo mostrerà chiaramente sia sull'interfaccia che nella barra dell'applicazione. Non accade nulla se premi PLAY.

### Tray icon
Quando minimizzi ClipTTS nel tray (angolo in basso a destra), puoi ancora controllarlo da lì: PLAY, STOP, PAUSA sono disponibili direttamente dal menu del tray. Utile per continuare l'ascolto senza occupare spazio sullo schermo.

**Un click sinistro sulla tray icon accende o spegne l'autoplay.** L'icona a colori significa autoplay attivo; grigia significa spento. Con l'autoplay acceso, ogni testo che copi viene letto subito, in automatico — un solo click controlla tutto, senza bisogno di aprire menu o finestre.

Spegnendo l'autoplay con quel click, ClipTTS interrompe **subito** anche una lettura in corso in quel momento — non aspetta che finisca. Un solo click ferma tutto e disattiva insieme.

Se hai una registrazione REC in corso, l'autoplay viene ignorato del tutto: copiare un nuovo testo non interrompe né riavvia la registrazione.

**Avvia con Windows**: dal menu della tray icon puoi attivare l'avvio automatico di ClipTTS ad ogni accesso a Windows. Non servono permessi da amministratore. Disponibile solo nella versione scaricata dal sito, non eseguendo il programma da codice sorgente.

---

## WavPlayer

Quando termini una registrazione con REC, WavPlayer si apre automaticamente con il file appena creato.

**Cosa puoi fare:**
- Riprodurre il file audio
- Regolare la velocità (0.9x, 1x, 1.1x, 1.2x, 1.4x — gli stessi preset di ClipTTS, oppure libera sulla timeline)
- Scrubbare (trascinare) sulla timeline per andare a qualunque punto
- I file REC vengono salvati per sempre nella cartella Wav — puoi riascoltarli quando vuoi, perfino mesi dopo

---

## Dove sono i miei file?

I file WAV che generi sono salvati nella cartella **Wav**, nella stessa posizione dove hai messo ClipTTS.exe. Premi il tasto **WAV** sull'interfaccia per aprire quella cartella direttamente da Esplora File di Windows.

I file non vengono mai cancellati automaticamente — li gestisci tu.

---

## Localizzazione

ClipTTS parte in **inglese** di default. Per cambiarla, apri il menu della tray icon → **Lingua interfaccia** → scegli English o Italiano. La scelta resta salvata per le volte successive.

Questa è la lingua dell'*interfaccia* (pulsanti, popup). La lingua della voce TTS (il dropdown "Lingua" nella finestra principale) è del tutto separata e non cambia insieme a questa.

---

## Licenza

Al primo avvio serve internet una sola volta: inserisci la chiave `CLIP-...` ricevuta via email e premi **Attiva** (nel campo funziona anche il tasto destro → Incolla). Se la chiave è giusta vedi `✓ Licenza attiva` e il programma parte.

Il tastino **LIC** in alto a destra (simmetrico a VIS) apre il pannello licenza: mostra a chi è intestata (nome/email), il prodotto (1 PC o 3 PC), la chiave mascherata e la data dell'ultima verifica. Tre bottoni:

- **Riprova**: forza subito una validazione (utile dopo aver liberato uno slot dal portal).
- **Cambia chiave**: libera lo slot della chiave attuale (serve internet) e ne chiede una nuova.
- **Disattiva su questo PC**: libera lo slot (1/3 PC) per spostare il programma — la chiave resta valida. Chiede conferma; dopo la disattivazione ClipTTS si chiude e alla prossima apertura chiede una chiave.

Ad ogni avvio ClipTTS valida la licenza in silenzio. Senza rete parte comunque se l'ultima verifica è entro 30 giorni, altrimenti chiede di collegarti. Se i posti sono finiti (es. stessa chiave 1 PC su un secondo computer) dice `Limite attivazioni raggiunto`: libera un PC dal customer portal Polar e poi riprova ad attivare.

Chiave persa? Riscaricala dall'email di acquisto o dalla tua pagina purchases di Polar — resta lì per sempre. Cambio PC? Premi Disattiva sul vecchio prima di attivare il nuovo.

### Antivirus / falsi positivi
ClipTTS è un programma nuovo e poco diffuso, quindi alla prima apertura Windows SmartScreen o qualche antivirus può mostrare un avviso (un falso positivo): il programma legge la clipboard e resta nel tray, e questo comportamento viene spesso segnalato per prudenza. Non c'è nulla di pericoloso.
- **SmartScreen:** clicca **Ulteriori informazioni** → **Esegui comunque**.
- **Antivirus:** aggiungi la cartella di ClipTTS alle esclusioni (o ripristina il file dalla quarantena). Se vuoi, puoi segnalare il file al produttore dell'antivirus come falso positivo.
- Scarica ClipTTS solo dal link ufficiale che ricevi con l'acquisto. La sintesi vocale resta tutta offline; internet serve solo per la licenza.

---

## Note tecniche

- La sintesi vocale è **completamente offline**: nessun testo esce dal tuo computer.
- Solo la licenza usa internet: attivazione (una volta) e validazione silenziosa ad ogni avvio, con 30 giorni di tolleranza offline.
- Non richiede installazione. È un unico eseguibile — clicca e va.
- Tutti i dati (pronuncie salvate, tema scelto, velocità) rimangono nel tuo computer.
- Non ci sono account, login, o connessioni internet necessarie dopo il primo avvio.

---

**Domande?** Se qualcosa non è chiaro, controlla i pulsanti sull'interfaccia — ogni funzione è ben visibile e immediata.

Sito: [https://fabricsoftware.dev](https://fabricsoftware.dev)
Contatti: [support@fabricsoftware.dev](mailto:support@fabricsoftware.dev)

---

Motore vocale: Supertonic 3 © Supertone, Inc. — MIT License (modello open-weight: https://huggingface.co/Supertone/supertonic-3).
