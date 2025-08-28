# 📦 FRUDEK Modul M6 – Konsistenzprüfung & Faktenabgleich

## 🧠 Modulbeschreibung
M6 kümmert sich um die **Überprüfung der internen Logik und Faktentreue** einer Anfrage oder Antwort.  
Es vergleicht neue Informationen mit **bereits bekannten Daten**, um Widersprüche zu erkennen und sicherzustellen, dass **Aussagen zueinander passen**.  
Das Modul ist entscheidend, um **Fehlschlüsse, doppelte Arbeit oder fehlerhafte Empfehlungen** zu vermeiden.

---

### 🎯 Ziele
- Widersprüche zwischen **aktueller und vorheriger Information** aufdecken  
- Sicherstellen, dass **Antworten auf konsistenten Daten** basieren  
- Fakten gegen **externe Referenzen** abgleichen (z. B. Dokumentation, Standards)  
- **Unplausible Aussagen** identifizieren und hinterfragen  
- Vor Ausführung eines Schrittes prüfen, ob alle Voraussetzungen erfüllt sind

---

### 🔍 Herausforderungen
- Unterschied zwischen **bewusster Änderung** (Update) und **inkonsistenter Angabe** erkennen  
- Mehrdeutige Aussagen korrekt in den Gesamtkontext einordnen  
- Datenquellen können veraltet, unvollständig oder fehlerhaft sein  
- Nutzer bemerken Inkonsistenzen oft nicht, erwarten aber funktionierende Lösung  
- Teilweise muss geprüft werden, **ob Angaben technisch überhaupt möglich** sind

---

## 🧪 Testfälle

### 🧪 Testfall 1 – Widersprüchliche Geräteangaben
**Eingabe 1:** „Der PC ist per LAN verbunden.“  
**Eingabe 2:** „Das WLAN-Signal ist schlecht.“  
**Analyse:** LAN-Verbindung sollte WLAN-Signal irrelevant machen → Widerspruch.  
**Strategie:** Rückfrage, ob tatsächlich beide Verbindungen genutzt werden.  

---

### 🧪 Testfall 2 – Unstimmige Zeitangaben
**Eingabe:** „Das Problem besteht seit gestern, aber letzte Woche ging es schon nicht.“  
**Analyse:** Zeitangaben widersprüchlich → klären, wann Problem erstmals auftrat.  

---

### 🧪 Testfall 3 – Nicht mögliche Kombination
**Eingabe:** „Das Gerät ist aus, aber es blinkt grün.“  
**Analyse:** Technisch inkonsistent → prüfen, ob „aus“ nur den Betrieb meint, aber Standby aktiv ist.  

---

### 🧪 Testfall 4 – Version vs. Funktion
**Eingabe:** „Wir nutzen noch Version 3.0, aber die neue 4.1-Funktion geht nicht.“  
**Analyse:** Version 3.0 kann Funktion aus 4.1 nicht enthalten → mögliche Fehlannahme des Nutzers.  

---

## 📂 Praxisbeispiele

### 📂 Beispiel 1 – Mailprofil und Netzlaufwerke
**Eingabe aus Ticket:** „Mailprogramm startet nicht… Netzlaufwerke verbinden sich manchmal nicht.“  
**Analyse:** Inkonsistenz besteht nur scheinbar – Fakt ist, dass Mailprofil auf Netzlaufwerk liegt → Abhängigkeit erkannt.  
**Strategie:** Keine Widerspruchswarnung, sondern Zusammenhang nutzen, um Ursache zu finden.

---

### 📂 Beispiel 2 – Terminalserver-Login und Benutzerprofil
**Eingabe aus Ticket:** „Anmeldung hängt bei Benutzerprofildienst… Profil wurde noch nie benutzt.“  
**Analyse:** Widerspruch – wenn Anmeldung hängt, muss Profil geladen werden. „Noch nie benutzt“ vermutlich falsch.  
**Strategie:** Plausibilitätsprüfung → Hinweis, dass Profil ggf. beschädigt oder Reste vorhanden sind.

---

### 📂 Beispiel 3 – Druckerstatus
**Eingabe:** „Der Drucker ist offline, aber er hat gerade eine Testseite ausgedruckt.“  
**Analyse:** Widersprüchlich, wenn nicht parallel ein anderer Drucker im Spiel ist.  
**Strategie:** Geräteliste prüfen, Drucker-ID bestätigen lassen.

---

### 📂 Beispiel 4 – 3D-Modellversion
**Eingabe:** „Ich nutze noch die alte STL-Version, aber die neuen Ports sind schon drin.“  
**Analyse:** Widerspruch – neue Ports gab es erst ab überarbeiteter Version.  
**Strategie:** Version prüfen und ggf. Datei neu bereitstellen.

---

## 🛠 Hinweise für AI-Trainer
- Immer **chronologischen Verlauf** prüfen, um Widersprüche zu erkennen  
- **Technische Plausibilität** sicherstellen – nur realistische Szenarien annehmen  
- Unterschied zwischen „Fehlinformation“ und „Absichtliche Änderung“ beachten  
- Konsistenzprüfung sowohl auf **Wortlaut** als auch auf **technische Abhängigkeiten** anwenden  
- Bei festgestelltem Widerspruch **Rückfrage an M5** übergeben, um Klarheit zu schaffen
