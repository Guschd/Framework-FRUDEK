# M8 – Historien & Änderungsnachverfolgung

## 🧭 Ziel

M8 definiert die Prinzipien und Verfahren zur **dokumentierten Änderungshistorie** in KI-gestützter Kreativarbeit. Damit soll jede Änderung an Inhalten – ob textlich, strukturell oder lizenziell – nachvollziehbar, attributierbar und reproduzierbar gemacht werden.

Ziel ist eine lückenlose Rückverfolgung (Audit-Trail) in Verbindung mit menschlicher oder KI-gestützter Autorenschaft.

---

## 🧬 Änderungsformen

| Typ | Beschreibung | Beispiel |
|-----|--------------|----------|
| 📝 **Inhaltlich** | Text, Struktur, Inhalt wird verändert | Umbau einer Markdown-Struktur |
| 🧾 **Formal** | Metadaten, Formatierung, YAML-Blöcke | Lizenzfeld von „leer“ auf CC BY |
| 🔀 **Strukturell** | Reihenfolge, Kapitelstruktur, Modularisierung | Aufspaltung eines Moduls |
| 🧪 **KI-generiert** | Änderung erfolgt durch Sprachmodell | Rewrite durch GPT-4 |
| 🕵️ **Manual Override** | explizite, manuell gesetzte Änderung | „Text wurde bewusst verkürzt“ |

---

## 📋 Beispiel-Logik für Änderungsvermerke

```yaml
# am Kopf einer Datei
---
history:
  - date: 2025-07-17
    by: GPT-4
    type: rewrite
    note: "Abschnitt 2.3 wurde präzisiert"
  - date: 2025-07-19
    by: Sebastian
    type: manual
    note: "Layoutvorgaben aus M2 übernommen"
---
```

---

## 🛠️ Werkzeuge zur Historienverfolgung

| Ebene | Werkzeug | Beschreibung |
|-------|----------|--------------|
| 🔍 Snippet | YAML-Verlauf | Manuelle History-Einträge je Fragment |
| 🗂️ Modul | Git-Commits | Git-Logs pro Markdown |
| 🧠 KI-Intervention | Prompt-Protokoll | GPT-Eingaben als Historie abspeichern |
| 📅 Zeitmarke | FRUDEK-Timestamps | automatische Zeitstempel bei Änderung |
| 🔗 Quellverweis | `source:` Tag | Rückverlinkung zu Ursprungsversionen |

---

## 🧩 Best Practices

- ✍️ Alle Änderungen **immer mit Zeit, Autor, Zweck** dokumentieren  
- 💡 Auch KI-generierte Änderungen als solche kennzeichnen  
- 🧠 Bei Rewrite durch Sprachmodell: Prompt + Modellversion speichern  
- 📁 Dateien mit Konflikthistorie in separatem Ordner ablegen („/legacy“ oder „/review“)  
- 🔐 Historien nicht löschen, nur ergänzen

---

## 🧪 Beispiel für GPT-Revisionseintrag

```yaml
history:
  - date: 2025-07-18
    by: GPT-4
    type: refinement
    prompt: "Fasse diesen Abschnitt kürzer, aber sachlich korrekt."
    model: GPT-4.5-turbo
```

---

## 🔄 Integration mit GitHub

- Git-Kommentare als Quellhistorie nutzbar (z. B. „M6: Lizenzkonfliktlogik ergänzt“)  
- Historienblock direkt aus Commit-Message erzeugbar (optionales Tool M12)  
- Vergleichsansicht mit `diff` oder `rich diff` bei Markdown sinnvoll

---

## 🔗 Verknüpfung zu anderen Modulen

- basiert auf:  
  → M3 – Dokumentationsformate  
  → M5 – YAML-Metadaten  
  → M7 – Konfliktlösung

- wird verwendet in:  
  → M9 – Attribution  
  → M10 – Freigabeübersicht  
  → M12 – Automatisierte Historienableitung

---