# Claude Code Konfiguration für Architecture-Docs

## Projektspezifische Befehle

### Build & Entwicklung
- **Build**: `./dtcw generateSite`
- **Preview**: `./dtcw previewSite` (lokaler Server auf port 4000)
- **Vollständige Dokumentation**: `./dtcw generateHTML generatePDF`
- **Nur HTML**: `./dtcw generateHTML`

### Linting & Qualitätssicherung
- **AsciiDoc Syntax Check**: Automatisch durch docToolchain
- **Link Check**: `./dtcw htmlSanityCheck`
- **Deploy Test**: `./dtcw generateSite && ls -la build/microsite/output`

### Arbeitsweise mit KI
Dieses Projekt nutzt arc42 + docToolchain für strukturierte Architekturdokumentation.

**Wichtige Pfade:**
- Hauptdokumentation: `src/docs/arc42/modules/ROOT/pages/`
- Bilder: `src/docs/arc42/modules/ROOT/assets/images/`
- Build-Output: `build/microsite/output/`
- Konfiguration: `docToolchainConfig.groovy`

**Vor Änderungen immer:**
1. Vorhandene Struktur analysieren
2. arc42-Konventionen befolgen
3. Deutsche Sprache verwenden
4. Build testen mit `./dtcw generateSite`

## Vibe Coding Best Practices

### 1. Iterative Architektur-Entwicklung
- Beginne mit groben Konzepten in Kapitel 1-4
- Verfeinere schrittweise die Details in Kapiteln 5-8
- Nutze KI für konsistente Formatierung und Struktur

### 2. Template-basiertes Arbeiten
- Nutze vorhandene arc42-Struktur als Basis
- Erweitere Templates für wiederkehrende Muster
- Dokumentiere Entscheidungen in Kapitel 9

### 3. Diagramm-Integration
- Nutze PlantUML oder Draw.io für Diagramme
- Speichere in `assets/images/` mit beschreibenden Namen
- Verweise explizit aus dem Text

### 4. Qualitätssicherung
- Regelmäßige Builds nach Änderungen
- Review von KI-generierten Inhalten
- Versionierung wichtiger Änderungen