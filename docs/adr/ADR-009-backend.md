# ADR-009: Backend als API- und Abstraktionsschicht

## Status
Accepted

## Kontext
Mehrere Komponenten greifen auf gemeinsame Datenquellen zu.

## Entscheidung
Ein Backend (Kotlin) fungiert als:
- API für Frontend
- Abstraktionsschicht für Graphdatenbank
- Persistenzschicht für Dokumente

## Konsequenzen
- Entkopplung der Systeme
- Klare Verantwortlichkeiten
- Zusätzliche Komponente im System
