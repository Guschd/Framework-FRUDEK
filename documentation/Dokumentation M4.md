# 📦 FRUDEK Modul M4 – Kontextgewichtung & Relevanzfilter

## 🧠 Modulbeschreibung
M4 ist dafür verantwortlich, eingehende Anfragen nach **Bedeutung und Relevanz** zu filtern.  
Es erkennt, welche Teile einer Eingabe **wesentlich** für die Beantwortung sind und welche **irrelevanten oder ablenkenden Elemente** als „Rauschen“ zu behandeln sind.  
Das Modul entscheidet, ob Nebenaspekte **vollständig ignoriert**, **gekürzt** oder **bewusst einbezogen** werden, um eine vollständige und präzise Antwort zu liefern.

---

### 🎯 Ziele
- Erkennen der **Kerninformation** in einer Anfrage  
- Identifikation von **irrelevantem Kontext** oder thematischen Abschweifungen  
- Gewichtung einzelner Informationsteile nach **Bedeutung für die Problemstellung**  
- Sicherstellen, dass wichtige Randbedingungen **nicht versehentlich entfernt** werden  
- Reduzierung von **Verarbeitungszeit** durch Fokussierung auf relevante Daten

---

### 🔍 Herausforderungen
- Nutzer formulieren oft **mehrere Themen** in einem Prompt  
- Relevanz ist oft **kontextabhängig** und erfordert Vorwissen  
- **Emotionale Zusätze** können vom Kernproblem ablenken, sind aber für Tonfallwahl relevant  
- Gefahr, zu viel zu filtern und dadurch **wichtige Details zu verlieren**  
- Abgrenzung zwischen „irrelevant“ und „sekundär relevant“ ist oft fließend

---

## 🧪 Testfälle

### 🧪 Testfall 1 – Mehrere Themen in einer Anfrage
**Eingabe:** „Mein Drucker spinnt, und übrigens hat sich mein PC gestern komisch verhalten.“  
**Analyse:** Druckerproblem ist das Hauptthema, PC-Verhalten sekundär.  
**Strategie:** Hauptproblem zuerst lösen, Nebenthema in separater Rückfrage behandeln.  

---

### 🧪 Testfall 2 – Emotionale Rahmung
**Eingabe:** „Seit dem letzten Update ist wieder alles kaputt, ich bin echt genervt.“  
**Analyse:** Emotion wichtig für Tonfall, Kernproblem ist „letztes Update“ → technische Analyse.  
**Strategie:** Emotion wahrnehmen, Kernproblem technisch angehen.  

---

### 🧪 Testfall 3 – Fachlicher Kern in Smalltalk eingebettet
**Eingabe:** „Hoffentlich hattest du ein schönes Wochenende… mein Export geht nicht mehr.“  
**Analyse:** Smalltalkteil ist nicht problemrelevant, Exportproblem ist Kern.  
**Strategie:** Höflich auf Smalltalk reagieren, dann Problem lösen.  

---

### 🧪 Testfall 4 – Impliziter Nebenaspekt mit hoher Relevanz
**Eingabe:** „Mein WLAN ist langsam, und mein Drucker druckt nur über Kabel.“  
**Analyse:** WLAN-Probleme könnten Ursache für Druckerproblem sein.  
**Strategie:** Nebenaspekt berücksichtigen, da technisch verbunden.  

---

## 📂 Praxisbeispiele

### 📂 Beispiel 1 – Mailprogramm mit Nebenthema
**Eingabe aus Ticket:** „Bei Herrn $Anwender funktioniert das Mailprogramm nicht (PC wurde schon mehrfach neu gestartet)! … Laufwerk manuell verknüpft. gpupdate und gpupdate /force hat keine Auswirkung. … Ach ja, die Netzlaufwerke spinnen auch manchmal.“  
**Analyse:**  
- Hauptproblem: Mailprogramm funktioniert nicht.  
- Nebenaspekt: Netzlaufwerksprobleme → technisch relevant, da Mailprofile dort liegen.  
**Strategie:**  
- Beide Themen bearbeiten, da sie technisch zusammenhängen.  
**Kommentar Sebastian:**  
> „Hier ist der Nebenaspekt indirekt der Schlüssel zur Lösung. Filterung hätte den Kern übersehen.“

---

### 📂 Beispiel 2 – Terminalserver-Login mit persönlichem Zusatz
**Eingabe aus Ticket:** „Warten auf Benutzerprofildienst… dauert Stunden. Nebenbei: brauche neue Tastatur.“  
**Analyse:**  
- Hauptproblem: Anmeldeblockade am Terminalserver.  
- Nebenaspekt: Hardwarebedarf → organisatorisch, nicht technisch mit dem Hauptproblem verknüpft.  
**Strategie:**  
- Kernproblem sofort bearbeiten, Nebenaspekt an Beschaffungsstelle weitergeben.

---

### 📂 Beispiel 3 – 3D-Druckprojekt mit Zusatzwunsch
**Eingabe:** „Kannst du mir das Drachenboot anpassen, und wenn du Zeit hast, vielleicht noch ein Logo reinmachen?“  
**Analyse:**  
- Hauptauftrag: Anpassung für Display und Micro-USB-Ports.  
- Nebenaspekt: Logo → optische Zusatzfunktion.  
**Strategie:**  
- Hauptauftrag priorisieren, Zusatzwunsch als optional markieren.  
**Kommentar Sebastian:**  
> „Das ist ein klassischer Fall von 'Hauptjob jetzt, Extras später', sonst läuft man Gefahr, sich zu verzetteln.“

---

### 📂 Beispiel 4 – Schulungstermine mit Randbemerkung
**Eingabe aus Ticket:** „Wir haben ein Schulungskontingent… intern noch Klärungsbedarf… Ach ja, die Dokumentation für die Fachkonferenz ist noch nicht fertig.“  
**Analyse:**  
- Hauptthema: Klärung von Schulungsterminen.  
- Nebenaspekt: Fertigstellung der Konferenzdokumentation → organisatorisch wichtig, aber nicht Bestandteil des Hauptauftrags.  
**Strategie:**  
- Hauptthema weiterverfolgen, Nebenaspekt gesondert dokumentieren.

---

## 🛠 Hinweise für AI-Trainer
- Immer **Haupt- vs. Nebenaspekte** klar trennen  
- Nebenaspekte **nicht ignorieren**, sondern in separater Liste/Rückfrage erfassen  
- **Kontextabhängigkeit** prüfen: manchmal ist ein Nebenaspekt Schlüssel zum Hauptproblem  
- Emotionen nicht filtern, sondern zur **Tonalitätsanpassung** an M3 weitergeben  
- Bei stark gemischten Themen separate Bearbeitungs-Threads anlegen
