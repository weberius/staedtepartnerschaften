# User Journey 1

## *Forscherin Anna – Von einer Stadt zur vergleichenden Analyse*

### 🎯 Ziel der Nutzerin

Vergleichende Erkenntnisse über **Motive und Muster von Städtepartnerschaften** gewinnen.

---

## Phase 1: Einstieg – Fokus auf eine Stadt

### Nutzeraktion

Anna öffnet das System und gibt ein:

> „Köln“

oder wählt Köln aus einer Karte.

---

### Systemreaktion (Frontend)

* Stadtprofil „Köln“ wird angezeigt
* Visualisierung:

  * Köln als zentraler Knoten
  * Partnerstädte als verbundene Knoten
* Metadaten:

  * Anzahl der Partnerschaften
  * Zeiträume
  * geografische Streuung

---

### Interner Prozess (System)

* Abfrage des Wissensgraphen
* Prüfen:

  * Existieren alle Kanten?
  * Existieren Analyse-Dokumente?

---

## Phase 2: Kontextualisierung – Warum diese Partnerschaften?

### Nutzeraktion

Anna klickt auf:

> „Analyse der Partnerschaften“

---

### Systemreaktion (Frontend)

* Liste der Partnerstädte mit:

  * bekannten Motiven (z. B. Versöhnung, Kultur, Wirtschaft)
  * Confidence Score
* Quellenübersicht

---

### Interner Prozess

* Falls Analyse fehlt:

  * Trigger an n8n
  * Recherche (Wikidata / Gemini)
  * Analyse (Ollama)
  * Persistenz im Graph + Dokumentenspeicher

---

## Phase 3: Vergleich – Muster erkennen

### Nutzeraktion

Anna wählt:

> „Vergleiche mit anderen Städten“

Filter:

* Zeitraum: nach 1945
* Region: Europa

---

### Systemreaktion (Frontend)

* Netzwerkansicht erweitert:

  * mehrere Städte
  * Farbcodierung nach Motiv
* Tabellenansicht:

  * Häufigkeit der Motive
  * zeitliche Verteilung

---

### Interner Prozess

* Aggregationsabfrage über Graph
* Zusammenführung mehrerer Analyse-Dokumente
* keine neue Recherche nötig

---

## Phase 4: Hypothesenbildung

### Nutzeraktion

Anna stellt eine Frage:

> „Welche Motive unterscheiden Köln von anderen deutschen Großstädten?“

---

### Systemreaktion (Frontend)

* Strukturierte Antwort:

  * Gemeinsamkeiten
  * Unterschiede
  * Unsicherheiten
* Zitate & Quellen

---

### Interner Prozess

* Query → Wissensgraph
* Textgenerierung mit lokalem Ollama
* Quellenverweise aus Dokumentenspeicher

---

## Phase 5: Ergebnis sichern

### Nutzeraktion

Anna:

* exportiert die Analyse
* speichert eine Ansicht

---

### Systemreaktion

* Export als:

  * Markdown / PDF
* Persistente Referenz auf Datenstand


