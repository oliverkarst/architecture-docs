# KI-gestützte Architekturdokumentation mit arc42

Ein Lernprojekt für effektive Softwarearchitekturdokumentation mit Hilfe von KI-Tools (Vibe Coding).

## 🎯 Zielsetzung

Dieses Repository demonstriert, wie moderne KI-Tools (insbesondere Claude Code) effektiv für die Erstellung und Pflege von Architekturdokumentation eingesetzt werden können. Es nutzt das bewährte **arc42-Template** in Verbindung mit **docToolchain** für eine professionelle Dokumentations-Pipeline.

## 🏗️ Architektur-Übersicht

```
architecture-docs/
├── 📁 src/docs/arc42/          # Haupt-Architekturdokumentation
│   └── modules/ROOT/pages/     # arc42-Kapitel (1-12)
├── 📁 docs/                    # Zusätzliche Dokumentation
│   ├── vibe-coding-guidelines.adoc
│   └── prompts/                # KI-Prompt-Bibliothek
├── 📁 templates/               # Wiederverwendbare Templates
│   ├── adr-template.md
│   └── arc42-prompts-library.md
├── 📁 build/                   # Generierte Dokumentation
└── ⚙️ docToolchainConfig.groovy # Build-Konfiguration
```

## 🚀 Schnellstart

### Voraussetzungen
- **Docker** (für docToolchain)
- **Git** (für Versionierung)
- **KI-Tool** (z.B. Claude Code, ChatGPT)

### 1. Repository Setup
```bash
git clone <repository-url>
cd architecture-docs

# Dokumentation bauen
./dtcw generateSite

# Vorschau starten (lokal)
./dtcw previewSite
# → http://localhost:4000
```

### 2. Mit KI arbeiten
```bash
# Claude Code Konfiguration ist bereits vorhanden
# Siehe CLAUDE.md für projektspezifische Befehle

# Beispiel-Workflow:
# 1. Template aus templates/ wählen
# 2. KI-Prompt aus docs/prompts/ anpassen
# 3. Generierten Inhalt in arc42-Struktur integrieren
# 4. Build testen: ./dtcw generateSite
```

## 📚 Inhalte und Features

### ✅ Vollständige arc42-Struktur
- **Kapitel 1-12** mit deutschen Überschriften
- Beispielinhalte für KI-gestützte Dokumentation
- Integrierte Qualitätssicherung

### ✅ KI-Integration
- **Prompt-Bibliothek** für alle arc42-Kapitel
- **Best-Practice-Guidelines** für Vibe Coding
- **Template-System** für wiederkehrende Aufgaben

### ✅ Automatisierung
- **GitHub Actions** für automatisches Deployment
- **docToolchain** für konsistente Builds
- **Diagramm-Generierung** mit PlantUML

### ✅ Qualitätssicherung
- Link-Validierung und Syntax-Checks
- Konsistenz-Prüfung zwischen Kapiteln
- Review-Prozesse für KI-generierte Inhalte

## 🎓 Lernziele

Dieses Projekt lehrt:

### 1. **Effiziente Architekturdokumentation**
- arc42 als bewährter Standard
- Strukturiertes Vorgehen mit Templates
- Automatisierung repetitiver Aufgaben

### 2. **KI-gestütztes Arbeiten (Vibe Coding)**
- Prompt Engineering für Dokumentation
- Iterative Verfeinerung mit KI
- Qualitätskontrolle bei KI-Outputs

### 3. **Moderne Toolchain**
- docToolchain für Build-Automatisierung
- Git-basierte Workflows
- CI/CD für Dokumentation

### 4. **Collaboration & Review**
- Team-Workflows mit KI-Tools
- Review-Prozesse für Qualitätssicherung
- Knowledge Sharing und Best Practices

## 📖 Anwendungsbeispiele

### Beispiel 1: Neues Projekt starten
```bash
# 1. Repository als Template verwenden
# 2. Stakeholder-Analyse mit KI (Kapitel 1)
# 3. Kontextabgrenzung entwickeln (Kapitel 3)
# 4. Schrittweise alle arc42-Kapitel ausfüllen
```

### Beispiel 2: Bestehende Architektur dokumentieren
```bash
# 1. System-Analyse mit KI-Unterstützung
# 2. Reverse Engineering der Architektur
# 3. Diagramme und Beschreibungen generieren
# 4. ADRs für historische Entscheidungen erstellen
```

### Beispiel 3: Architektur-Review
```bash
# 1. Vollständigkeits-Check mit Meta-Prompts
# 2. Konsistenz-Prüfung zwischen Kapiteln  
# 3. Qualitätsziele vs. Implementierung abgleichen
# 4. Verbesserungsvorschläge ableiten
```

## 🛠️ Erweiterte Nutzung

### Custom Prompts entwickeln
```markdown
# Basis-Prompt aus docs/prompts/ nehmen
# Projekt-spezifisch anpassen
# In Team teilen und iterativ verbessern
```

### Template-Bibliothek erweitern
```bash
# Neue Templates in templates/ ablegen
# Dokumentation in README.md aktualisieren
# Best Practices dokumentieren
```

### Multi-Projekt-Setup
```bash
# Repository als Submodule in anderen Projekten
# Shared Templates und Prompts
# Zentrale Qualitätsstandards
```

## 📊 Metriken und Erfolg

### Quantitative Ziele
- **60% Zeitersparnis** bei Dokumentationserstellung
- **Konsistenz-Score > 90%** zwischen Kapiteln
- **Vollständigkeit > 95%** nach arc42-Standard

### Qualitative Ziele
- Bessere **Verständlichkeit** für alle Stakeholder
- **Nachvollziehbare** Architekturentscheidungen
- **Wartbare** und **erweiterbare** Dokumentation

## 🔄 Roadmap und Weiterentwicklung

### Phase 1: Foundation ✅
- [x] arc42-Setup mit docToolchain
- [x] KI-Prompt-Bibliothek
- [x] Template-System
- [x] GitHub Actions Pipeline

### Phase 2: Advanced Features (geplant)
- [ ] Mehrsprachige Templates
- [ ] Domain-spezifische Prompts (Web, Mobile, IoT)
- [ ] Integration mit PlantUML Server
- [ ] Automatisierte Diagramm-Synchronisation

### Phase 3: Community (geplant)  
- [ ] Community-Templates
- [ ] Plugin-System für verschiedene KI-Tools
- [ ] Metrics und Analytics Dashboard
- [ ] Workshops und Schulungsmaterialien

## 🤝 Beitragen und Feedback

### Issues und Verbesserungsvorschläge
- GitHub Issues für Bug-Reports
- Feature-Requests willkommen
- Best-Practice-Sharing erwünscht

### Community Guidelines
- **Konstruktives Feedback** zu Templates und Prompts
- **Erfahrungsaustausch** über KI-Tools
- **Qualitätsorientierte** Diskussionen

## 📚 Weiterführende Ressourcen

### Dokumentation
- [`CLAUDE.md`](CLAUDE.md) - Claude Code spezifische Konfiguration
- [`docs/vibe-coding-guidelines.adoc`](docs/vibe-coding-guidelines.adoc) - Detaillierte Arbeitsweise
- [`templates/README.md`](templates/README.md) - Template-Dokumentation

### Externe Links
- [arc42.org](https://arc42.org/) - arc42 Template Dokumentation
- [docToolchain](https://doctoolchain.org/) - Build-Tool für Dokumentation
- [PlantUML](https://plantuml.com/) - Diagramm-Generierung

## 📞 Support

**Maintainer:** @oliver  
**Projektstatus:** Active Development  
**Version:** 1.0.0  
**Letzte Aktualisierung:** Januar 2025

---

*Dieses Projekt demonstriert moderne Ansätze für Architekturdokumentation und ist als Lernobjekt und Referenz-Implementierung konzipiert.*