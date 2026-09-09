# ClipTTS — User Manual

## The core concept

ClipTTS listens to your clipboard. Copy text from any app (browser, Obsidian, text editor, chat), and ClipTTS notices and brings itself to the foreground, ready to read it. You don't open anything, you don't remember hotkeys.

If the "bring to foreground on every copy" behavior bothers you, you can disable it from the tray icon menu.

You can also go further and turn on **autoplay**: copy a text, and ClipTTS reads it on its own — no need to open the interface or press PLAY. You don't even need the tray icon for this: just copy, and it speaks.

---

## Main buttons

### PLAY
Reads the text currently in your clipboard. If the clipboard is empty, nothing happens.

### STOP
Stops playback immediately.

### PAUSE
Pauses playback. When you press it again, playback resumes from the exact point where you stopped — at the end of a sentence.

### VIS
Opens a popup showing **everything** currently in your clipboard, exactly as ClipTTS will read it. Useful to check what's about to be read before pressing PLAY.

### MOD
Corrects the pronunciation of a single word on the fly. Select a field in the popup, type the correction (e.g., "Accento" becomes "Accentó"), and save. It also works with synonyms, acronyms, or completely unrelated words — useful if you want ClipTTS to read "NASA" as "Enne-A-Esse-A" or a name like "Marco" with a particular pronunciation.

### T=T
Opens the pronunciation dictionary. Here you can add permanent rules, or simply view and edit the ones you've saved with MOD.

### REC
**Records everything to WAV.** Unlike PLAY which just reads, REC accumulates each synthesis and saves them as a single audio file at the end. Press REC, then PLAY (or multiple PLAYs in sequence), and press REC again to finish and save the file. The file opens automatically in WavPlayer.

---

## Selections and controls

### Voice
Choose from the available voices. You can change it anytime, even during playback.

### Speed
Adjust the reading speed (default: 1.5x). Lower values slow down, higher values speed up.

### Language
ClipTTS supports 32 languages. Select the language of the text you're about to read. Change it freely while listening.

### Background
Customize the visual theme. 14 different themes are available. Pick the one you prefer.

### Words per group (default: 10)
Technical parameter that controls playback attack speed: the lower the number, the sooner audio starts after pressing Play. With the default value, playback starts in under 3 seconds, regardless of text length — running on CPU alone, no GPU required. Raise the value if you prefer smoother speech from the first group onward, at the cost of a slightly slower start.

---

## Special behaviors

### Drag and drop files
You can drag a file (.txt, .docx, .pdf) directly onto the ClipTTS window. The content is read automatically and copied to your clipboard. Works on any point of the interface.

### Empty clipboard
If your clipboard is empty, ClipTTS will show it clearly both on the interface and in the taskbar. Nothing happens if you press PLAY.

### Tray icon
When you minimize ClipTTS to the tray (bottom right corner), you can still control it from there: PLAY, STOP, PAUSE are available directly from the tray menu. Useful to keep listening without taking up screen space.

**A left click on the tray icon turns autoplay on or off.** A colored icon means autoplay is on; gray means it's off. With autoplay on, any text you copy is read immediately, automatically — one click controls everything, no need to open menus or windows.

---

## WavPlayer

When you finish a recording with REC, WavPlayer opens automatically with the file you just created.

**What you can do:**
- Play the audio file
- Adjust speed (0.9x, 1x, 1.1x, 1.2x, 1.4x — the same presets as ClipTTS, or freely on the timeline)
- Scrub (drag) the timeline to jump to any point
- REC files are saved forever in the Wav folder — you can listen to them anytime, even months later

---

## Where are my files?

The WAV files you generate are saved in the **Wav** folder, in the same location where you placed ClipTTS.exe. Press the **WAV** button on the interface to open that folder directly in Windows File Explorer.

Files are never deleted automatically — you manage them.

---

## Localization

ClipTTS automatically detects your Windows system language:
- **Italian** → interface in Italian
- **Other language** → interface in English

There's no manual selection. The TTS voice language (the "Language" dropdown) remains separate from the interface.

---

## Technical notes

- ClipTTS is **completely offline**. No data leaves your computer.
- Requires no installation. It's a single executable — click and go.
- All data (saved pronunciations, chosen theme, speed) stays on your computer.
- No accounts, logins, or internet connections needed after the first run.

---

**Questions?** If anything isn't clear, look at the buttons on the interface — every function is visible and straightforward.
