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
```

## devcontainer

Das Projekt nutzt einen **Dev Container** für eine einheitliche und reproduzierbare Entwicklungsumgebung. Der Container basiert auf Ubuntu 24.04 und folgt dem Prinzip des lokalen Betriebs (siehe ADR-001).

### Voraussetzungen

- **Docker** (oder kompatible Container-Runtime)
- **VS Code** mit der Erweiterung [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

### Enthaltene Tools

Der Dev Container stellt folgende Werkzeuge bereit:

- **Java/JDK 21** – für Backend-Entwicklung (Kotlin)
- **Node.js 20** – für Frontend-Entwicklung und Tooling
- **Docker CLI + Compose v2** – zur Orchestrierung der lokalen Infrastruktur
- **Git** – Versionsverwaltung

### Installierte VS Code-Erweiterungen

- `bierner.markdown-mermaid` – Mermaid-Diagramme in Markdown
- `eamodio.gitlens` – erweiterte Git-Integration
- `mhutchie.git-graph` – Visualisierung der Git-Historie
- `fwcd.kotlin` – Kotlin-Sprachunterstützung
- `continue.continue` – KI-Assistenz
- `ms-azuretools.vscode-docker` – Docker-Integration

### Sicherheitsmerkmale

Der Container läuft mit eingeschränkten Berechtigungen:
- `--cap-drop=ALL` – Alle Linux-Capabilities werden entfernt
- `--security-opt=no-new-privileges:true` – Verhindert Privilege-Escalation

### Docker-Socket-Zugriff

Der Host-Docker-Socket wird in den Container gemountet (`/var/run/docker.sock`), sodass Docker-Befehle aus dem Container heraus ausgeführt werden können. Dies ermöglicht:

- Starten der lokalen Infrastruktur mit `docker compose`
- Verwaltung von Containern (n8n, Neo4j, etc.)
- Isolierte Entwicklungsumgebung bei gleichzeitiger Integration mit dem Host-Docker-Daemon

### Nutzung

1. **Repository klonen**
2. **In VS Code öffnen**
3. **Auf Aufforderung "Reopen in Container" klicken** (oder über Command Palette: `Dev Containers: Reopen in Container`)
4. **Infrastruktur starten**: 
   ```bash
   cd infra
   docker compose up -d
   ```

Die n8n-Oberfläche ist dann unter http://localhost:5678 erreichbar (User: `admin`, Passwort: `admin`).

