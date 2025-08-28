# M9 – Attribution & Quellenkennzeichnung

## 🎯 Ziel
M9 beschreibt die Regeln und Empfehlungen zur **transparenten Nennung von Urhebern, Quellen und Bearbeitungsständen** innerhalb von CONVAI.  
Ziel ist die rechtlich und ethisch korrekte **Zuschreibung von Inhalten**, egal ob von Menschen oder KI erstellt.

---

## 📌 Attributionsarten

| Art | Beschreibung | Beispiel |
|-----|--------------|----------|
| 👤 **Namentlich** | mit Personen- oder Projektnamen | „nach Sebastian Besold, 2025“ |
| 🔗 **Verlinkt** | mit direkter URL oder Quellpfad | `source: github.com/user/file.md` |
| 🧠 **KI-generiert** | klarer Hinweis auf Modellnutzung | „Erstellt durch GPT-5“ |
| 🧾 **Modular** | mit YAML-Feld am Modulbeginn | `attribution: CC BY-SA 4.0 – Sebastian` |

---

## 🧰 Tools & Techniken

- YAML-Feld `source`, `by`, `model`, `license`  
- Direktlinks zu Quellprojekten  
- Lizenzangaben (CC, MIT, GNU, …)  

```yaml
---
source: "https://github.com/xyz/projekt"
by: "Sebastian Besold"
model: GPT-5
license: CC BY 4.0
reuse: R2
---

# ⚖️ Warum Attribution wichtig ist

- ⛑️ schützt Urheberrechte und fördert Vertrauen  
- 🔍 ermöglicht Rückverfolgbarkeit und Qualitätssicherung  
- 🧠 unterscheidet KI-Output von menschlichen Beiträgen  
- 📚 hilft bei akademischer Nachvollziehbarkeit  

---

# 🔗 Verbindungen

- basiert auf: M6, M7  
- verwendet in: M10, M12  
- optional gekoppelt mit: M13 (Visualisierung)  
