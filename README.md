# KI-gestützte Orchestrierung von Wissensgraphen  
## Eine explorative Studie am Beispiel von Städtepartnerschaften

## Überblick

Dieses Repository enthält den Code, die Workflows und die begleitende Dokumentation einer Studie, die untersucht, **wie n8n, generative KI (Gemini, lokale LLMs) und Graphdatenbanken** zur orchestrierten Wissensgenerierung eingesetzt werden können.

Im Mittelpunkt steht **nicht ein produktives System**, sondern ein **Forschungs- und Studienartefakt**, das Transparenz, Nachvollziehbarkeit und Reproduzierbarkeit von KI-gestützten Analyseprozessen ermöglicht.

## Ziel der Studie

Die Studie verfolgt folgende Ziele:

- Untersuchung von **Low-Code-Orchestrierung** (n8n) für agentenähnliche KI-Prozesse
- Analyse der Rolle von **Graphdatenbanken** als Wissensstruktur
- Bewertung von **generativer KI** als Recherche- und Analysewerkzeug
- Erprobung eines **reproduzierbaren Forschungs-Setups**

## Zentrale Fragestellungen

- Wie lassen sich KI-gestützte Recherche- und Analyseprozesse transparent orchestrieren?
- Welche Vorteile bietet ein Wissensgraph gegenüber klassischen Dokumentensammlungen?
- Wo liegen die Grenzen von Low-Code-Orchestrierung für komplexe Wissenssysteme?
- Wie lässt sich Unsicherheit und Interpretation explizit modellieren?

## Repository-Struktur

```text
.
├─ frontend/          # Angular-Frontend (Exploration & Visualisierung)
├─ backend/           # Kotlin-Backend (API & Query-Layer)
├─ n8n/               # n8n-Workflows zur Orchestrierung
├─ graph/             # Graphschema & Beispielabfragen
├─ documents/         # KI-generierte Analysen (Markdown)
├─ ai/                # Prompts & Output-Schemata
├─ infra/             # Lokales Setup (Docker, Compose)
├─ docs/              # Vision, Methodik, Limitationen
└─ README.md