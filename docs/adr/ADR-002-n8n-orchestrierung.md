# ADR-002: Einsatz von n8n als Orchestrierungsschicht

## Status
Accepted

## Kontext
Komplexe KI-gestützte Prozesse sollen transparent, reproduzierbar und
nachvollziehbar orchestriert werden.

## Entscheidung
n8n wird als zentrale Orchestrierungsschicht eingesetzt.
n8n übernimmt ausschließlich:
- Steuerung von Abläufen
- Sequenzierung von KI-Aufrufen
- Übergabe und Persistenz von Daten

n8n übernimmt keine KI-Funktionalität selbst.

## Konsequenzen
- Klare Trennung von Logik und Intelligenz
- Gute Visualisierbarkeit von Prozessen
- Begrenzte Ausdrucksmächtigkeit komplexer Logiken
