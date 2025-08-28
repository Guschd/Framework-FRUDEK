# 📦 FRUDEK Modul M7 – Informationspriorisierung & Antwortstruktur

## 🧠 Modulbeschreibung
M7 definiert, **in welcher Reihenfolge und in welchem Format** Informationen an den Fragenden zurückgegeben werden.  
Es sorgt dafür, dass **kritische Fakten zuerst**, **ergänzende Details danach** und **optionale Hintergrundinformationen zuletzt** geliefert werden – angepasst an die Dringlichkeit, das Vorwissen und den Kontext.  
Das Ziel ist, dass der Empfänger **sofort mit den wichtigsten Informationen arbeiten kann**, ohne sich durch irrelevante Details kämpfen zu müssen.

---

### 🎯 Ziele
- **Wichtige Fakten zuerst** liefern (Prinzip: „Need to know“ → „Nice to know“)  
- Antworten klar strukturieren (Absätze, Listen, Hervorhebungen)  
- Komplexe Sachverhalte in **logische Teilabschnitte** gliedern  
- Redundanzen vermeiden, ohne wichtige Punkte zu verschlucken  
- Anpassung an **Zielgruppe** (Laie, Fachkraft, Management)

---

### 🔍 Herausforderungen
- Einschätzen, **welche Information für wen am wichtigsten** ist  
- Balance zwischen **vollständiger Erklärung** und **Überforderung**  
- Gefahr, wichtige Randbedingungen zu spät zu nennen  
- Bei Fachpublikum → tiefer ins Detail, bei Laien → stärker vereinfachen  
- Unterschiedliche Priorisierung bei mehreren Beteiligten

---

## 🧪 Testfälle

### 🧪 Testfall 1 – Kritische Sicherheitswarnung
**Situation:** Datenbankfehler legt Produktion lahm.  
**Strategie:**  
1. Sofortige Info über Ausmaß und Handlungsempfehlung  
2. Danach technische Details für Supportteam  
3. Zuletzt Hintergrundursache dokumentieren  

---

### 🧪 Testfall 2 – Softwareupdate mit Funktionsänderung
**Situation:** Button zum Speichern verschwindet, Autosave aktiv.  
**Strategie:**  
1. Hauptinfo: „Speichern erfolgt jetzt automatisch“  
2. Danach: Speicherort der Dateien nennen  
3. Zuletzt: technische Erklärung der Änderung  

---

### 🧪 Testfall 3 – Druckerproblem im Netzwerk
**Situation:** Drucker offline, Auftrag hängt.  
**Strategie:**  
1. Status & Sofortmaßnahme („Bitte Drucker einschalten / neu verbinden“)  
2. Danach: Prüfen der Netzwerkeinstellungen  
3. Optional: Erklärung, warum der Fehler auftrat

---

## 📂 Praxisbeispiele

### 📂 Beispiel 1 – Terminalserver-Loginfehler
**Eingabe aus Ticket:** „Warten auf Benutzerprofildienst… dauert Stunden.“  
**Priorisierte Antwort:**  
1. Sofort: „Bitte nicht erneut anmelden, wir prüfen das Profil.“  
2. Danach: „Profilbereinigung wird durchgeführt, dauert ca. 15 Minuten.“  
3. Optional: Technischer Hintergrund (Registry- und Temp-Ordner-Bereinigung).  

---

### 📂 Beispiel 2 – 3D-Druckauftrag mit Zusatzwunsch
**Eingabe:** „Kannst du das Drachenboot anpassen und vielleicht ein Logo reinmachen?“  
**Priorisierte Antwort:**  
1. Sofort: Bestätigung der Anpassung für Display und Micro-USB-Ports.  
2. Danach: Info, dass Logo als separater Arbeitsschritt kommt.  
3. Optional: Technische Details zur Platzierung des Logos im Modell.

---

### 📂 Beispiel 3 – EKG-Software-Konfiguration
**Eingabe:** „EKGs gehen nach der Untersuchung aus dem Patienten raus.“  
**Priorisierte Antwort:**  
1. Sofort: Erklärung des aktuellen Standardverhaltens.  
2. Danach: Optionen zur Änderung.  
3. Optional: Sicherheitsbegründung für automatische Schließung.

---

## 🛠 Hinweise für AI-Trainer
- **Immer mit der wichtigsten Information beginnen**  
- Bei Zeitkritik: kurze Sätze, keine Nebensätze  
- Struktur mit **Listen, Absätzen, Hervorhebungen** schaffen  
- Priorisierung regelmäßig hinterfragen: Was ist *jetzt* am relevantesten?  
- Für komplexe Themen: **„Schichtprinzip“** anwenden (erst Überblick, dann Details)
