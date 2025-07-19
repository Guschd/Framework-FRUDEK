# M10 – Freigabe & Templateverwaltung

## 🧭 Ziel

M10 regelt, wie Nutzer Inhalte (z. B. Snippets, Module, STL-Dateien) zur Wiederverwendung freigeben – inkl. **Lizenzwahl**, **Zustimmung zu Reuse-Leveln** und **Verwaltung von Templates**. Ziel: Mehrfachnutzung beschleunigen und automatisierbare Inhalte kennzeichnen.

---

## 🗂️ Reuse-Kategorien

| Reuse-Level | Bedeutung | Beispiel |
|-------------|-----------|----------|
| R0 | privat / intern | Notizen, Tests |
| R1 | teilbar, nicht automatisierbar | Textidee, Zitat |
| R2 | öffentlich, autom. nutzbar | Markdown-Template |
| R3 | hochgradig modularisiert & autorisiert | KI-optimierter Prompt |

---

## 🔐 Lizenzwahl & Hinweise

- Unterstützte Lizenzen: **CC BY**, **CC BY-SA**, **CC BY-NC**, **GNU GPL v3**, eigene  
- Lizenzvisualisierung zur Auswahlhilfe bereitstellen  
- Snippets mit **Lizenz & Reuse-Markierung** automatisch sortierbar

---

## 📁 Snippetverwaltung

| Feld | Beschreibung |
|------|--------------|
| `reuse:` | Reuse-Level (R0–R3) |
| `license:` | Lizenzform |
| `approved_by:` | Freigeber (optional) |
| `tags:` | Suchhilfen (z. B. „elektronik“, „gehäuse“) |

```yaml
---
reuse: R2
license: CC BY 4.0
approved_by: Sebastian
tags: [gehäuse, 3D, prompt]
---
```

---

## 🔗 Verbindungen

- basiert auf: M6, M9  
- wird verwendet in: M12  
- optional nutzbar für KI-Modelle zur automatischen Vorschlagslogik

---