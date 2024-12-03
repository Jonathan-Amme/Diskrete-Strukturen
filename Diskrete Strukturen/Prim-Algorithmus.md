>Der **Prim-Algorithmus** ist ein Algorithmus zur Bestimmung eines **minimalen Spannbaums (MST)** eines gewichteten Graphen. Im Gegensatz zum **Kruskal-Algorithmus**, der mit Kanten arbeitet, wächst der Prim-Algorithmus ausgehend von einem Startknoten durch das schrittweise Hinzufügen der billigsten Kanten.

---

## Funktionsweise

1. **Wähle einen Startknoten** aus dem Graphen.
2. **Füge Kanten schrittweise hinzu**, wobei immer die billigste Kante gewählt wird, die einen neuen Knoten mit dem bereits gebildeten Baum verbindet.
3. Wiederhole den Vorgang, bis alle Knoten im Baum enthalten sind.

---

## Eingabe

- Ein **gewichteter, ungerichteter Graph** G=(V,E), wobei V die Menge der Knoten und E die Menge der Kanten ist.

---

## Ausgabe

- Eine Teilmenge von Kanten $T⊆E$, die den minimalen Spannbaum bildet.