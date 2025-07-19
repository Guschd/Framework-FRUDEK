# M6 – Lizenzlogik & Reuse-Klassen

## 🧭 Ziel

M6 beschreibt, wie Inhalte innerhalb von FRUDEK rechtlich und funktional freigegeben werden können. Es legt Lizenzarten fest, definiert Wiederverwendungs-Klassen (Reuse-Typen) und erklärt, wie Inhalte für andere Projekte, Tools oder Modelle bereitgestellt werden dürfen – oder bewusst nicht.

Das Modul stellt sicher, dass alle Outputs korrekt gekennzeichnet, nachvollziehbar attribuiert und bei Bedarf automatisiert weiterverwendbar sind.

---

## 🏷️ Lizenzklassen (empfohlene Standards)

### ⚖️ CC BY 4.0  
- **Was?** Creative Commons mit Namensnennung  
- **Erlaubt:** Veränderung, Weitergabe, kommerzielle Nutzung  
- **Pflicht:** Urheber muss genannt werden  
- **Einsatz bei:** Designsnippets, Texte, Templates

### 🚫 CC BY-NC 4.0  
- **Was?** Creative Commons mit Namensnennung, **nicht kommerziell**  
- **Erlaubt:** Nutzung, Veränderung für private oder gemeinnützige Zwecke  
- **Verboten:** kommerzielle Weiterverwertung  
- **Einsatz bei:** experimentellen Prompts, Prototypen

### 🧪 GNU GPL v3  
- **Was?** Freie Softwarelizenz (GNU General Public License Version 3)  
- **Erlaubt:** Nutzung, Veränderung, Verbreitung unter gleicher Lizenz  
- **Pflicht:** Quelloffenlegung bei Weitergabe  
- **Einsatz bei:** Skripten, Automatisierung, Metaprompts

### 🧷 FRUDEK-Intern (nicht freigegeben)  
- **Was?** Lokale Inhalte ohne externe Freigabe  
- **Einsatz bei:** Zwischenständen, Testversionen, geschützten Daten  
- **Hinweis:** explizit als "nicht freigegeben" markieren

---

## ♻️ Reuse-Klassen

Die Reuse-Klasse legt fest, **wie ein Inhalt wiederverwendet werden darf** – unabhängig von der Lizenz.

| Klasse | Bedeutung | Anwendung |
|--------|-----------|-----------|
| 🔁 **R0 – Einmalnutzung** | nur im Ursprungsprojekt gültig | individuelle Logs, temporäre Bilder |
| 🔁 **R1 – Manuelle Wiederverwendung** | Wiederverwendung nach Prüfung erlaubt | einfache Markdown-Fragmente |
| 🔁 **R2 – Automatisierte Reuse erlaubt** | direkte Einbindung in Tools / KI-Modelle möglich | Templates, modulare Prompts |
| 🔁 **R3 – Referenz-/Trainingsmaterial** | für Schulung, Dokumentation, Modelltraining optimiert | Beispielprojekte, Freigabedatenbanken |

---

## 🧰 Lizenz- und Reuse-Kennzeichnung

### 📁 Im Projektverzeichnis
- Hauptlizenz im Projektordner:  
  `LICENSE.txt` (z. B. GNU GPL v3)

- Lizenzblock in Markdown-Headern oder YAML-Feldern:
  ```yaml
  license: CC BY 4.0
  reuse: R2
  attribution: "Sebastian Besold"
  ```

### 📝 In Snippets oder Einzeldateien
- Jeder wiederverwendbare Code- oder Textblock enthält Lizenz- und Reusehinweise  
- Beispiel am Ende einer `.md`:
  ```markdown
  ---
  Lizenz: CC BY 4.0  
  Wiederverwendung: R2 (automatisiert erlaubt)  
  Quelle: FRUDEK Modul M6
  ```

- Bilddateien erhalten einen eingebetteten Lizenzhinweis (z. B. rechts unten) oder liegen mit Begleitdatei `*.license.md` im selben Ordner

---

## 🧩 Best Practices

- Verwende **so offen wie möglich, so restriktiv wie nötig**  
- Dokumentiere Änderungen an lizenzierten Inhalten immer mit Datum  
- Bei kombinierten Inhalten (z. B. Markdown + Bild + Prompt) alle Bestandteile einzeln lizenzieren

---

## 💡 Prompt- und Snippetbeispiele

**Prompt für Lizenzmarkierung in YAML:**
```yaml
reuse: R2
license: CC BY 4.0
attribution: "Sebastian Besold"
```

**Textbaustein zur Lizenzkennzeichnung in Markdown:**
```markdown
---
Lizenz: CC BY-NC 4.0  
Wiederverwendung: R1 (manuell erlaubt)  
Quelle: Eigene Erstellung im Rahmen von FRUDEK M6
---
```

**Standard-Kommentar für Creative Commons in Readmes:**
```markdown
Dieses Dokument steht unter der Lizenz [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).  
Bitte geben Sie bei Wiederverwendung folgenden Hinweis an:  
„Quelle: FRUDEK-Projekt von Sebastian Besold (2025)“
```

---

## 🔗 Verknüpfung zu anderen Modulen

- basiert auf:  
  → M5 – Snippetverwaltung & Metadaten  
  → M3 – Projektarten & Dokumentationstypen

- wird verwendet in:  
  → M10 – Modellbibliothek & Freigabe  
  → M9 – Transparente Attribution & Prozesspfade  
  → M7 – Konfliktlösung bei Lizenzüberschneidung (z. B. bei CC vs. GPL)

---