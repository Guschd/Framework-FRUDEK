# 📦 FRUDEK Modul M10 – Freigabe & Templateverwaltung

## 🧠 Modulbeschreibung
M10 definiert die Prozesse zur **Nutzerfreigabe** und zur **Verwaltung wiederverwendbarer Vorlagen** innerhalb des FRUDEK-Systems.  
Es ermöglicht, dass Inhalte (z. B. STL-Dateien, Textbausteine, Artikel, Code-Snippets) nach ausdrücklicher Zustimmung des Urhebers in eine **Template-Bibliothek** aufgenommen werden.  
Diese Bibliothek dient zur **Beschleunigung zukünftiger Anfragen** und zur **Standardisierung wiederkehrender Outputs**.

Während M9 sich auf die **Zuschreibung und Quellenkennzeichnung** konzentriert, regelt M10 die **rechtliche und organisatorische Freigabe** sowie die **Kategorisierung und Wiederverwendung** dieser Inhalte.

---

### 🎯 Ziele
- **Rechtssichere Freigabe** von Nutzer- und KI-Outputs  
- Aufbau einer **durchsuchbaren Template-Bibliothek**  
- **Metadatenstruktur** zur schnellen Wiederverwendung  
- Effizienzsteigerung durch **Standardisierung** wiederkehrender Ergebnisse  
- Sicherstellung, dass Inhalte **nur nach ausdrücklicher Zustimmung** freigegeben werden

---

### 🔍 Herausforderungen
- Klare Abfrage der **Nutzerzustimmung**  
- Trennung zwischen **öffentlichen, internen und privaten Templates**  
- Vermeidung ungewollter Preisgabe sensibler Inhalte  
- Kategorisierung und Verschlagwortung für effiziente Wiederverwendung  
- Synchronisation mit Attribution (M9), ohne die Module zu vermischen

---

## 🧪 Testfälle

### 🧪 Testfall 1 – STL-Freigabe
**Eingabe:** „Kannst du die Datei in die Bibliothek aufnehmen?“  
**Analyse:** Prüfen, ob Urheber eindeutig ist und Rechte zur Weitergabe vorliegen.  
**Strategie:** Abfrage von Lizenz, Quelle und Nutzungsumfang.  

---

### 🧪 Testfall 2 – Textsnippet-Wiederverwendung
**Eingabe:** „Du kannst gerne meine Formulierung weiterverwenden.“  
**Analyse:** Zustimmung liegt vor, aber Kontext prüfen (Projekt, Version).  
**Strategie:** Template in Bibliothek ablegen, mit Metadaten (Autor, Datum, Tags).  

---

### 🧪 Testfall 3 – Unklare Zustimmung
**Eingabe:** „Mach damit, was du willst.“  
**Analyse:** Ethisch und rechtlich unscharf; muss präzisiert werden.  
**Strategie:** Rückfrage zur genauen Art der Weiterverwendung (öffentlich/privat).  

---

## 📂 Praxisbeispiele

### 📂 Beispiel 1 – 3D-Designprojekt Drachenboot
**Ausgangslage:** Nutzer stellt STL-Datei zur Verfügung, erlaubt Wiederverwendung.  
**Freigabeprozess:**  
1. Bestätigung, dass Nutzer Urheber ist  
2. Abfrage gewünschter Lizenz (z. B. CC BY-SA)  
3. Aufnahme in Kategorie „3D-Gehäuse – Raspberry Pi“ mit Metadaten  
4. Querverweis auf M9 zur Attribution

---

### 📂 Beispiel 2 – Textbaustein aus Supportfall
**Ausgangslage:** Nutzer erlaubt Verwendung einer Ticketantwort als Vorlage.  
**Freigabeprozess:**  
1. Entfernung personenbezogener Daten  
2. Aufnahme in „Support-Templates – Kundenkommunikation“  
3. Schlagwortvergabe für schnelle Auffindbarkeit

---

## 🛠 Hinweise für AI-Trainer
- **Immer aktive Zustimmung einholen** – keine stillschweigende Annahme  
- **Sensiblen Inhalt vor Aufnahme anonymisieren**  
- **Metadaten sauber pflegen** (Autor, Datum, Kategorie, Tags, Lizenz)  
- Bibliothek so strukturieren, dass sie **schnell durchsucht** werden kann  
- **M9-Attribution** und **M10-Freigabe** getrennt dokumentieren, aber verlinken
