# LLR-Revival v6.0 Nova

**Compatible with Logos Bible Software® and Verbum®**

> A fully browser-based library explorer for Logos/Verbum — developed by Pastor Hermann Fritz (FeG Horb am Neckar, Germany) as a revival and major extension of Steve Clark's original *Logos Library Reporter* (2015).

---

## What is LLR-Revival?

LLR-Revival reads your local Logos/Verbum database and presents all your books in a clear, feature-rich web interface — running directly in the browser, locally, without any additional app installation. No cloud dependency, no subscription.

---

## Key Features

### 📚 Library Explorer
- Automatic categorization of 22,000+ books into 40+ theological categories
- Multiple view modes: Modern (categories + groups) and Bookshelf (visual cover view)
- Book cover display extracted directly from the Logos database
- One-click opening of any book in Logos/Verbum
- Epoch timeline with 15 historical epochs

### 🔍 Advanced Search
- Full-text search across all books (title, author, category, series, year)
- Category, author, epoch and language filters
- Theological theme search with AI expansion
- Fuzzy search for approximate matches
- AI-powered book recommendations (Groq, OpenRouter, Anthropic, Ollama)

### ✝️ Sermon Workshop
- **350+ pericopes** from OT, NT and Apocrypha (liturgical year filtered)
- Cross-book liturgical feast search (Advent → all Advent texts from all books)
- Word studies for Greek, Hebrew and Latin with direct Logos links
- Clementina Vulgata and Neo-Vulgata links for Latin terms
- Literature references with library search and fallback to best commentaries
- AI exegetical sermon outline in 4 languages (DE/EN/FR/ES)
- Parallel texts with "Open all" function
- OT Introductions / NT Introductions / Archaeology quick access
- Export as DOCX, notes per pericope
- Project folders for sermon preparation

### 🤖 AI Integration
- Book recommendations and sermon outlines via Groq, OpenRouter, Anthropic, Ollama
- Configurable with your own API key

### ☁️ Cloud Sync
- Free synchronization via GitHub Gist
- Auto-sync every 15 minutes, cross-device

### 📖 More Features
- Daily Bible verse (OT + NT + Latin) with direct Logos link
- 34 themes, Quote mode, Reading mode
- Work projects, Import/Export (PDF, DOCX, TXT, JSON)
- Mobile optimized (Android/iOS)

---

## Languages

| Language | Installer | Port |
|----------|-----------|------|
| 🇩🇪 German | `Win/DE/01-INSTALLIEREN-Doppelklick.py` | 8421 |
| 🇬🇧 English | `Win/EN/01-INSTALL-DoubleClick.py` | 8422 |
| 🇫🇷 French | `Win/FR/01-INSTALLER-DoubleClic.py` | 8423 |
| 🇪🇸 Spanish | `Win/ES/01-INSTALAR-DobleClick.py` | 8424 |

All four language versions can run simultaneously on different ports.

---

## System Requirements

- **Logos Bible Software** (v4–10) or **Verbum** — must have been started at least once
- **Python 3.6+**
- **Modern browser** (Brave, Chrome, Firefox, Edge, Safari)
- **Windows** (primary), macOS and Linux supported
- iOS/Android: works with a local web server app (e.g. KWS)

---

## Installation

```
1. Extract the ZIP file
2. Open your language folder (e.g. Win/EN/)
3. Double-click the installer (.py file)
4. Installer reads Logos database, categorizes books, extracts covers
5. Desktop shortcut created automatically
6. Browser opens at http://localhost:8422 (EN)
```

---

## Architecture

```
LLR-Revival-6.0/
├── LLR-Revival-6.0-EN.html     # Main entry point
├── server.py                    # Local Python web server
├── lazy-loader-v6.js            # On-demand module loader
├── data.js                      # Your library data (installer-generated)
├── sermons-data.js              # 350+ pericopes
├── ui-sermon.js                 # Sermon Workshop
├── ui-ai-recommend.js           # AI recommendations
├── classifier.js                # Book categorization engine
├── cloud-sync.js                # GitHub Gist sync
├── styles.css                   # 34 themes
├── covers/                      # Book covers
└── covers-mobile/               # WebP thumbnails for mobile
```

---

## Credits

- **Steve Clark** — Original author of Logos Library Reporter (2015)
- **Hermann Fritz** — Complete redevelopment and maintenance of LLR-Revival v3.0–v6.0
- **Anthropic Claude AI** — AI software

---

## License

Open source — free use for the global Logos community.  
**Not for sale.** This software is exclusively for free, non-commercial use.

---

- 📦 [GitHub Repository](https://github.com/joefritz2024/Logos-Library-Reporter-Revival---v6.0-Nova---revised-and-reorganized-into-a-modular-structure)
- 📚 [Logos Bible Software](https://www.logos.com)

> 🇩🇪 **Auf Deutsch:** [README.de.md](README.de.md)

---
*Logos Bible Software® is a registered trademark of Faithlife LLC. LLR-Revival is not an official Faithlife product.*
