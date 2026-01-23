# ADR-003: Trennung von Orchestrierung und KI-Systemen

## Status
Accepted

## Kontext
KI-Systeme entwickeln sich schnell und sind austauschbar.
Die Studie soll nicht von einem konkreten Modell abhängen.

## Entscheidung
KI-Funktionalität wird nicht in n8n implementiert,
sondern über externe Dienste angebunden:
- Gemini API für Web-Recherche
- Ollama für lokale Analyse

## Konsequenzen
- Austauschbarkeit von KI-Modellen
- Klare methodische Abgrenzung
- Zusätzlicher Integrationsaufwand
