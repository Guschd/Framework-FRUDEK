# M3 – Projektarten & Dokumentationstypen

## 📌 Ziel
Dieses Modul beschreibt die verschiedenen Typen von Kreativprojekten, die mit KI-Unterstützung entstehen können, sowie die jeweils geeigneten Dokumentationsformen innerhalb von FRUDEK. Ziel ist eine standardisierte Struktur, die sowohl technisch als auch semantisch nachvollziehbar bleibt.

---

## 🔧 Projektarten (Typisierung)

| Typ | Beschreibung | Beispiele |
|-----|--------------|-----------|
| **Hardware-Prototyping** | CAD-/STL-getriebene Entwürfe mit 3D-Druck oder Elektronikbezug | Raspberry-Pi-Gehäuse, Sensorhalterungen |
| **Texterzeugung & Strukturierung** | Generierung strukturierter Inhalte | wissenschaftliche Outline, Promptsammlungen |
| **Prompt-Replikation** | Erstellung übertragbarer Eingabe-/Antwortmuster | KI-Prompts für Midjourney, GPT, Sora |
| **Dokumentation & Reports** | Generierte Protokolle oder Statusdokumente | Zeitverläufe, Worklogs, Change-Logs |
| **Kombinationsprojekte** | Mischung aus Text, Bild und Logikstruktur | visuelle Lizenzwahl, codierte Metaprompts |

---

## 📘 Dokumentationstypen

| Typ | Zweck | Format | Ort |
|-----|-------|--------|-----|
| **README.md** | Überblick pro Modul oder Projekt | Markdown | `main/M*/README.md` |
| **Logbuch** | Zeitlicher Verlauf & Statusupdates | `.md` oder `.csv` | `docs/` oder `examples/` |
| **Snippets** | Wiederverwendbare Prompt- oder Antwortteile | `.txt`, `.md`, JSON | `snippets/` |
| **Beispieldateien** | Konkrete Anwendungen / Proof of Concept | `.md`, `.png`, `.stl`, `.py` | `examples/` |
| **Nutzerfreigaben** | Freigegebene Outputs inkl. Lizenz | `.md`, `.json` | `library/` (optional) |

---

## 🧩 Interaktion mit anderen Modulen

- Verweist auf M5 („Snippet-Verwaltung“) und M10 („Freigaben“)
- Grundlage für spätere Automatisierung der Kategorisierung

---

## 📎 Beispielanwendung

Das Drachenboot-Projekt (siehe `examples/`) ist ein Typ: **Hardware-Prototyping mit begleitender Status-Dokumentation**, dokumentiert als `M1`, `M2`, `M3`, `M9`, `M10`.
