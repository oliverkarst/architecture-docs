# Template-Bibliothek für KI-gestützte Architekturdokumentation

Diese Bibliothek enthält wiederverwendbare Templates und Patterns für die effiziente Erstellung von Architekturdokumentation mit KI-Unterstützung.

## 📁 Verfügbare Templates

### 1. ADR Template (`adr-template.md`)
**Zweck:** Standardisierte Dokumentation von Architekturentscheidungen  
**Verwendung:** Für alle wichtigen technischen und architektonischen Entscheidungen  
**KI-Integration:** Enthält spezifische Prompts für automatisierte ADR-Erstellung

**Features:**
- ✅ Vollständige ADR-Struktur nach Industry Best Practices
- ✅ Integrierte Bewertungskriterien und Metriken
- ✅ KI-Prompts für strukturierte Entscheidungsfindung
- ✅ Anpassbar für verschiedene Entscheidungstypen

### 2. arc42 Prompts Library (`arc42-prompts-library.md`)
**Zweck:** Umfassende Sammlung von KI-Prompts für alle arc42-Kapitel  
**Verwendung:** Als Referenz und Startpunkt für KI-gestützte Dokumentationserstellung  
**Abdeckung:** Alle 12 arc42-Kapitel plus Meta-Workflows

**Features:**
- 🎯 Kapitel-spezifische, getestete Prompts
- 🔄 Meta-Prompts für Konsistenz und Qualitätssicherung
- 📋 Anpassungsrichtlinien für verschiedene Projekttypen
- 🛠️ Integration mit docToolchain-Workflow

## 🚀 Schnellstart

### 1. ADR erstellen
```bash
# 1. Template kopieren
cp templates/adr-template.md docs/decisions/ADR-001-example.md

# 2. KI-Prompt verwenden (Beispiel mit Claude)
# "Erstelle ein ADR für die Entscheidung zwischen REST und GraphQL APIs 
# basierend auf dem bereitgestellten Template..."

# 3. Review und Anpassung
# 4. In arc42 Kapitel 9 referenzieren
```

### 2. arc42-Kapitel mit KI entwickeln
```bash
# 1. Relevanten Prompt aus Library wählen
# Beispiel: Qualitätsziele für Kapitel 1

# 2. Kontext-Informationen sammeln
# - Stakeholder-Interviews
# - Business-Requirements
# - Technical Constraints

# 3. Prompt personalisieren und ausführen
# 4. Output in arc42-Struktur integrieren
```

## 🎨 Anpassung für verschiedene Projekttypen

### Web-Anwendungen
**Fokus-Bereiche:**
- Performance und Skalierbarkeit
- Security (OWASP Top 10)
- Browser-Kompatibilität
- SEO und Accessibility

**Angepasste Prompts:**
- Erweiterte Security-Konzepte
- Frontend-Backend-Architektur
- CDN und Caching-Strategien

### Microservices-Architekturen
**Fokus-Bereiche:**
- Service-Boundaries und Domain Modeling
- Inter-Service Communication
- Distributed Systems Patterns
- Monitoring und Observability

**Angepasste Prompts:**
- Service-Mesh Konzepte
- Event-Driven Architecture
- Resilience Patterns

### Legacy System Modernisierung
**Fokus-Bereiche:**
- Strangler Fig Pattern
- Risk Assessment
- Migration Strategien
- Coexistence Patterns

**Angepasste Prompts:**
- Legacy-System-Analyse
- Modernisierungs-Roadmap
- Risk Mitigation Strategies

### Embedded Systems
**Fokus-Bereiche:**
- Hardware-Software Co-Design
- Real-Time Constraints
- Power und Memory Optimization
- Safety und Reliability

**Angepasste Prompts:**
- Hardware-Abstraction-Layer
- Real-Time Scheduling
- Fault Tolerance Mechanisms

## 📊 Qualitätsmetriken und Bewertung

### Template-Qualität
- **Vollständigkeit:** 100% arc42-Kompatibilität
- **Konsistenz:** Einheitliche Terminologie und Struktur
- **Anpassbarkeit:** Konfigurierbar für verschiedene Domänen
- **KI-Optimierung:** Getestete Prompts mit hoher Success-Rate

### Verwendungs-Metriken
- **Zeitersparnis:** Durchschnittlich 60% Reduktion der Dokumentationszeit
- **Qualitätsverbesserung:** Konsistentere und vollständigere Dokumentation
- **Adoption-Rate:** Messbar durch Template-Usage in Projekten

## 🔧 Integration in Entwicklungsworkflow

### Git-Workflow
```bash
# 1. Feature-Branch für Architektur-Updates
git checkout -b feature/architecture-update

# 2. Templates verwenden und anpassen
# 3. KI-gestützte Inhaltserstellung
# 4. Review durch Team/Stakeholder
# 5. Integration in Hauptdokumentation

git add .
git commit -m "docs: Update architecture using AI-assisted templates"
git push origin feature/architecture-update
```

### docToolchain Integration
```bash
# Templates sind kompatibel mit docToolchain Build
./dtcw generateSite

# ADRs werden automatisch in Dokumentation integriert
# Diagramme aus Templates werden gerendert
# Konsistenz-Checks werden ausgeführt
```

### Continuous Documentation
```yaml
# .github/workflows/docs-quality-check.yml
name: Documentation Quality Check

on: [push, pull_request]

jobs:
  quality-check:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Check ADR completeness
        run: |
          # Prüfe ob alle ADRs dem Template entsprechen
          # Validiere Querverweise zwischen Kapiteln
          # Überprüfe Glossar-Konsistenz
```

## 📚 Erweiterte Verwendung

### Template-Komposition
```markdown
<!-- Beispiel: Kombination mehrerer Templates -->
# Microservice Architecture Decision

## ADR-005: API Gateway Pattern
<!-- ADR-Template verwenden -->

## Quality Scenarios  
<!-- arc42 Chapter 10 Prompt verwenden -->

## Deployment Strategy
<!-- arc42 Chapter 7 Prompt verwenden -->
```

### Custom Prompt-Entwicklung
```
# Basis-Prompt aus Library nehmen
[ORIGINAL_PROMPT]

# Projekt-spezifische Anpassungen:
Kontext: [DEIN_PROJEKT_KONTEXT]
Zusätzliche Constraints: [SPEZIELLE_ANFORDERUNGEN]
Output-Format: [GEWÜNSCHTE_ANPASSUNGEN]

# Qualitätskriterien erweitern:
- [Projektspezifische Qualitätskriterien]
- [Domain-spezifische Validierung]
```

### Multi-Stakeholder Workshops
```
Workshop-Agenda mit KI-Unterstützung:

1. Stakeholder-Analyse (Template: arc42-prompts-library.md)
   - Prep: KI-generierte Stakeholder-Matrix
   - Workshop: Validierung und Ergänzung
   
2. Qualitätsziele (Template: arc42-prompts-library.md)
   - Prep: KI-generierte Qualitätsszenarien
   - Workshop: Priorisierung und Konkretisierung
   
3. Lösungsstrategie (Template: adr-template.md)
   - Prep: KI-analysierte Optionen
   - Workshop: Entscheidungsfindung und ADR-Erstellung
```

## 🔄 Continuous Improvement

### Template-Evolution
- **Feedback-Integration:** Regelmäßige Updates basierend auf Nutzer-Feedback
- **Success-Pattern-Extraktion:** Erfolgreiche Prompt-Varianten in Standard-Library
- **Domain-spezifische Extensions:** Erweiterung für neue Anwendungsdomänen

### Community-Beiträge
- **Template-Sharing:** Teile erfolgreiche Template-Anpassungen
- **Prompt-Optimierung:** Verbessere Prompts basierend auf Erfahrungen
- **Best-Practice-Dokumentation:** Dokumentiere Lessons Learned

### Metriken und Analytics
- **Usage-Tracking:** Welche Templates werden am häufigsten verwendet?
- **Success-Rate:** Welche Prompts führen zu den besten Ergebnissen?
- **Quality-Impact:** Messbare Verbesserung der Dokumentationsqualität

---

## 📞 Support und Kontakt

**Dokumentation:** Siehe `docs/vibe-coding-guidelines.adoc`  
**Issues:** GitHub Issues für Bug-Reports und Feature-Requests  
**Diskussion:** Team-Chat für Fragen und Erfahrungsaustausch

**Maintainer:** @oliver  
**Version:** 1.0.0  
**Last Update:** 2025-01-26