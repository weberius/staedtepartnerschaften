# Methodology

## 1. Ziel der Studie

Diese Studie untersucht, wie Low-Code-Orchestrierung (n8n) in
Kombination mit generativer KI (Gemini, Ollama) zur iterativen
Erstellung und Erweiterung eines Wissensgraphen genutzt werden kann.

## 2. Methodische Annahmen

- Städtepartnerschaften werden als relationale Wissensobjekte verstanden.
- Informationen aus dem Internet sind fragmentiert und kontextabhängig.
- KI-generierte Analysen sind interpretativ, nicht faktisch.

## 3. Datenquellen

Die Studie nutzt folgende Quellen:
- strukturierte Wissensdatenbanken (z. B. Wikidata)
- unstrukturierte Webquellen (über Gemini)
- lokal generierte Analyse-Texte (Ollama)

## 4. Orchestrierung der Wissensgenerierung

Die Orchestrierung erfolgt über n8n-Workflows, die folgende Aufgaben übernehmen:
1. Trigger-basierte Recherche
2. Sequenzierung von KI-Aufrufen
3. Persistenz von Ergebnissen

## 5. Rolle der KI

Gemini:
- Recherche & Zusammenfassung externer Informationen

Ollama:
- Interpretation, Vergleich und Kontextualisierung

## 6. Wissensmodell

Wissen wird in Form eines Graphen modelliert:
- Knoten: Städte
- Kanten: Städtepartnerschaften
- Attribute: Zeitraum, Motive, Quellen

## 7. Analyseprozess

Analysen erfolgen:
- auf Basis persistierter Fakten
- durch KI-gestützte Synthese
- mit expliziter Trennung von Fakt und Interpretation

## 8. Reproduzierbarkeit

Alle Analysen sind reproduzierbar durch:
- versionierte Prompts
- gespeicherte Quellen
- versionierte Workflows

## 9. Limitationen

- unvollständige Quellen
- kulturelle Verzerrungen
- KI-Halluzinationen

## 10. Reflexion

Die Studie erhebt keinen Anspruch auf historische Vollständigkeit,
sondern auf explorative Erkenntnisgewinnung.

