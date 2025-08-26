# Architecture Decision Record Template

## ADR-001: [Titel der Architekturentscheidung]

**Status:** [Proposed | Accepted | Deprecated | Superseded by ADR-XXX]  
**Datum:** [YYYY-MM-DD]  
**Entscheider:** [Namen oder Rollen]  
**Review-Datum:** [YYYY-MM-DD - für wichtige Entscheidungen]

### Kontext und Problemstellung

[Beschreibe die Situation und das Problem, das eine Architekturentscheidung erfordert. Führe technische, organisatorische oder projektspezifische Details auf, die für das Verständnis wichtig sind.]

**Business-Driver:**
- [Geschäftlicher Grund 1]
- [Geschäftlicher Grund 2]

**Technische Anforderungen:**
- [Technische Anforderung 1]
- [Technische Anforderung 2]

**Constraints:**
- [Beschränkung 1]
- [Beschränkung 2]

### Entscheidung

[Beschreibe die Entscheidung, die getroffen wurde. Verwende aktive Sprache.]

**Gewählte Option:** [Name/Beschreibung der gewählten Alternative]

**Begründung:** [Warum wurde diese Option gewählt?]

### Betrachtete Alternativen

#### Alternative 1: [Name der Alternative]
**Beschreibung:** [Kurze technische Beschreibung]

**Vorteile:**
- ✅ [Vorteil 1]
- ✅ [Vorteil 2]

**Nachteile:**
- ❌ [Nachteil 1] 
- ❌ [Nachteil 2]

**Bewertung:** [Warum wurde diese Alternative verworfen?]

#### Alternative 2: [Name der Alternative]
**Beschreibung:** [Kurze technische Beschreibung]

**Vorteile:**
- ✅ [Vorteil 1]
- ✅ [Vorteil 2]

**Nachteile:**
- ❌ [Nachteil 1]
- ❌ [Nachteil 2]

**Bewertung:** [Warum wurde diese Alternative verworfen?]

### Konsequenzen

#### Positive Auswirkungen
- ✅ [Positive Auswirkung 1]
- ✅ [Positive Auswirkung 2]
- ✅ [Positive Auswirkung 3]

#### Negative Auswirkungen/Risiken
- ⚠️ [Risiko oder Nachteil 1]
- ⚠️ [Risiko oder Nachteil 2]

#### Neutrale Auswirkungen
- ℹ️ [Neutrale Auswirkung 1]
- ℹ️ [Neutrale Auswirkung 2]

### Implementierung

**Erforderliche Schritte:**
1. [Implementierungsschritt 1]
2. [Implementierungsschritt 2]
3. [Implementierungsschritt 3]

**Aufwand:** [Geschätzter Aufwand in Personentagen]
**Timeline:** [Geplanter Implementierungszeitraum]
**Verantwortlich:** [Name/Team für Umsetzung]

### Monitoring und Messung

**Erfolgskriterien:**
- [Messbarer Erfolgsfaktor 1]
- [Messbarer Erfolgsfaktor 2]

**Monitoring-Metriken:**
- [Metrik 1] - Zielwert: [Wert]
- [Metrik 2] - Zielwert: [Wert]

**Review-Trigger:**
- Nach [Zeitraum] automatische Überprüfung
- Bei Erreichen von [spezifischem Ereignis]

### Verwandte Entscheidungen

**Abhängige ADRs:**
- [ADR-XXX: Titel] - Diese Entscheidung baut auf/wird beeinflusst von

**Betroffene Systeme/Komponenten:**
- [System 1] - [Art der Auswirkung]
- [System 2] - [Art der Auswirkung]

### Notizen

**Diskussion:**
- [Wichtige Punkte aus der Diskussion]
- [Ungelöste Fragen oder zukünftige Überlegungen]

**Lessons Learned:**
- [Erkenntnisse aus vorherigen ähnlichen Entscheidungen]

**Referenzen:**
- [Link zu relevanten Dokumenten]
- [Externe Quellen oder Standards]

---

## Verwendungshinweise

### KI-Prompt für ADR-Erstellung:

```
Kontext: [TECHNISCHE_SITUATION_ODER_PROBLEM]
Aufgabe: Erstelle ein ADR nach dem bereitgestellten Template

Entscheidung: [WELCHE_ENTSCHEIDUNG_GETROFFEN_WERDEN_SOLL]
Alternativen: [BEKANNTE_ALTERNATIVEN_ODER_OPTIONEN]
Stakeholder: [WER_IST_BETROFFEN]

Format: Vollständiges ADR nach Template
Stil: Objektiv, nachvollziehbar, technisch präzise
Fokus: Rationale für Entscheidung und langfristige Auswirkungen
```

### Best Practices:

1. **Ein ADR pro Entscheidung** - Vermeide zu breite oder zu spezifische Scope
2. **Zeitnahe Dokumentation** - Erstelle ADRs während oder kurz nach der Entscheidungsfindung
3. **Objektive Darstellung** - Stelle auch verworfene Alternativen fair dar
4. **Messbare Konsequenzen** - Definiere konkrete Erfolgs- und Risiko-Metriken
5. **Living Documents** - Aktualisiere Status und Lessons Learned über Zeit

### Anpassung für verschiedene Bereiche:

- **Security-Entscheidungen:** Erweitere um Threat Model und Compliance-Aspekte
- **Performance-Entscheidungen:** Fokus auf Metriken und Benchmarking
- **Tool/Framework-Auswahl:** Detaillierte Evaluationskriterien
- **Architektur-Pattern:** Verweis auf etablierte Pattern und deren Anwendbarkeit