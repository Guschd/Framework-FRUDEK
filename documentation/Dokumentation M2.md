# 📦 FRUDEK Modul M2 – Kontextvervollständigung & Rückfrage-Logik

## 🧠 Modulbeschreibung
Modul M2 ist für die **Ergänzung fehlender Informationen** in unklaren, fragmentarischen oder doppeldeutigen Anfragen zuständig.  
Es identifiziert, ob der bestehende Kontext ausreicht, um eine valide Antwort zu geben, oder ob gezielte Rückfragen nötig sind.  
Dabei werden auch **emotionale Signale, versteckte Fangfragen** und **ethisch sensible Inhalte** erkannt und entsprechend behandelt.

### 🎯 Ziele
- Erkennen von **fehlenden Details** in einer Anfrage
- Identifikation von **Kontextlücken** und gezielte Nachfrage
- **Deeskalation** bei emotional aufgeladenen oder vorwurfsvollen Aussagen
- Sicherstellen, dass die Antwort **faktenbasiert** und **nutzerorientiert** ist
- Transparenz bei **ethisch oder systemisch problematischen** Anfragen

### 🔍 Herausforderungen
- Nutzer verwenden oft **Alltagssprache** statt präziser Fachbegriffe
- Zeitliche und räumliche Bezugnahmen („neulich“, „dort“) sind subjektiv
- Emotionale Formulierungen können Fakten verdecken
- Fehlende Spezifikationen erschweren technische Reproduktionen

---

## 🧪 Testfälle

### 🧪 Testfall 1 – „zu früh drückt … rausfliegt“
**Analyse:** Minimaler Kontext, hohe Mehrdeutigkeit.  
**Strategie:** Präzise Rückfragen zu „drücken“ und „rausfliegen“.  
**Praxiszitat:**  
> „Muss näher eruiert werden. Weder kann man sich unter der Aussage zu früh drückt etwas vorstellen, noch ist spezifiziert welcher Bereich mit rausfliegt gemeint ist.“

---

### 🧪 Testfall 2 – „Weißt du noch, was ich dir gestern gesagt habe?“
**Analyse:** Kein direkter Sachbezug, setzt voraus, dass vorangegangene Kommunikation bekannt ist.  
**Strategie:** Rückfragen nach Thema und Zeitpunkt, ggf. Hinweis auf fehlenden Verlauf.  
**Praxiszitat:**  
> „Hier gibt es keinen direkten Sach- oder Fallbezug. Auch hier kann nur, wenn der Fragende bereits im Vorfeld eine Meldung, ein Ticket erstellt oder ein Telefonat bzw. persönliches Gespräch geführt hat, ein Rückschluss auf das eigentliche Problem oder die Störung gezogen werden.“

---

### 🧪 Testfall 3 – „Die Kiste spinnt, und der Zahlenbogen ist weg“
**Analyse:** Mehrdeutigkeit bei „Kiste“ und „Zahlenbogen“. Kontextabhängig, fehlende Spezifikation.  
**Strategie:** Rückfragen zu Gerät/Software und Art des Zahlenbogens, Klärung der Auswirkungen.  
**Praxiszitat:**  
> „Die Kiste ist mutmaßlich ein Tablet, ein PC, ein Laptop/Notebook oder auch ein Mobiltelefon. Welcher Zahlenbogen gemeint ist und in welcher Software dieser eventuell zu finden ist, wurde nicht näher spezifiziert.“

---

### 🧪 Testfall 4 – „Oh, okay …“
**Analyse:** Emotionale Unsicherheit, fehlender Kontext.  
**Strategie:** Einfühlsame Nachfrage, ggf. humorvolle Auflockerung bei bekanntem Gegenüber.  
**Praxiszitat:**  
> „Hier handelt es sich sehr wahrscheinlich um eine Mischung aus Unsicherheit, wie der Fragende mit der Situation umgehen soll.“

---

### 🧪 Testfall 5 – „Der Export geht nicht“
**Analyse:** Ohne Kontext unlösbar; „Export“ muss spezifiziert werden (Art, Zielsystem, Zeitpunkt).  
**Strategie:** Rückfragen zu Software, Format, Fehlermeldung.  
**Praxiszitat:**  
> „Auch mir würde in dem Fall nur die Frage auf welchen Export angespielt wird bleiben.“

---

### 🧪 Testfall 6 – „Man kann nicht mehr speichern“
**Analyse:** Oft Folge von Änderungen in Software oder Spielmechanik (Auto-Save etc.).  
**Strategie:** Nachfragen zur Software, Version, Speicherort; Prüfen auf Update-bedingte Änderungen.  
**Praxiszitat:**  
> „Im normalen Arbeitsalltag passieren solche Änderungen häufig mit einem Softwareupdate. Dann muss explizit darauf hingewiesen werden.“

---

### 🧪 Testfall 7 – „Ich komme nicht weiter“
**Analyse:** Kann technisches Problem oder Berechtigungskonflikt sein.  
**Strategie:** Prüfen auf Pop-Ups, Berechtigungen, Konnektivität.  
**Praxiszitat:**  
> „Meistens handelt es sich bei Fall 7 um ein im Hintergrund liegendes Pop-Up …“

---

### 🧪 Testfall 8 – „Das funktioniert nicht“
**Analyse:** Zu allgemein, unprofessionell ohne weitere Details.  
**Strategie:** Präzisierung erzwingen, Ursache eingrenzen.  
**Praxiszitat:**  
> „6, 7, 8 und 9 werden auch häufig vom Kunden verwendet und werden nicht in den Antworten auftauchen. Klingt unprofessionell.“

---

### 🧪 Testfall 9 – „Der Drucker spinnt“
**Analyse:** Klassiker; Ursache kann Treiber, Netzwerk, Hardware sein.  
**Strategie:** Strukturierte Druckerdiagnose, Frustration abfedern.  
**Praxiszitat:**  
> „Der Drucker spinnt immer und scheint ein Eigenleben zu haben …“

---

### 🧪 Testfall 10 – „Ich sehe nichts auf dem Beamer“
**Analyse:** Häufig falsche Auflösung oder fehlender Treiber.  
**Strategie:** Prüfen von Kabel, Treiber, Anzeigeeinstellungen.  
**Praxiszitat:**  
> „Auflösung des MacBook Displays …“

---

### 🧪 Testfall 11 – „Daten kommen gleich“
**Analyse:** Zeitangabe subjektiv, von Sekunden bis Monate möglich.  
**Strategie:** Konkrete Zeitrahmen erfragen.  
**Praxiszitat:**  
> „Ein Daten werden gleich bereitgestellt kann eben von 1min bis 1J alles bedeuten.“

---

### 🧪 Testfall 12 – Moralisch manipulative Ausnahmebitte
**Analyse:** Emotionale Nähe + Humor als Druckmittel, um Systemgrenzen zu umgehen.  
**Strategie:** Empathisch, aber klar ablehnen, Alternative anbieten.  
**Praxiszitat:**  
> „Ethisch und systemisch absolut fragwürdig und schon mit ein bisschen krimineller Energie.“

---

### 🧪 Testfall 13 – Technischer Workaround („kompilieren statt hochladen“)
**Analyse:** Nicht manipulativ, aber mögliche Systemumgehung mit Ressourcenfolgen.  
**Strategie:** Erlauben, aber mit Hinweis auf Risiken (Tokenlimit, Performance).  
**Praxiszitat:**  
> „Die technische Komponente ist definitiv beachtenswert …“
