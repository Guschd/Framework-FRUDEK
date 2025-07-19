# M12 – Automatisierte Validierung & Ableitung

## 🧭 Ziel

M12 beschreibt Werkzeuge und Logiken zur **automatischen Prüfung**, **Qualitätseinstufung** und **Historienableitung** aus Snippets und Modulen. Ziel: Reduktion manueller Prüfung und bessere Integration in KI-gestützte Workflows.

---

## 🤖 Automatisierbare Elemente

- Lizenzprüfung (bekannt/unkompatibel/fehlend)
- Reuse-Feld validieren (gegen Logik)
- YAML-Vollständigkeit
- Historienanalyse (zeitliche Abfolge, Konflikte)
- Modellversatz (z. B. GPT vs. Mensch)

---

## 🛠️ Beispiel-Regeln

```text
Wenn reuse=R2 → license darf nicht leer sein
Wenn license=CC BY-NC → reuse≠R3
Wenn keine history → Status=Q1
```

---

## 💡 Optionale Erweiterungen

- GUI-Modul zur Anzeige von Konflikten
- Visualisierung der Reuse-Pfade (Graph)
- YAML-Editor mit Validierung (M13)

---

## 🔗 Verbindungen

- basiert auf: M5, M6, M7, M9, M10, M11  
- Zielmodul zur Automatisierung innerhalb von FRUDEK  
- vorbereitet für API-Nutzung (M14)

---