# ADR-007: Modularer Monorepo-Ansatz

## Status
Accepted

## Kontext
Die Studie umfasst mehrere technische Komponenten mit engem Zusammenhang.

## Entscheidung
Alle Komponenten werden in einem modularen Monorepo verwaltet:
- frontend/
- backend/
- n8n/
- docs/
- infra/

## Konsequenzen
- Einheitliche Versionierung
- Klare Struktur
- Weniger Overhead als Multi-Repo-Setups
