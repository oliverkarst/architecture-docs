# Prompt-Templates für Architekturanalyse

## 1. System-Kontextanalyse

### Prompt für Kapitel 3 (Kontextabgrenzung)

```
Kontext: [SYSTEM_BESCHREIBUNG]
Aufgabe: Analysiere das System und erstelle eine Kontextabgrenzung für arc42 Kapitel 3

Erstelle:
1. Fachlicher Kontext - externe Akteure und deren Schnittstellen
2. Technischer Kontext - externe Systeme und Protokolle
3. Kontextdiagramm als PlantUML-Code

Format: 
- Deutsche Überschriften nach arc42-Template
- PlantUML-Syntax für Diagramme
- Strukturierte Listen für Schnittstellen

Berücksichtige:
- Datenschutz und Compliance-Aspekte
- Performance-relevante Schnittstellen
- Security-Boundaries
```

### Anwendungsbeispiel:
**Input:** "E-Commerce-Plattform mit Webshop, Payment-Gateway und Lagerverwaltung"

**Expected Output:** 
- PlantUML-Diagramm mit Akteuren (Kunde, Admin, Payment-Provider)
- Tabellarische Schnittstellenbeschreibung
- Technische Protokolle und Standards

## 2. Lösungsstrategie-Entwicklung

### Prompt für Kapitel 4 (Lösungsstrategie)

```
Kontext: [QUALITÄTSZIELE] und [RANDBEDINGUNGEN]
Aufgabe: Entwickle eine Lösungsstrategie für arc42 Kapitel 4

Erstelle strukturierte Antworten zu:
1. Technische Entscheidungen mit Begründung
2. Architekturprinzipien und -pattern
3. Wichtige Implementierungsaspekte

Format:
- Tabelle: Qualitätsziel → Lösungsansatz → Rationale
- Bullet-Points für Designprinzipien
- Verweise auf etablierte Pattern

Kriterien:
- Konsistenz mit Qualitätszielen
- Realisierbarkeit in gegebenen Constraints
- Wartbarkeit und Erweiterbarkeit
```

## 3. Bausteinsicht-Generierung

### Prompt für Kapitel 5 (Bausteinsicht)

```
Kontext: [LÖSUNGSSTRATEGIE] und [SYSTEM_KOMPLEXITÄT]
Aufgabe: Erstelle Bausteinsicht für arc42 Kapitel 5

Generiere für jede Ebene:
1. Whitebox-Diagramm als PlantUML
2. Tabellarische Bausteindescription
3. Schnittstellen und Abhängigkeiten

Struktur:
- Ebene 1: Grobe Systemaufteilung (3-7 Bausteine)
- Ebene 2: Verfeinerung kritischer Bausteine
- Konsistente Namenskonventionen

PlantUML-Anforderungen:
- Deutsche Beschriftungen
- Dependency-Pfeile mit Labels
- Logische Gruppierungen
```

### Template-Code:
```plantuml
@startuml Bausteinsicht_Ebene1
!define RECTANGLE class

package "System XY" {
  RECTANGLE Baustein1 [
    <b>Baustein 1
    --
    Verantwortlichkeit 1
    Verantwortlichkeit 2
  ]
  
  RECTANGLE Baustein2 [
    <b>Baustein 2
    --
    Verantwortlichkeit A
    Verantwortlichkeit B
  ]
  
  Baustein1 --> Baustein2 : Interface X
}
@enduml
```

## 4. Qualitätsanforderungen-Ableitung

### Prompt für Kapitel 10 (Qualitätsanforderungen)

```
Kontext: [STAKEHOLDER_ERWARTUNGEN] und [SYSTEM_CRITICALITY]
Aufgabe: Konkretisiere Qualitätsanforderungen für arc42 Kapitel 10

Erstelle Qualitätsszenarien nach Schema:
1. Stimulus → System → Response → Measure
2. Kategorisierung nach ISO 25010
3. Testbare Akzeptanzkriterien

Format:
- Tabelle mit Szenario, Priorität, Kriterien
- Messbare Metriken (z.B. Response Time < 200ms)
- Verifikationsmethoden

Fokus auf:
- Performance, Usability, Security
- Operationelle Qualitätsmerkmale
- Compliance-Anforderungen
```

## 5. ADR-Generierung

### Prompt für Kapitel 9 (Architekturentscheidungen)

```
Kontext: [TECHNISCHE_ENTSCHEIDUNG] mit [ALTERNATIVEN]
Aufgabe: Erstelle Architecture Decision Record (ADR) für arc42 Kapitel 9

Verwende ADR-Template:
1. Status: [Proposed/Accepted/Deprecated]
2. Kontext: Warum ist die Entscheidung nötig?
3. Entscheidung: Was wurde entschieden?
4. Konsequenzen: Positive und negative Auswirkungen

Stil:
- Prägnant und nachvollziehbar
- Objektive Darstellung von Alternativen
- Klare Rationale für Entscheidung
- Auswirkungen auf andere Entscheidungen
```

### ADR-Template:
```markdown
## ADR-XXX: [Titel der Entscheidung]

**Status:** Accepted
**Datum:** [YYYY-MM-DD]
**Entscheider:** [Namen]

### Kontext
[Beschreibung der Situation und des Problems]

### Entscheidung  
[Die getroffene Entscheidung]

### Alternativen
- Alternative 1: [Beschreibung + Pro/Contra]
- Alternative 2: [Beschreibung + Pro/Contra]

### Konsequenzen
**Positiv:**
- [Positive Auswirkung 1]

**Negativ/Risiken:**
- [Negative Auswirkung 1]

**Neutral:**
- [Neutrale Auswirkung 1]
```

## 6. Verwendung und Anpassung

### Best Practices:
1. **Kontextualisierung:** Ersetze [PLACEHOLDER] mit projektspezifischen Informationen
2. **Iterative Verfeinerung:** Nutze Outputs als Input für Folge-Prompts  
3. **Qualitätskontrolle:** Validiere generierte Inhalte fachlich
4. **Versionierung:** Dokumentiere erfolgreiche Prompt-Varianten

### Anpassung an Projekttypen:
- **Microservices:** Erweitere Bausteinsicht um Service-Boundaries
- **Legacy-Systeme:** Fokus auf Risiken und Modernisierungsstrategie  
- **Embedded Systems:** Hardware-Software-Verteilung in Deployment-Sicht

### Qualitätskriterien für Outputs:
- ✅ Vollständige arc42-Struktur
- ✅ Deutsche Fachterminologie
- ✅ Konsistente Diagramm-Notation
- ✅ Nachvollziehbare Entscheidungsrationalе
- ✅ Testbare/messbare Qualitätskriterien