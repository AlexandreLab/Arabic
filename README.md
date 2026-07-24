# Majlis — Arabic (Weeks 1–4)

A single-file web app for learning the basics of Gulf Arabic. No build step, no
dependencies — just open `index.html` in a browser.

## Features

- **Letters** — the 28 letters grouped by shape family, with the four written
  forms (isolated / initial / medial / final), audio, and record-yourself.
- **Flashcards** — survival vocabulary with a lightweight SM-2-style spaced
  repetition schedule.
- **Decode drill** — sound out real words letter by letter, then reveal.
- **Pronunciation lab** — listen & shadow, record & A/B compare against the
  reference voice, and an AI check using browser speech recognition
  (Chrome/Edge).
- **Progress** — day streak, letters known, cards due, and a Week 4 checkpoint.

## Usage

Open `index.html` directly, or serve the folder and visit it in a browser:

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

Serving over `http://localhost` (rather than opening the file directly) is
recommended so microphone access for recording and the AI check works reliably.

## Notes

- Progress is stored in the browser's `localStorage` — same browser + same
  location keeps your data. Use **Export progress** to back it up.
- Text-to-speech and speech recognition depend on the browser; the pronunciation
  AI check works best in Chrome or Edge.
