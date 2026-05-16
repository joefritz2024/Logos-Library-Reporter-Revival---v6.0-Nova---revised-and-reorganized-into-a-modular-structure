# LLR-Revival v6.0 Nova

**Kompatibel mit Logos Bible Software® und Verbum®**

> Ein vollständiger Browser-basierter Bibliotheks-Explorer für Logos/Verbum — entwickelt von Pastor Hermann Fritz (FeG Horb am Neckar) als Fortführung und Weiterentwicklung von Steve Clarks *Logos Library Reporter* (2015).

---

## Was ist LLR-Revival?

LLR-Revival liest die lokale Logos/Verbum-Datenbank aus und stellt alle eigenen Bücher in einer übersichtlichen, multifunktionalen Web-Oberfläche dar — direkt im Browser, ohne Installation einer weiteren App. Die Anwendung läuft vollständig lokal, ohne Cloud-Abhängigkeit.

---

## Hauptfunktionen

### 📚 Bibliotheks-Explorer
- Automatische Kategorisierung von 22.000+ Büchern in **40+ theologische Kategorien**
- Mehrere Ansichtsmodi: Modern (Kategorien + Gruppen) und Bookshelf (visuelles Bücherregal)
- Buchcover-Anzeige aus der Logos-Datenbank (automatisch extrahiert)
- Direktes Öffnen jedes Buches in Logos/Verbum per Klick
- Epoch-Timeline mit 15 historischen Epochen

### 🔍 Erweiterte Suche
- Volltextsuche über alle Bücher (Titel, Autor, Kategorie, Serie, Jahr)
- Kategorie-Filter, Autoren-Filter, Epochen-Filter
- Theologische Themen-Suche
- Fuzzy-Suche für unscharfe Treffer
- KI-gestützte Buchempfehlungen (Groq, OpenRouter, Anthropic, Ollama)

### ✝️ Predigt-Werkstatt
- **350+ Perikopen** aus AT, NT und Apokryphen (Kirchenjahr-gefiltert)
- Buchübergreifende Kirchenfest-Suche (Advent → alle Advent-Texte aus allen Büchern)
- Wortstudien zu Griechisch, Hebräisch und Latein mit direktem Öffnen in Logos
- Clementina Vulgata und Neo-Vulgata Verknüpfung bei lateinischen Texten
- Literaturverweise mit Bibliothekssuche und Fallback auf beste Kommentare
- KI-exegetische Gliederung (Groq/OpenRouter/Anthropic/Ollama) — 4-sprachig
- Paralleltexte (Konzept-Matching) mit „Alle öffnen"-Funktion
- AT-Einleitungen / NT-Einleitungen / Archäologie — Direktzugriff
- Export als DOCX
- Notizfunktion (perikopen-bezogen, mit Export)
- Projektmappen: Bücher, Notizen und Zitate für Predigtvorbereitung bündeln

### 🤖 KI-Integration
- Buchempfehlungen via KI (Groq, OpenRouter, Anthropic, Ollama)
- KI-exegetische Predigtgliederung in DE/EN/FR/ES
- Konfigurierbar mit eigenem API-Key

### ☁️ Cloud-Sync
- Synchronisation über GitHub Gist (kostenlos)
- Auto-Sync alle 15 Minuten
- Geräteübergreifend: Desktop ↔ Tablet ↔ Smartphone

### 📖 Weitere Features
- Tages-Bibelvers (AT + NT + Latein) mit Direktlink in Logos
- Zitate-Modus, Lese-Modus
- Arbeitsprojekte mit Bücherlisten, Notizen, Zitaten
- Import/Export (PDF, DOCX, TXT, JSON)
- Google Drive Sync
- 34 Themes (Aurora, Kloster, Nordisch, Papyrus u.v.m.)
- Lese-Fortschritt-Tracking
- Verlauf der geöffneten Bücher
- Persönliche Bücher (Logos Personal Books)
- Mobile-optimiert (Android/iOS mit lokalem Webserver)

---

## Sprachen

| Sprache | Installer |
|---------|-----------|
| 🇩🇪 Deutsch | `Win/DE/01-INSTALLIEREN-Doppelklick.py` |
| 🇬🇧 English | `Win/EN/01-INSTALL-DoubleClick.py` |
| 🇫🇷 Français | `Win/FR/01-INSTALLER-DoubleClic.py` |
| 🇪🇸 Español | `Win/ES/01-INSTALAR-DobleClick.py` |

Die Benutzeroberfläche ist vollständig in allen 4 Sprachen übersetzt (i18n-System).

---

## Systemvoraussetzungen

- **Logos Bible Software** (Version 4–10) oder **Verbum** — muss mindestens einmal gestartet worden sein
- **Python 3.6+** (für den Installer und lokalen Server)
- **Moderner Browser** (Brave, Chrome, Firefox, Edge, Safari)
- **Windows** (primär), macOS und Linux werden unterstützt
- iOS/Android: funktioniert mit lokalem Webserver-App (KWS, Simple HTTP Server)

---

## Installation

```
1. ZIP-Datei entpacken
2. Gewünschte Sprachversion öffnen (z.B. Win/DE/)
3. 01-INSTALLIEREN-Doppelklick.py doppelklicken
4. Installer liest Logos-Datenbank, kategorisiert Bücher, extrahiert Cover
5. Desktopverknüpfung wird automatisch erstellt
6. Browser öffnet sich automatisch auf http://localhost:8421
```

---

## Architektur

LLR-Revival v6.0 ist modular aufgebaut (28+ JavaScript-Module):

```
LLR-Revival-6.0/
├── LLR-Revival-6.0-DE.html     # Hauptdatei (Einstiegspunkt)
├── server.py                    # Lokaler Python-Webserver (Port 8421)
├── lazy-loader-v6.js            # Modularer On-Demand-Loader
├── data.js                      # Bibliotheksdaten (vom Installer generiert)
├── sermons-data.js              # Perikopen-Daten (350+ Texte)
├── ui-sermon.js                 # Predigt-Werkstatt
├── ui-ai-recommend.js           # KI-Buchempfehlungen
├── ui-docs.js                   # Arbeitsprojekte
├── ui-bookops.js                # Bibliothekssuche
├── classifier.js                # Buch-Kategorisierung
├── cloud-sync.js                # GitHub Gist Sync
├── styles.css                   # 34 Themes
├── covers/                      # Buchcover (vom Installer extrahiert)
└── covers-mobile/               # WebP-Thumbnails für Mobilgeräte
```

---

## Kategorien (Auswahl)

Bibel & Bibelwörterbücher · Kommentare · Kirchengeschichte · Theologie & Dogmatik · Biblische Sprachen · Systematische Theologie · Homiletik & Predigt · Hermeneutik & Auslegung · Apologetik & Weltanschauung · Archäologie & Geschichte Israels · Biblische Theologie · Altes Testament · Neues Testament · Mission & Evangelisation · Seelsorge · Eschatologie · Ethik · Biografien · Lexika & Wörterbücher · Nachschlagewerke · I. Journale & Magazine · II. Kleine Buch- & Journalreihen · Landkarten & Atlanten · Persönliche Bücher · Personen der Bibel & Kirchengeschichte · Early American History · und weitere

---

## Entwicklung

LLR-Revival begann als Einzeldatei-Applikation und wurde über Hunderte von Revisionen zur heutigen modularen v6.0-Architektur weiterentwickelt.

**Entwickler:** Pastor Hermann Fritz (FeG Horb am Neckar, Baden-Württemberg) mit Claude AI (Anthropic)  
**Ursprung:** Basiert auf Steve Clarks *Logos Library Reporter* (2015)  
**Lizenz:** Open Source — freie Nutzung für die weltweite Logos-Community

---

## Credits

- **Steve Clark** — Ursprünglicher Autor des Logos Library Reporter (2015)
- **Hermann Fritz** — Komplette Neuentwicklung, Erweiterung und Pflege von LLR-Revival v3.0–v6.0
- **Anthropic Claude AI** — KI-Software

---

## Links

- 📦 [GitHub Repository](https://github.com/joefritz2024/Logos-Library-Reporter-Revival---v6.0-Nova---revised-and-reorganized-into-a-modular-structure)
- 📚 [Logos Bible Software](https://www.logos.com)
- ⛪ [FeG Horb am Neckar](https://feg-horb.de)

---

*LLR-Revival ist kein offizielles Produkt von Faithlife/Logos. Logos Bible Software® ist ein eingetragenes Warenzeichen von Faithlife LLC.*
