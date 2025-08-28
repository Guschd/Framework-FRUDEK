# M11 – Technisch-Emotionale Eskalationen

## 🧭 Zielsetzung

Modul 11 identifiziert typische Szenarien, in denen technische Probleme eine emotionale Dynamik entwickeln – sowohl im Gespräch zwischen Mensch und KI als auch im klassischen IT-Support.  
Ziel ist es, diese eskalierenden Situationen frühzeitig zu erkennen, zu entschärfen und strukturiert zu dokumentieren.

---

## 🔍 Hintergrund

Viele Anfragen, die an Supportsysteme oder KI-Systeme gestellt werden, sind durch Frust, Zeitdruck oder Unsicherheit geprägt.  
Dieses Modul stellt konkrete Beispiele solcher Konversationen bereit, analysiert die emotionale wie technische Komponente und zeigt auf, wie mit geeigneten Antworten reagiert werden kann.

---

## 🧪 Strukturierte Testfälle (Frage-Antwort-Szenarien)

Jeder Testfall folgt dem Schema:

- **Fragestellung (Input)**
- **Interpretation / Bewertung**
- **Empfohlene Reaktion**
- **Kommentar / Erfahrungswert**

---

### ✅ Testfall A

**Input:**  
„Nix geht mehr, mach was!“

**Interpretation:**  
Emotional aufgeladener Notruf. Kein konkreter Fehler beschrieben.

**Empfohlene Reaktion:**  
Subtil deeskalierend: „Ok, das klingt nicht gut. Wo bist du gerade und was wolltest du denn machen?“  
Optional humorvoll, wenn Verhältnis bekannt: „Ich hab's für dich kaputt gemacht, damit du früher nach Hause kannst.“

**Kommentar:**  
Frust, Unsicherheit und Dringlichkeit in einem Satz. Fingerspitzengefühl gefragt.

---

### ✅ Testfall B

**Input:**  
„Der Export geht nicht mehr.“

**Interpretation:**  
Stark kontextabhängig. „Export“ kann viele Bedeutungen haben. Wer fragt?

**Empfohlene Reaktion:**  
Nutzerkontext rekonstruieren: „Geht es um die Buchhaltung, Zeiterfassung oder einen Datenbankexport?“

**Kommentar:**  
Personalerin = Zeiterfassung, Buchhaltung = Faktur oder DATEV. Rolle gibt Hinweis auf Inhalt.

---

### ✅ Testfall C

**Input:**  
„Ich hab den Button vermisst!“

**Interpretation:**  
UI-Änderung, Update, AutoSave oder Speicherprozess wurde entfernt oder verändert.

**Empfohlene Reaktion:**  
Ablauf rekonstruieren, neue Speicherlogik erklären, ggf. Pfad zur Datei zeigen.

**Kommentar:**  
Ähnlich wie Spiele mit AutoSave – Änderung wird als Kontrollverlust wahrgenommen.

---

### ✅ Testfall D

**Input:**  
„Ich hab’s kaputt gemacht…“

**Interpretation:**  
Emotionale Komponente. Häufig Schuldeingeständnis aus Überforderung.

**Empfohlene Reaktion:**  
Beruhigend & niedrigschwellig antworten: „Ist halb so wild. Gib mir mal deinen PC-Namen, ich schau drauf.“

**Kommentar:**  
Typischer Supportfall, der Nähe und Verständnis erfordert. Ironie manchmal hilfreich.

---

### ✅ Testfall E

**Input:**  
„Ich weiß nicht was passiert ist…“

**Interpretation:**  
Passiert bei Datenverlust, versehentlichem Löschen, falschem Ordner etc.

**Empfohlene Reaktion:**  
„Kannst du dich erinnern, was du zuletzt gemacht hast?“ – Schrittweise Annäherung.

**Kommentar:**  
Technisch meist banal, menschlich aber mit Stress verbunden.

---

### ✅ Testfall F (entfernt)

Dieser Fall wurde gestrichen.

---

### ✅ Testfall G

**Input:**  
„Der Drucker lebt sein eigenes Leben!“

**Interpretation:**  
Humorvolle Umschreibung für sporadische oder unerklärliche Fehler.

**Empfohlene Reaktion:**  
„Welche Druckaufträge kommen nicht an? Welche LED leuchtet? Welche Meldung zeigt er?“  
Techniknah mit Humor kombinieren.

**Kommentar:**  
Von falschem Fach über falschen Drucker bis zu Office-Stromausfall – Klassiker.

---

### ✅ Testfall H

**Input:**  
„Ich seh nix am Beamer!“

**Interpretation:**  
Typischer Fall bei falscher Auflösung, inkompatibler Verbindung oder Treiberfehler.

**Empfohlene Reaktion:**  
Abfrage der Tastenkombinationen (z. B. Windows+P), externe Anzeige, Auflösung prüfen.

**Kommentar:**  
Häufig nach Neuinstallation oder fehlender Hersteller-Treiber.

---

### ✅ Testfall I

**Input:**  
„Daten werden gleich bereitgestellt…“

**Interpretation:**  
Zwischen „gleich“ (1 min) und „gleich“ (1 Monat) liegt die Unsicherheit.

**Empfohlene Reaktion:**  
Zeitfenster abfragen: „Wann haben Sie die letzte Rückmeldung erhalten?“  
Prognose nach FRUDEK 9.6 (Evidenzbasierte Zeitprognose) ggf. anhängen.

**Kommentar:**  
Zeitgefühl differiert stark. Erwartungsmanagement extrem wichtig.

---

### ✅ Testfall J

**Input:**  
„Hast du mal 5 Min für mich?“

**Interpretation:**  
Meist unterschätzter Trigger. Erwartet sofortige Lösung.

**Empfohlene Reaktion:**  
Priorisierung ansprechen: „Ich schau gern rein. Ist es dringend oder kann ich mich in 30 Min melden?“

**Kommentar:**  
Typischer Burnout-Treiber im menschlichen Support. Auch für KI ein Risikofaktor bei Ressourcenpriorisierung.

---

## 🧩 Modulbezug

- **Verknüpft mit:**  
  - **M2 (Kontextauflösung)**  
  - **M4 (Fehlerquellenmodellierung)**  
  - **M6 (Semantische Feinjustierung)**  
  - **M9 (Attribution & Transparenz)**  
  - **M13 (Visualisierung von Prozesspfaden)**

- **Optional verwendbar mit:**  
  - Eskalationsindikator / Emotionsparser  
  - Reaktionsmodul für situatives Framing  

---

## 💬 Empfehlung

Dieses Modul kann als Grundlage für ein Emotionserkennungs-Plugin dienen, welches sprachliche Muster erkennt und KI-typische Antwortstrategien auf das passende Eskalationslevel abstimmt.

---

## 🛠️ YAML-Metadaten

```yaml
---
modul: M11
title: Technisch-Emotionale Eskalationen
author: Sebastian Besold / GPT-4o
license: CC BY 4.0
version: 1.0
linked_modules: [M2, M4, M6, M9, M13]
last_updated: 2025-08-07
---
