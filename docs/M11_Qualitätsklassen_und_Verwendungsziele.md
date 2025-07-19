# M11 – Qualitätsklassen & Verwendungsziele

## 🧭 Ziel

M11 bietet ein Schema zur **Einschätzung von Qualität und Nutzungsabsicht** für alle im FRUDEK-System erfassten Inhalte. Ziel: Inhalte gezielt nach Reifegrad, Genauigkeit oder Einsatzform differenzieren können.

---

## 🎯 Qualitätsstufen

| Stufe | Bedeutung | Beispiel |
|-------|-----------|----------|
| Q0 | unfertig / Idee | Entwurf, Brainstorm |
| Q1 | roh nutzbar | Markdown ohne Attribution |
| Q2 | dokumentiert | vollständiges YAML, korrekt lizenziert |
| Q3 | publikationsreif | formal geprüft, vollständig dokumentiert |

---

## 🎯 Verwendungsziele

| Ziel | Beschreibung |
|------|--------------|
| 👨‍🏫 Lernzweck | interne Erprobung, Studien, Feedback |
| 🧪 Testsystem | temporärer Einsatz in Prototypen |
| 📚 Doku | interne oder externe Dokumentation |
| 📦 Distribution | Veröffentlichung als offizielles Asset |

---

## 🔄 Kombination mit M10

Ein Snippet kann z. B. folgende Metadaten tragen:

```yaml
---
quality: Q2
reuse: R2
purpose: "Doku"
license: CC BY-SA 4.0
---
```

---

## 🔗 Verbindungen

- basiert auf: M6, M9, M10  
- wird verwendet in: M12, M13

---