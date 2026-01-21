# Limitationen der Studie

Dieses Kapitel beschreibt die methodischen, technischen und inhaltlichen Grenzen der Studie.  
Die Limitationen sind **keine Schwächen im engeren Sinne**, sondern ergeben sich bewusst aus dem explorativen und prototypischen Charakter des Systems.

---

## 1. Inhaltliche Limitationen

### 1.1 Unvollständigkeit der Daten
Städtepartnerschaften sind weltweit nicht einheitlich dokumentiert.  
Viele Informationen liegen nur fragmentiert, lokal oder in unterschiedlichen Sprachen vor.

- Nicht alle Partnerschaften sind öffentlich erfasst
- Historische Motive sind teilweise nicht mehr rekonstruierbar
- Offizielle Darstellungen können politische Narrative widerspiegeln

Der Wissensgraph bildet **keinen vollständigen oder abschließenden Überblick**, sondern eine explorative Auswahl.

---

### 1.2 Kontextabhängigkeit von Motiven
Die Motivation für Städtepartnerschaften ist häufig:
- mehrdeutig
- zeitlich wandelbar
- kulturell geprägt

KI-gestützte Analysen können diese Komplexität **nur approximieren**, nicht vollständig abbilden.

---

## 2. Methodische Limitationen

### 2.1 Interpretativer Charakter der KI
Die eingesetzten KI-Systeme:
- erzeugen keine „objektive Wahrheit“
- sondern interpretative Zusammenfassungen auf Basis verfügbarer Texte

Auch bei sorgfältiger Prompt-Gestaltung können:
- Verzerrungen
- Vereinfachungen
- Fehlinterpretationen

auftreten.

---

### 2.2 Abhängigkeit von Prompts und Workflows
Die Ergebnisse sind stark abhängig von:
- Formulierung der Prompts
- Reihenfolge der Workflow-Schritte
- Auswahl der Datenquellen

Kleine Änderungen in der Orchestrierung können zu **qualitativ anderen Ergebnissen** führen.

---

### 2.3 Fehlende Ground-Truth-Validierung
Die Studie verzichtet bewusst auf eine systematische externe Validierung aller Ergebnisse durch Expert:innen.

Aussagen dienen der Exploration, nicht der Verifikation.

---

## 3. Technische Limitationen

### 3.1 Prototypischer Charakter
Das System ist:
- lokal betrieben
- nicht auf Skalierung ausgelegt
- nicht für produktiven Dauerbetrieb optimiert

Aspekte wie:
- Performance
- Ausfallsicherheit
- parallele Nutzung

werden nicht untersucht.

---

### 3.2 Beschränkungen von Low-Code-Orchestrierung
n8n bietet Transparenz und Flexibilität, bringt jedoch auch Grenzen mit sich:

- eingeschränkte Kontrollflüsse
- begrenzte Debugging-Möglichkeiten
- Workflow-Komplexität steigt schnell

Diese Aspekte können die Wartbarkeit bei wachsender Komplexität einschränken.

---

## 4. Limitationen der Graphmodellierung

### 4.1 Vereinfachung komplexer Beziehungen
Die Modellierung als Graph erfordert:
- Reduktion komplexer historischer Prozesse
- Abbildung vielschichtiger Motive auf diskrete Attribute

Dadurch können:
- Ambivalenzen
- Widersprüche
- Mehrdeutigkeiten

nur eingeschränkt dargestellt werden.

---

### 4.2 Zeitliche Dynamik
Veränderungen über die Zeit (z. B. Wandel von Motiven) werden nur begrenzt berücksichtigt.

Der Graph stellt überwiegend **statische Momentaufnahmen** dar.

---

## 5. Sprachliche und kulturelle Limitationen

### 5.1 Sprachabhängigkeit der Quellen
Die Qualität der Analyse hängt stark von:
- verfügbaren Sprachen
- Übersetzungsqualität
- kulturellen Kontexten

ab.

Bestimmte Regionen sind dadurch systematisch unterrepräsentiert.

---

### 5.2 Westlich geprägte Perspektiven
Viele verfügbare Quellen stammen aus westlichen Informationskontexten, was zu:
- eurozentrischen Interpretationen
- kulturellen Verzerrungen

führen kann.

---

## 6. Ethische Limitationen

### 6.1 Autorität und Interpretation
KI-generierte Texte können den Eindruck von Autorität erzeugen, obwohl sie interpretativ sind.

Das System adressiert dies durch:
- explizite Kennzeichnung von Unsicherheit
- Quellenverweise
- Trennung von Fakt und Interpretation

Eine vollständige Eliminierung dieses Effekts ist jedoch nicht möglich.

---

## 7. Zusammenfassung

Die Studie versteht sich als **methodische Exploration**, nicht als abschließende Analyse von Städtepartnerschaften.

Die beschriebenen Limitationen sind integraler Bestandteil des Forschungsdesigns und dienen der:
- Einordnung der Ergebnisse
- Transparenz gegenüber Nutzer:innen
- wissenschaftlichen Nachvollziehbarkeit

