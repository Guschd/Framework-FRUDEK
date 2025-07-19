# M14 – API-Logik & Exportstruktur

## 🧭 Ziel

Modul M14 legt die technischen und konzeptionellen Grundlagen für die **API-Anbindung von FRUDEK** sowie für die automatisierte **Export- und Verteilstruktur**. Es schafft die Voraussetzung für Schnittstellen zu externen Tools, automatisierte Snippetverteilung und Metadatenzugriff.

---

## 🔌 API-Ziele

| Ziel | Beschreibung |
|------|--------------|
| 📤 Snippet-Export | Einzel- oder Paketweise Bereitstellung als JSON, YAML, Markdown |
| 📥 Snippet-Import | Annahme validierter Fremdsnippets mit Freigabeprüfung |
| 🔍 Metadatenzugriff | API-Endpunkte für Suche, Filter und Reuse-Historie |
| 🔄 Repositorysync | Automatisierter Sync mit GitHub o.ä. |
| 📊 Lizenzabfragen | Filterung nach Lizenz, Qualität oder Herkunft |

---

## 🧱 API-Struktur (Beispiel)

```yaml
GET /api/snippets/{id}
→ returns: {
  id: "S14_001",
  module: "M10",
  license: "CC-BY 4.0",
  origin: "user",
  validated: true,
  created_at: "2025-07-18"
}
```

```http
POST /api/snippets
Body: {
  content: "...",
  metadata: { module: "M7", license: "GPL-3.0", ... }
}
```

---

## 📁 Exportstruktur

| Format | Zweck |
|--------|-------|
| `.md` | Menschlich lesbare Projekt- und Snippetstruktur |
| `.yaml` / `.json` | Maschinenlesbare Snippetstruktur |
| `.zip` | Gesamtarchiv für Projekte oder Modulsets |
| `.pdf` (optional) | Dokumentationsauszüge für Lesefluss |

---

## 🛡️ Sicherheit & Kontrolle

- Authentifizierung über Token oder Projekt-ID  
- Exportfilterung nach Freigabestatus (M10)  
- Eingeschränkter Schreibzugriff (nur validierte Quellen)  
- Lizenzprüfung durch M6 + M12  

---

## 🔗 Verbindungen

- basiert auf: M5, M6, M10, M12  
- Voraussetzung für: M15 (Netzwerkweite Snippetverteilung)  
- optional kombinierbar mit M13 (Visual-API)

---