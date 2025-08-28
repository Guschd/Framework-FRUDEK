# M12 – Response Framing & Situative Gewichtung

## 🧭 Zielsetzung

Modul M12 beschreibt die Fähigkeit, **Antworten abhängig vom Gesprächskontext, situativer Dringlichkeit und emotionalem Zustand** des Fragenden zu gestalten.

Ziel ist es, den generierten Output **nicht nur semantisch korrekt**, sondern auch **menschlich angemessen, empathisch und proaktiv** zu gestalten – ohne in allgemeine Floskeln abzurutschen.

---

## 🎯 Kerngedanke

Nicht jede Antwort ist in jeder Situation richtig – auch wenn sie formal korrekt ist.

Framing bedeutet, dass Antworten auf Grundlage von:
- Dringlichkeit (z. B. Totalausfall vs. Komfortproblem),
- Fragestil (z. B. ironisch, wütend, ratlos, präzise)
- Beziehungsstatus (z. B. lange Supporthistorie vs. Erstkontakt)
- Abhängigkeiten (z. B. Quartalsreport steht an)

… **unterschiedlich gewichtet und formuliert** werden müssen.

---

## 🔍 Beispielhafte Framing-Stile

| Stiltyp | Beschreibung | Beispielantwort |
|--------|--------------|-----------------|
| 🤝 Freundlich-kooperativ | Bei Hilfsbereitschaft und Sachlichkeit | „Das schauen wir uns gleich gemeinsam an.“ |
| 💡 Lösungsorientiert | Bei klaren technischen Fragen | „Bitte geben Sie mir den Hostnamen, dann sehe ich nach.“ |
| 🔄 Relational-humorvoll | Bei lockerer Beziehung oder Kolleg:innen | „Ich hab’s extra kaputt gemacht, damit du eher heim darfst 😅“ |
| 🧘 Beruhigend-deeskalierend | Bei Stress, Frust, Eskalation | „Wir bekommen das gemeinsam hin. Ich begleite dich Schritt für Schritt.“ |
| 📍 Direkt-pragmatisch | Bei sehr erfahrener Person | „Terminal öffnen und Befehl `xyz` eingeben – das sollte es lösen.“ |
| 🧠 Meta-reflektierend | Bei KI-Misstrauen oder ethischer Unsicherheit | „Ich bin eine KI und arbeite auf Basis deiner Eingaben. Du bestimmst das Ziel.“ |

---

## 🧪 Strukturierte Testfälle

---

### ✅ Testfall A

**Input:**  
„Mach es einfach – du weißt doch wie’s geht!“

**Framing-Erkennung:**  
→ Informell, locker, evtl. kollegialer Kontext

**Empfohlener Stil:**  
🔄 Relational-humorvoll / 📍 Direkt-pragmatisch

**Antwortbeispiel:**  
„Wenn ich dein Netzwerk-Setup noch richtig im Kopf habe, starten wir am besten mit der letzten Änderung. Bereit?“

---

### ✅ Testfall B

**Input:**  
„Ich weiß echt nicht mehr weiter. Wenn das nicht bald läuft, bin ich geliefert.“

**Framing-Erkennung:**  
→ Emotionaler Druck, evtl. externe Deadline

**Empfohlener Stil:**  
🧘 Beruhigend-deeskalierend / 💡 Lösungsorientiert

**Antwortbeispiel:**  
„Okay, kein Grund zur Sorge – wir lösen das Schritt für Schritt. Was war das letzte, das noch funktioniert hat?“

---

### ✅ Testfall C

**Input:**  
„Ich hab den Button vermisst… 😩“

**Framing-Erkennung:**  
→ Zwischen Frust und Humor, meist bei UI-Änderung

**Empfohlener Stil:**  
🧘 + 💡 (je nach Verlauf)

**Antwortbeispiel:**  
„Der Button hat sich in Rente verabschiedet – aber wir finden den neuen Workflow. Ich zeig’s dir.“

---

### ✅ Testfall D

**Input:**  
„Ich will das nicht schon wieder erklären.“

**Framing-Erkennung:**  
→ Ermüdung, evtl. Wiederholungsfall

**Empfohlener Stil:**  
🧘 + 🤝

**Antwortbeispiel:**  
„Ich versteh dich. Ich schau mal, was in der Historie hinterlegt ist – wir fangen nicht bei null an.“

---

## 🧩 Modulbezug

- **Verknüpft mit:**  
  - **M1 – Inputklassifikation**  
  - **M2 – Kontextauflösung**  
  - **M6 – Semantische Feinjustierung**  
  - **M11 – Technisch-emotionale Eskalationen**  

- **Optional kombinierbar mit:**  
  - Sentiment-Parser / Emotion-Klassifikator  
  - Nutzerhistorie / Historienlogik (z. B. „letzter Fall“)  

---

## 🔗 Besonderheit

Dieses Modul **verschmilzt Soft-Skill-Kompetenz mit technischer Analyse** und ermöglicht so eine empathische und situative Reaktion – sowohl durch Menschen als auch durch KI-Systeme.

Das Ziel ist nicht „richtige“ Antworten zu geben, sondern **passende**, **tragfähige** und **entlastende** Antworten.

---

## 🛠️ YAML-Metadaten

```yaml
---
modul: M12
title: Response Framing & Situative Gewichtung
author: Sebastian Besold / GPT-4o
license: CC BY 4.0
version: 1.0
linked_modules: [M1, M2, M6, M11]
last_updated: 2025-08-07
---
