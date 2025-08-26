# arc42 Prompts-Bibliothek für KI-gestützte Dokumentation

## Kapitel-spezifische Prompts

### Kapitel 1: Einführung und Ziele

#### Stakeholder-Analyse
```
Kontext: [PROJECT_DESCRIPTION]
Aufgabe: Identifiziere und beschreibe Stakeholder für arc42 Kapitel 1

Analysiere für jeden Stakeholder:
1. Rolle und Verantwortungsbereich
2. Erwartungshaltung bezüglich der Architektur
3. Einfluss auf Architekturentscheidungen
4. Kommunikationsbedürfnisse

Format: arc42-konforme Tabelle mit deutschen Überschriften
Zielgruppe: [TECHNICAL_LEVEL] Dokumentationsleser
```

#### Qualitätsziele definieren
```
Kontext: [BUSINESS_REQUIREMENTS] und [SYSTEM_CONSTRAINTS]
Aufgabe: Definiere Top-5 Qualitätsziele für arc42 Kapitel 1

Erstelle für jedes Qualitätsziel:
1. ISO 25010-Kategorie
2. Konkretes, messbares Szenario
3. Priorität und Rationale
4. Konfliktpotential mit anderen Zielen

Format: Tabelle nach arc42-Template
Fokus: Testbare und operationalisierbare Ziele
```

### Kapitel 2: Randbedingungen

#### Constraint-Katalogisierung
```
Kontext: [ORGANIZATIONAL_CONTEXT] und [TECHNICAL_ENVIRONMENT]
Aufgabe: Systematisiere Randbedingungen für arc42 Kapitel 2

Kategorien:
1. Organisatorische Randbedingungen
2. Technische Randbedingungen
3. Konventionen

Für jede Constraint:
- Beschreibung und Hintergrund
- Auswirkung auf Architektur
- Flexibilität/Verhandelbarkeit

Format: Strukturierte Listen nach arc42-Schema
```

### Kapitel 3: Kontextabgrenzung

#### Fachlicher Kontext
```
Kontext: [DOMAIN_DESCRIPTION]
Aufgabe: Erstelle fachlichen Kontext für arc42 Kapitel 3

Identifiziere:
1. Alle fachlichen Nachbarsysteme
2. Geschäftsprozesse an den Schnittstellen
3. Datenfluss und Geschäftsobjekte
4. Verantwortlichkeiten und Grenzen

Zusätzlich: PlantUML-Kontextdiagramm mit deutschen Beschriftungen
Format: Kombination aus Fließtext, Tabelle und Diagramm
```

#### Technischer Kontext
```
Kontext: [SYSTEM_INTEGRATION_REQUIREMENTS]
Aufgabe: Definiere technischen Kontext für arc42 Kapitel 3

Spezifiziere für jede Schnittstelle:
1. Technisches Protokoll (HTTP/REST, Message Queue, etc.)
2. Datenformat (JSON, XML, Binary)
3. Fehlerbehandlung und Retry-Strategien
4. Security-Mechanismen
5. Performance-Charakteristika

Format: Tabelle + PlantUML-Diagramm mit Protokoll-Labels
```

### Kapitel 4: Lösungsstrategie

#### Strategische Entscheidungen
```
Kontext: [QUALITY_GOALS] und [CONSTRAINTS]
Aufgabe: Entwickle Lösungsstrategie für arc42 Kapitel 4

Erstelle Mapping:
Qualitätsziel → Architektur-Ansatz → Rationale → Alternativen

Berücksichtige:
1. Architekturmuster (Layered, Microservices, etc.)
2. Technologie-Entscheidungen
3. Organisatorische Aspekte
4. Risiko-Mitigation

Format: Strukturierter Text mit Begründungs-Tabellen
Stil: Entscheidungsorientiert und nachvollziehbar
```

### Kapitel 5: Bausteinsicht

#### Hierarchische Zerlegung
```
Kontext: [SYSTEM_COMPLEXITY] und [SOLUTION_STRATEGY]
Aufgabe: Entwickle Bausteinsicht für arc42 Kapitel 5

Erstelle für jede Ebene (1-3):
1. Whitebox-Beschreibung mit PlantUML
2. Tabellarische Baustein-Beschreibung
3. Wichtige Schnittstellen
4. Blackbox-Template für kritische Bausteine

PlantUML-Anforderungen:
- Konsistente Namenskonventionen
- Dependency-Richtungen
- Schnittstellen-Labels
- Farbkodierung nach Verantwortung

Ziel: Verständliche Systemdekomposition
```

### Kapitel 6: Laufzeitsicht

#### Szenario-Modellierung
```
Kontext: [KEY_USE_CASES] und [SYSTEM_BUILDING_BLOCKS]
Aufgabe: Erstelle Laufzeitsicht für arc42 Kapitel 6

Wähle 3-5 wichtigste Szenarien:
1. Happy Path des Hauptuse-Cases
2. Kritische Fehlerbehandlung
3. Performance-kritischer Pfad
4. Security-relevanter Ablauf

Für jedes Szenario:
- PlantUML-Sequenzdiagramm
- Textuelle Beschreibung der Schritte
- Qualitäts-Aspekte (Performance, Security)
- Varianten und Alternativen

Format: Diagramm + erklärende Beschreibung
```

### Kapitel 7: Verteilungssicht

#### Deployment-Architektur
```
Kontext: [INFRASTRUCTURE_REQUIREMENTS] und [SCALABILITY_NEEDS]
Aufgabe: Entwerfe Verteilungssicht für arc42 Kapitel 7

Modeliere:
1. Hardware-Topologie
2. Software-Deployment auf Nodes
3. Netzwerk-Verbindungen und Protokolle
4. Redundanz und Failover

PlantUML-Deployment-Diagramm mit:
- Node-Definitionen für Hardware
- Artifact-Placement
- Communication-Paths
- Kapazitäts-Annotationen

Zusätzlich: Operational Procedures (Start/Stop/Monitor)
```

### Kapitel 8: Querschnittliche Konzepte

#### Konzept-Entwicklung
```
Kontext: [CROSS_CUTTING_CONCERN] (z.B. Security, Logging, Error Handling)
Aufgabe: Beschreibe querschnittliches Konzept für arc42 Kapitel 8

Struktur:
1. Problem und Zielsetzung
2. Lösungsansatz und Pattern
3. Umsetzung in verschiedenen Bausteinen
4. Konfiguration und Variabilität
5. Beispiele und Code-Snippets

Diagramm-Typ wählen:
- Klassendiagramm für strukturelle Konzepte
- Aktivitätsdiagramm für Prozess-Konzepte
- Komponentendiagramm für Verteilungs-Konzepte

Ziel: Wiederverwendbare, konsistente Umsetzung
```

### Kapitel 9: Architekturentscheidungen

#### ADR-Generierung
```
Kontext: [TECHNICAL_DECISION] mit [ALTERNATIVES_CONSIDERED]
Aufgabe: Erstelle Architecture Decision Record für arc42 Kapitel 9

ADR-Struktur:
1. Status und Kontext
2. Entscheidung mit Rationale
3. Konsequenzen (positiv/negativ)
4. Betroffene Stakeholder
5. Implementierungs-Implikationen

Stil:
- Objektive Darstellung von Alternativen
- Messbare Entscheidungskriterien
- Nachvollziehbare Begründung
- Langfristige Perspektive

Template: Nutze standardisiertes ADR-Format
```

### Kapitel 10: Qualitätsanforderungen

#### Qualitätsbaum und Szenarien
```
Kontext: [STAKEHOLDER_EXPECTATIONS] und [SYSTEM_CHARACTERISTICS]
Aufgabe: Konkretisiere Qualitätsanforderungen für arc42 Kapitel 10

Erstelle Qualitätsszenarien nach Schema:
Stimulus → System → Response → Measure

ISO 25010-Kategorien priorisieren:
1. Performance Efficiency
2. Security
3. Reliability
4. Usability
5. Maintainability

Format: Tabelle mit konkreten, testbaren Szenarien
Zusätzlich: Qualitätsbaum als Mind-Map oder Hierarchie
```

### Kapitel 11: Risiken und technische Schulden

#### Risiko-Assessment
```
Kontext: [SYSTEM_ARCHITECTURE] und [TECHNOLOGY_CHOICES]
Aufgabe: Identifiziere Risiken für arc42 Kapitel 11

Kategorisiere Risiken:
1. Technische Risiken
2. Organisatorische Risiken
3. Externe Abhängigkeiten
4. Qualitätsrisiken

Für jedes Risiko:
- Wahrscheinlichkeit (Hoch/Mittel/Niedrig)
- Impact-Bewertung
- Mitigation-Strategien
- Monitoring-Indikatoren

Format: Risiko-Register mit Maßnahmen-Roadmap
```

### Kapitel 12: Glossar

#### Terminologie-Management
```
Kontext: [DOMAIN_TERMINOLOGY] und [TECHNICAL_TERMS]
Aufgabe: Erstelle Glossar für arc42 Kapitel 12

Sammle Begriffe aus:
1. Fachdomäne/Business-Begriffe
2. Technische Architektur-Begriffe
3. Produkt-/Projekt-spezifische Begriffe
4. Abkürzungen und Akronyme

Pro Begriff:
- Präzise Definition
- Kontext der Verwendung
- Synonyme oder verwandte Begriffe
- Referenzen zu relevanten Kapiteln

Format: Alphabetische Liste oder thematische Gruppierung
Ziel: Einheitliches Verständnis aller Stakeholder
```

## Meta-Prompts für Dokumentations-Workflow

### Konsistenz-Check
```
Kontext: [VOLLSTÄNDIGE_ARC42_DOKUMENTATION]
Aufgabe: Prüfe Konsistenz zwischen arc42-Kapiteln

Validiere:
1. Konsistente Verwendung von Begriffen (vs. Glossar)
2. Übereinstimmung Qualitätsziele ↔ Lösungsstrategie
3. Bausteinsicht ↔ Laufzeitsicht Konsistenz
4. ADR-Referenzen und Abhängigkeiten
5. Stakeholder-Erwartungen ↔ Qualitätsanforderungen

Output: Liste von Inkonsistenzen mit Kapitel-Referenzen
Priorisierung: Nach Auswirkung auf Verständlichkeit
```

### Vollständigkeits-Assessment
```
Kontext: [AKTUELLE_ARC42_DOKUMENTATION] und [PROJECT_PHASE]
Aufgabe: Bewerte Vollständigkeit der Architekturdokumentation

Prüfe pro Kapitel:
1. Pflichtinhalte nach arc42-Template
2. Projektspezifische Vollständigkeit
3. Zielgruppengerechte Detailtiefe
4. Aktualität der Informationen

Bewertung:
- ✅ Vollständig und aktuell
- ⚠️ Unvollständig aber ausreichend
- ❌ Unvollständig und kritisch

Output: Vollständigkeits-Matrix mit Handlungsempfehlungen
```

### Qualitäts-Review
```
Kontext: [ARC42_KAPITEL_ODER_SEKTION]
Aufgabe: Führe Qualitäts-Review der Dokumentation durch

Kriterien:
1. **Korrektheit:** Fachlich richtige Inhalte
2. **Verständlichkeit:** Angemessen für Zielgruppe
3. **Vollständigkeit:** Alle relevanten Aspekte abgedeckt
4. **Konsistenz:** Einheitliche Terminologie und Stil
5. **Aktualität:** Übereinstimmung mit aktueller Systemrealität

Bewertungsskala: 1-5 mit spezifischen Verbesserungsvorschlägen
Format: Review-Report mit priorisierten Maßnahmen
```

## Verwendung und Anpassung

### Prompt-Personalisierung:
1. **Kontext ersetzen:** [PLACEHOLDER] durch projektspezifische Informationen
2. **Detailgrad anpassen:** Je nach Zielgruppe und Projektphase
3. **Output-Format:** An Tool-Chain und Präferenzen anpassen
4. **Iterative Verfeinerung:** Outputs als Input für Follow-up-Prompts verwenden

### Best Practices:
- **Ein Prompt pro Konzept:** Vermeide zu breite oder komplexe Aufgaben
- **Spezifische Constraints:** Definiere klar Format, Stil und Umfang
- **Validierung einbauen:** Definiere Qualitätskriterien im Prompt
- **Kontextualisierung:** Gib immer ausreichend Projektkontext mit