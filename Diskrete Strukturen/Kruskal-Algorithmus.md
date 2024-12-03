>Der Kruskal-Algorithmus ist ein Algorithmus zur Bestimmung eines minimalen Spannbaums (MST) eines gewichteten Graphen. Er ist ein Beispiel für einen **gierigen Algorithmus**, da er schrittweise die kleinsten verfügbaren Kanten auswählt, ohne spätere Konsequenzen zu berücksichtigen.

---

## Funktionsweise

1. **Sortiere die Kanten** des Graphen aufsteigend nach ihrem Gewicht.
2. **Initialisiere die Teilmengen** (z. B. mit einer Union-Find-Datenstruktur), wobei jeder Knoten seine eigene Menge bildet.
3. **Iteriere durch die sortierten Kanten**:
    - Füge die Kante zum MST hinzu, wenn sie keine **Zyklen** im Baum erzeugt.
    - Wenn ein Zyklus entsteht, ignoriere die Kante.
4. **Beende**, wenn alle Knoten durch genau ∣V∣−1 Kanten verbunden sind.

---

## Eingabe

- Ein **gewichteter, ungerichteter Graph** G=(V,E), wobei V die Menge der Knoten und E die Menge der Kanten ist.

---

## Ausgabe

- Eine Teilmenge von Kanten $T⊆E$, die den minimalen Spannbaum bildet