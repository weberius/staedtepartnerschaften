# ADR-004: Verwendung eines Wissensgraphen als primäres Datenmodell

## Status
Accepted

## Kontext
Städtepartnerschaften sind hochgradig vernetzt, mehrdeutig und kontextabhängig.

## Entscheidung
Eine Graphdatenbank wird als primäres Datenmodell verwendet.
- Städte → Knoten
- Partnerschaften → Kanten
- Motive, Quellen, Analysen → Properties oder Zusatzknoten

## Konsequenzen
- Natürliche Abbildung komplexer Beziehungen
- Erhöhte Modellierungskomplexität
- Gute Basis für visuelle Exploration
