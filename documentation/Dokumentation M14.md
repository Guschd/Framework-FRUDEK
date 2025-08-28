# M14 – Validierung & Qualitätssicherung

## 🧭 Zielsetzung

M14 stellt die Werkzeuge, Methoden und Richtlinien zur Verfügung, mit denen Inhalte, Antworten und Entscheidungen innerhalb des FRUDEK-Systems auf ihre **Richtigkeit, Konsistenz und Zuverlässigkeit** geprüft werden.

Dieses Modul zielt darauf ab, **Vertrauen durch wiederholbare Prüfverfahren, Feedback-Integration und technische Validierungsprozesse** zu stärken – sowohl für menschliche als auch KI-generierte Beiträge.

---

## ✅ Anwendungsfelder

- Prüfung der Antwortqualität (inhaltlich, formal, ethisch)
- Rückverfolgbarkeit von Entscheidungen und Antwortwegen
- Double-Check durch kontrollierte Gegenfragen oder Eskalationspfade
- Qualitätssicherung durch Feedbacksysteme oder Peer-Review
- Einsatz in Pilotstudien, Modultests, Prompt-Tests

---

## 🧰 Tools & Techniken

| Tool / Verfahren | Einsatzbereich | Bemerkung |
|------------------|----------------|-----------|
| 🔄 Redundanzprüfung | semantisch ähnliche Prompts testen | erkennt Inkonsistenzen |
| 🧪 Double Prompting | zwei Varianten generieren & vergleichen | erhöht Sicherheit |
| 🤝 Peer Review (Mensch ↔ KI) | bei kritischen Inhalten / Studien | Vertrauen durch Transparenz |
| 📊 Bewertungsbögen | standardisierte Feedbackformulare | auch für Studien geeignet |
| 🧠 Logfile-Analyse | technische Validierung von Antwortverhalten | z. B. bei API-Tests |
| 🧾 Prüflisten / Checklisten | manuelle QS für sensitive Usecases | z. B. medizinische, juristische Anfragen |

---

## 🧪 Testfall-Cluster

### ✅ Testfall A

**Frage:** „Warum kommen bei gleicher Frage unterschiedliche Antworten?“

**Analyse:** Redundanzprüfung (verschiedene Nutzer, gleiches Thema). Unterschiede durch Framing (M12) oder tagesaktuelle Wissensbasis.

**QS-Maßnahme:** Antwortvergleiche loggen, Version annotieren, Auslöser klären.

---

### ✅ Testfall B

**Frage:** „Kann ich mich auf die Antwort verlassen? Ich muss das in meiner Bachelorarbeit zitieren.“

**Lösung:**  
→ Modul 9 (Attribution) + Modul 14 → Qualitätssicherungskennzeichnung  
→ Vorschlag: Metadaten-Export + optionaler Vermerk: *nicht peer-reviewed*

---

### ✅ Testfall C

**Kontext:** Zwei KI-Antworten liefern unterschiedliche technische Pfade (z. B. zur Serverdiagnose)

**QS-Schritte:**

- Replikation der Testbedingungen
- Extraktion der relevanten Module (z. B. M2, M4, M6)
- Rückfrage an Nutzer: „Welche Konfiguration bestand genau?“
- Nachtest mit simulierter Umgebung

---

## 📌 Metadaten & Kontrollfelder

In alle qualitätsrelevanten Ausgaben können folgende Felder eingebettet werden:

```yaml
quality_check: passed
confidence_level: 0.92
peer_reviewed: false
last_validated: 2025-08-07
validator: GPT-4o / SB


🔄 Feedbackzyklen


Eingebettet in Studienprojekte (z. B. bei Modultests)
Eskalation an Kontrollinstanz bei widersprüchlichen Ergebnissen
Möglichkeit zur Rückmeldung durch Nutzer (Schaltfläche oder Prompt)





🔗 Verbindungen


verwendet durch: M1–M13 (inhaltliche Validierung)
besonders relevant für: 
M9 (Attribution)
M12 (Framing)
M11 (technische Fehlerbilder)

⚠️ Hinweise


KI-generierte Inhalte müssen kenntlich gemacht werden
Studienoutputs brauchen mehrstufige QS (Pilot, Review, Archivierung)
Validierung ≠ Wahrheit → Modul liefert belastbare Wahrscheinlichkeiten, keine Beweise

---
modul: M14
title: Validierung & Qualitätssicherung
author: Sebastian Besold / GPT-4o
version: 1.0
linked_modules: [M1, M9, M11, M12]
tools: [redundanztest, peer_review, checklists, feedbacklog]
license: CC BY 4.0
last_updated: 2025-08-07
---
