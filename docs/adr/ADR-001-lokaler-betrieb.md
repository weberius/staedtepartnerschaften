# ADR-001: Lokaler Betrieb aller Kernkomponenten

## Status
Accepted

## Kontext
Die Studie legt Wert auf Reproduzierbarkeit, Kontrolle über Datenflüsse
und minimale externe Abhängigkeiten.

## Entscheidung
Alle Kernkomponenten werden lokal betrieben:
- n8n
- Graphdatenbank
- Backend (Kotlin)
- lokale LLMs (Ollama)

Externe APIs (z. B. Gemini) werden nur gezielt für Recherche eingesetzt.

## Konsequenzen
- Hohe Kontrolle über Daten und Prozesse
- Erhöhte Komplexität im lokalen Setup
- Gute Eignung für explorative Forschung
