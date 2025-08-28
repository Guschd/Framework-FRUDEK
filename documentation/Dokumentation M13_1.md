# M13 – Visualisierung & Darstellungsformate

## 🧭 Zielsetzung

M13 beschreibt die systematische Darstellung von Inhalten, Zusammenhängen, Prozessen und Entscheidungswegen im FRUDEK-Framework **in visuell zugänglicher Form**.

Das Modul bietet eine **Grundstruktur für grafische, schematische oder interaktive Visualisierungen**, um komplexe Abläufe und modulare Inhalte besser verständlich, teilbar und nachnutzbar zu machen.

---

## 🎯 Hauptanwendung

- **Erstellung visueller Diagramme** (z. B. Flussdiagramme, Entscheidungsbäume)
- **Export als Vektorgrafik, PNG, SVG oder Markdown-embedded**
- **Darstellung von Modulen, Relationen, Fragetypen, Eskalationen, Antwortstrategien**
- **Verlinkung mit Attributions-/Templatemodulen (M9, M10)**

---

## 🧰 Empfohlene Tools & Formate

| Tool / Format | Einsatzzweck | Vorteile |
|---------------|--------------|----------|
| `Mermaid.js`  | eingebettete Diagramme im Markdown | leicht wartbar & Git-kompatibel |
| `Graphviz (.dot)` | komplexe Entscheidungsketten | für KI-generierte Diagramme optimiert |
| `PlantUML` | Kombination aus UML & Text | flexibel für Architektur |
| `Draw.io / diagrams.net` | manuelle Visualisierung | für Fine-Tuning & Präsentation |
| `SVG exportiert aus GPT Plugin` | als statische Darstellung | portable & druckbar |
| `PDF mit eingebetteten Grafiken` | für akademische Dokumentation | zitierfähig |
# 📐 Best Practices

- Jeder Visualisierung sollte ein **YAML-Metablock** vorangestellt werden, der Quelle, Bearbeitungsstand und Lizenz nennt.  
- Farben, Symbole und Icons sind **konsistent** aus dem FRUDEK-Designsystem zu verwenden.  
- **Legenden und Tooltips** (bei interaktiven Varianten) sind Pflicht.  
- Bei **Kollaborationen**: Änderungen an Visualisierungen wie Code behandeln → Commit & Diff-Log.  

---

# 🧪 Testfall-Cluster

---

## ✅ Testfall A

**Kontext:** Modul 12 beschreibt Reaktionsstile – der Nutzer wünscht eine Übersicht.  

**Frage:** „Kannst du mir das als Übersicht geben?“  

**Empfohlene Darstellung:**  
- Tabelle  
- Mermaid-Diagramm zur Framing-Wahl auf Basis von Tonlage und Kontext  

---

## ✅ Testfall B

**Kontext:** Komplexe Kette in Modul 2.  

**Frage:** „Wie hängen Kontextauflösung, Framing und Eskalation zusammen?“  

**Lösung:**  
- Entscheidungskette als Graph (Mermaid oder DOT)  
- Exportierbar als PDF / SVG  

---

## ✅ Testfall C

**Kontext:** Technische Umsetzung für Trainings- oder Studienzwecke.  

**Frage:** „Kannst du das als druckbares Prozessblatt ausgeben?“  

**Lösung:**  
- Flussdiagramm in Draw.io  
- YAML-Metadaten + Lizenzangabe  
- PDF mit eingebetteter Quelle (M9/M10)  

---

# 🔗 Verbindungen

- setzt auf: M6 (Semantik), M9 (Attribution), M10 (Freigabe)  
- verwendet durch:  
  - Studien & Publikationen  
  - Prompt-Templates  
  - Hilfe-Module / Schulungsversionen  

---

# ⚠️ Hinweise

- Visualisierung **ersetzt nicht die Dokumentation** – sie unterstützt die Verständlichkeit.  
- Im Falle divergierender Versionen gilt immer die **textuelle Referenz** aus dem jeweiligen Modul.

## 🔍 Beispiele für Darstellungsformate

### 📊 Prozesskette (via Mermaid)

```mermaid
graph TD
  Start[⏱️ Prompt erkannt]
  Kontext[🔎 Kontextanalyse (M2)]
  Framing[🧭 Framing (M12)]
  Gewichtung[⚖️ Gewichtung]
  Antwort[💬 Antwortformulierung]
  Feedback[🔁 Feedbacklogik (optional)]

  Start --> Kontext --> Framing --> Gewichtung --> Antwort --> Feedback
