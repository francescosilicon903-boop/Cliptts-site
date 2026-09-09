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
Apre un popup che mostra **tutto** il contenuto della clipboard, esattamente come lo leggerà ClipTTS. Utile per controllare cosa sta per essere letto prima di premere PLAY.

### MOD
Corregge la pronuncia di una singola parola al volo. Seleziona un campo nel popup, scrivi la correzione (es. "Accento" diventa "Accentó"), e salva. Funziona anche con sinonimi, acronimi, o parole che non c'entrano nulla — utile se vuoi che ClipTTS legga "NASA" come "Enne-A-Esse-A" o un nome come "Marco" con una pronuncia particolare.

### T=T
Apre il dizionario delle pronunce. Qui puoi aggiungere regole permanenti, oppure semplicemente guardare e modificare quelle che hai già salvato con MOD.

### REC
**Registra tutto in WAV.** A differenza di PLAY che legge semplicemente, REC accumula ogni sintesi e le salva come un unico file audio al termine. Premi REC, quindi PLAY (o più PLAY consecutivi), e alla fine premi di nuovo REC per terminare e salvare il file. Il file si apre automaticamente in WavPlayer.

---

## Selezioni e controlli

### Voce
Scegli tra le voci disponibili. Puoi cambiarla in qualunque momento, anche durante la riproduzione.

### Velocità
Regola la velocità di lettura (default: 1.5x). Valori più bassi rallentano, più alti accelerano.

### Lingua
ClipTTS supporta 32 lingue. Seleziona quella del testo che stai per far leggere. Cambia pure mentre stai ascoltando.

### Sfondo
Personalizza il tema visivo. Sono disponibili 14 temi diversi. Scegli quello che preferisci.

### Parole per gruppo (default: 10)
Parametro tecnico che controlla la velocità di attacco della riproduzione: più basso è il numero, prima parte l'audio dopo aver premuto Play. Con il valore predefinito parte in meno di 3 secondi, indipendentemente dalla lunghezza del testo — girando solo su CPU, nessuna GPU richiesta. Alza il valore se preferisci un discorso più fluido fin dal primo gruppo, a scapito di un attacco leggermente più lento.

---

## Comportamenti speciali

### Trascinamento file
Puoi trascinare direttamente un file (.txt, .docx, .pdf) sulla finestra di ClipTTS. Il contenuto viene letto automaticamente e copiato nella clipboard. Funziona su qualunque punto dell'interfaccia.

### Clipboard vuota
Se la clipboard è vuota, ClipTTS lo mostrerà chiaramente sia sull'interfaccia che nella barra dell'applicazione. Non accade nulla se premi PLAY.

### Tray icon
Quando minimizzi ClipTTS nel tray (angolo in basso a destra), puoi ancora controllarlo da lì: PLAY, STOP, PAUSA sono disponibili direttamente dal menu del tray. Utile per continuare l'ascolto senza occupare spazio sullo schermo.

**Un click sinistro sulla tray icon accende o spegne l'autoplay.** L'icona a colori significa autoplay attivo; grigia significa spento. Con l'autoplay acceso, ogni testo che copi viene letto subito, in automatico — un solo click controlla tutto, senza bisogno di aprire menu o finestre.

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

ClipTTS rileva automaticamente la lingua del tuo sistema operativo Windows:
- **Italiano** → interfaccia in italiano
- **Altra lingua** → interfaccia in inglese

Non c'è scelta manuale. La lingua della voce TTS (il dropdown "Lingua") rimane separata dall'interfaccia.

---

## Note tecniche

- ClipTTS è **completamente offline**. Nessun dato esce dal tuo computer.
- Non richiede installazione. È un unico eseguibile — clicca e va.
- Tutti i dati (pronuncie salvate, tema scelto, velocità) rimangono nel tuo computer.
- Non ci sono account, login, o connessioni internet necessarie dopo il primo avvio.

---

**Domande?** Se qualcosa non è chiaro, controlla i pulsanti sull'interfaccia — ogni funzione è ben visibile e immediata.
