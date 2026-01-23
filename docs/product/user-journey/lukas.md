# User Journey 2

## *Journalist Lukas – Von einer Frage zur erzählbaren Story*

### 🎯 Ziel des Nutzers

Eine **verständliche, visuelle Geschichte** entwickeln.

---

## Phase 1: Einstieg – Frage statt Objekt

### Nutzeraktion

Lukas stellt direkt eine Frage:

> „Warum haben deutsche Städte so viele französische Partnerstädte?“

---

### Systemreaktion (Frontend)

* Klar strukturierte Antwort:

  * kurze Erklärung
  * visuelle Netzwerkübersicht
* Option:

  > „Vertiefe diese Geschichte“

---

### Interner Prozess

* Interpretation der Frage
* Abgleich:

  * Existieren bereits Analysen?
* Falls nicht:

  * n8n-Workflow:

    * Wikidata
    * Gemini (historischer Kontext)
    * Ollama (Narrativ)

---

## Phase 2: Story-Struktur

### Nutzeraktion

Lukas klickt:

> „Story-Ansicht“

---

### Systemreaktion (Frontend)

* Kapitelstruktur:

  1. Historischer Kontext
  2. Beispiele (z. B. Köln–Paris)
  3. Muster & Zahlen
* Zitate & Quellen

---

### Interner Prozess

* Zusammenführung bestehender Analysen
* Narrative Aufbereitung
* Keine neuen Fakten, nur Reorganisation

---

## Phase 3: Visuelle Anker

### Nutzeraktion

Lukas wählt:

> „Visualisierung für Artikel“

---

### Systemreaktion (Frontend)

* Exportfähige Visualisierung:

  * Netzwerkdiagramm
  * Highlight bestimmter Kanten
* Kurzbeschreibung („Caption“)

---

### Interner Prozess

* Rendering aus Graphdaten
* Metadaten-Anreicherung

---

## Phase 4: Zuspitzung & Validierung

### Nutzeraktion

Lukas fragt:

> „Ist das eher politische Symbolik oder echte Zusammenarbeit?“

---

### Systemreaktion (Frontend)

* Abwägende Antwort:

  * beide Perspektiven
  * Unsicherheiten klar benannt
* Verweise auf Beispiele

---

### Interner Prozess

* Analyse mit Ollama
* Verlinkung zu Einzelfällen

---

## Phase 5: Veröffentlichung

### Nutzeraktion

Lukas:

* exportiert Textbausteine
* übernimmt Grafiken

---

### Systemreaktion

* Zitatfähige Zusammenfassungen
* Quellenliste
* Lizenzhinweise

