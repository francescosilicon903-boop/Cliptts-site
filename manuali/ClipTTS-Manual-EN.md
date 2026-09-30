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
Opens a popup showing **everything** currently in your clipboard, exactly as ClipTTS will read it — and you can edit it right there. Two buttons: "Save to clipboard" (saves your edits to the clipboard, without playing) or "Play" (saves and immediately reads the corrected text).

### MOD
Corrects the pronunciation of a single word on the fly. **Copy the word** (no need to open any window first), then press MOD: a popup opens already filled in with that word, cursor placed right after the "=" sign ready for your correction (e.g., "Accento" becomes "Accentó"). Press Enter or click Save. If you had more than one word copied, MOD only takes the first one. It also works with synonyms, acronyms, or completely unrelated words — useful if you want ClipTTS to read "NASA" as "Enne-A-Esse-A" or a name like "Marco" with a particular pronunciation.

### T=T
Opens the pronunciation dictionary. Here you can add permanent rules, or simply view and edit the ones you've saved with MOD.

### REC
**Records to WAV in a single step.** Copy the text you want recorded, then press REC once: ClipTTS synthesizes the whole text silently, in the background — you won't hear it as it generates. When done, it saves the file automatically and opens WavPlayer on its own.

Pressing REC again **while it's still generating** cancels the whole recording: nothing gets saved.

Alongside the WAV file, ClipTTS also saves a twin text file with the same name, containing the original text — handy for finding out what a recording was about without listening to it again.

---

## Selections and controls

### Voice
Choose from the available voices. You can change it anytime, even during playback.

### Speed
Adjust the reading speed (default: 1.2x). Lower values slow down, higher values speed up.

### Language
ClipTTS supports 31 languages. Select the language of the text you're about to read. Change it freely while listening.

### Background
Customize the visual theme. 14 different themes are available. Pick the one you prefer.

### Words per group (default: 10)
Technical parameter that controls playback attack speed: the lower the number, the sooner audio starts after pressing Play. With the default value, playback starts in under 3 seconds, regardless of text length — running on CPU alone, no GPU required. Raise the value if you prefer smoother speech from the first group onward, at the cost of a slightly slower start.

---

## Special behaviors

### Drag and drop files
You can drag a file directly onto the ClipTTS window. The content is read automatically and copied to your clipboard. Works on any point of the interface.

Supported formats: **.docx**, **.pdf**, and plain text in all its common forms — **.txt, .md, .markdown, .csv, .log, .json, .py, .js, .html, .htm, .xml, .yaml, .yml, .ini, .cfg, .srt**. Code files, subtitles, config files: if it's readable text, ClipTTS opens it.

The PLAY button briefly flashes green if the file was read correctly, red if something went wrong — no popups interrupting what you're doing.

### Empty clipboard
If your clipboard is empty, ClipTTS will show it clearly both on the interface and in the taskbar. Nothing happens if you press PLAY.

### Tray icon
When you minimize ClipTTS to the tray (bottom right corner), you can still control it from there: PLAY, STOP, PAUSE are available directly from the tray menu. Useful to keep listening without taking up screen space.

**A left click on the tray icon turns autoplay on or off.** A colored icon means autoplay is on; gray means it's off. With autoplay on, any text you copy is read immediately, automatically — one click controls everything, no need to open menus or windows.

Turning autoplay off with that click also stops any playback that's happening **right then** — it doesn't wait for it to finish. One click stops everything and turns it off together.

If a REC session is running, autoplay is ignored entirely: copying new text won't interrupt or restart the recording.

**Start with Windows**: from the tray icon menu, you can enable ClipTTS launching automatically every time you sign in to Windows. No administrator rights needed. Available only in the version downloaded from the site, not when running the program from source.

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

ClipTTS starts in **English** by default. To change it, open the tray icon menu → **Interface language** → choose English or Italiano. Your choice is saved for next time.

This is the *interface* language (buttons, popups). The TTS voice language (the "Language" dropdown in the main window) is entirely separate and doesn't change with this setting.

---

## Technical notes

- ClipTTS is **completely offline**. No data leaves your computer.
- Requires no installation. It's a single executable — click and go.
- All data (saved pronunciations, chosen theme, speed) stays on your computer.
- No accounts, logins, or internet connections needed after the first run.

---

**Questions?** If anything isn't clear, look at the buttons on the interface — every function is visible and straightforward.

Website: [https://fabricsoftware.dev](https://fabricsoftware.dev)
Contact: [support@fabricsoftware.dev](mailto:support@fabricsoftware.dev)
