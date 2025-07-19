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
