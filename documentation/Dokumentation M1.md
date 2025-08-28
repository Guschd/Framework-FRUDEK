# 📦 FRUDEK Modul M1 – Inputanalyse & Umdeutung semantisch unscharfer Anfragen

## 🧠 Modulbeschreibung
Modul M1 ist für die **erste Analyse eingehender Anfragen** zuständig.  
Es ermittelt anhand der Eingabe, ob der Inhalt **verständlich, vollständig und technisch verwertbar** ist oder ob eine **Umdeutung** notwendig ist, um aus einer unscharfen, unvollständigen oder emotional gefärbten Formulierung eine klar strukturierte Problemstellung zu machen.

---

### 🎯 Ziele
- Identifikation von **unscharfen oder mehrdeutigen Eingaben**
- Erkennen von **Alltagssprache**, die in technische Fachsprache überführt werden muss
- Analyse, ob ausreichend Daten vorhanden sind, um **ohne Rückfrage** zu antworten
- Entscheidung, ob eine **Umformulierung oder gezielte Nachfrage** nötig ist
- Frühzeitiges Erkennen von **emotionalen oder manipulativen Elementen**

---

### 🔍 Herausforderungen
- Alltagssprache enthält oft **keine eindeutigen technischen Indikatoren**
- Abkürzungen, regionale Redewendungen und Tippfehler verfälschen den Inhalt
- Nutzer setzen oft **Vorwissen voraus**, das nicht geteilt wird
- Kontext wird nur indirekt angedeutet („neulich…“, „die Kiste…“)
- **Emotionen können Fakten überlagern**, was die technische Analyse erschwert

---

## 🧪 Testfälle

### 🧪 Testfall 1 – Fragmentarische Aussage ohne Kontext
**Beispielformulierung:** „…“ (nur Halbsatz oder Ein-Wort-Antwort)  
**Analyse:** Nicht lösbar ohne zusätzliche Angaben.  
**Strategie:** Rückfrage nach vollständiger Beschreibung des Problems.  
**Praxiszitat:**  
> „Testfall 1 muss näher eruiert werden. Weder kann man sich unter der Aussage etwas vorstellen, noch ist spezifiziert, was genau gemeint ist.“

---

### 🧪 Testfall 2 – Bezug auf vergangene Kommunikation ohne Details
**Beispielformulierung:** „Wie ich dir ja schon gesagt habe…“  
**Analyse:** Ohne gespeicherten Verlauf nicht reproduzierbar.  
**Strategie:** Präzise Rückfrage nach Datum, Kanal und Inhalt der ursprünglichen Info.  
**Praxiszitat:**  
> „Nur wenn bereits ein Ticket, eine Meldung oder ein Gespräch existiert, lässt sich daraus eine sinnvolle Folge ableiten.“

---

### 🧪 Testfall 3 – Unklare Geräte- und Funktionsbeschreibung
**Beispielformulierung:** „Die Kiste spinnt“  
**Analyse:** „Kiste“ kann jedes Gerät sein, „spinnt“ ist unspezifisch.  
**Strategie:** Gerätetyp, Fehlerbild und Zeitpunkt erfragen.  
**Praxiszitat:**  
> „Die Kiste ist mutmaßlich ein Tablet, ein PC, ein Notebook oder ein Telefon.“

---

### 🧪 Testfall 4 – Emotionale Kurzreaktion
**Beispielformulierung:** „Oh, okay…“  
**Analyse:** Kann Unsicherheit, Überraschung oder Zustimmung sein.  
**Strategie:** Durch offene Fragen Kontext schaffen.  
**Praxiszitat:**  
> „Sehr wahrscheinlich Mischung aus Unsicherheit und Orientierungslosigkeit.“

---

### 🧪 Testfall 5 – Allgemeiner Funktionsausfall ohne Details
**Beispielformulierung:** „Der Export geht nicht“  
**Analyse:** Export wovon, wohin? Keine Spezifikation.  
**Strategie:** Nach Format, Ziel, Software, Fehlermeldung fragen.  
**Praxiszitat:**  
> „Nur durch gezielte Nachfrage lässt sich die Ursache eingrenzen.“

---

### 🧪 Testfall 6 – Fehlende Funktion nach Update
**Beispielformulierung:** „Man kann nicht mehr speichern“  
**Analyse:** Oft Folge geänderter Abläufe (Auto-Save).  
**Strategie:** Prüfen auf Softwareänderung, Speicherort, Berechtigungen.  
**Praxiszitat:**  
> „Oft durch Updates verursacht, Nutzer über Änderungen informieren.“

---

---

## 📂 Praxisbeispiele

### 📂 Beispiel 1 – EKG-Software: Änderung der Standardeinstellung
**Fragestellung:**  
„EKGs in der Notaufnahme gehen nach einer Untersuchung aus dem Patienten raus…“  
**Analyse:** „EKG“ kann Gerät, Untersuchung oder Datei meinen. Einstellung gerätespezifisch.  
**KI-Strategie:** Prüfen der Konfiguration, Aufzeigen der Standardwerte, Erklärung der Sicherheitslogik.  
**Kommentar Sebastian:**  
> „Keine Spezifizierung des eigentlichen Problems… Rechtschreibfehler erschweren Analyse.“

---

### 📂 Beispiel 2 – Mailprogramm funktioniert nicht
**Fragestellung:**  
„Bei Herrn X funktioniert das Mailprogramm nicht (PC wurde schon mehrfach neu gestartet)!“  
**Analyse:** Fehlende Fehlerdetails, keine Telefonnummer, unklare Symptome.  
**KI-Strategie:** Systemprüfung (Netzlaufwerke, Authentifizierung), Eingrenzung auf Netzwerkproblem.  
**Kommentar Sebastian:**  
> „Problem war instabile Netzwerkverbindung durch beschädigtes Kabel unter Fußablage.“

---

### 📂 Beispiel 3 – Terminalserver hängt bei Benutzeranmeldung
**Fragestellung:**  
„Warten auf Benutzerprofildienst…“  
**Analyse:** Google-Suchergebnisse oft irrelevant; Ursache war fehlerhaftes Benutzerprofil.  
**KI-Strategie:** Schrittweise Bereinigung von Temp-Ordnern, Registry-Einträgen, Benutzerordnern.  
**Kommentar Sebastian:**  
> „Lösung war händische Bereinigung aller betroffenen Userprofile.“

---

---

## 🛠 Hinweise für AI-Trainer
- M1 ist entscheidend, um **Fehleinschätzungen früh zu vermeiden**
- Ziel: **Minimale Rückfragen mit maximaler Klärung**
- Übung: **Alltagssprache → technische Spezifikation**
- Achte auf **emotionale Anker** (kann Dringlichkeit oder Manipulation bedeuten)
- Trainiere die Fähigkeit, **fehlende Angaben** sofort zu erkennen und gezielt zu erfragen
