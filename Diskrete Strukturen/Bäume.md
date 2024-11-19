>Ein mathematischer Baum ist eine spezielle Art von Graph in der Mathematik. Er wird in der Graphentheorie verwendet und ist durch folgende Eigenschaften definiert:

- Ein Baum ist ein **zusammenhängender Graph ohne Zyklen**.
- Ein Baum mit n Knoten hat immer $n−1$ Kanten.

Mathematische Bäume finden Anwendung in vielen Bereichen, darunter Informatik (z. B. Datenstrukturen), Algorithmik, Netzwerke und sogar Biologie.

---

## Definition

Ein Baum $T$ ist ein Paar $(V,E)$, wobei:

- V die Menge der Knoten (Vertices) ist.
- $E⊆V×V$ die Menge der Kanten (Edges) ist.

Eigenschaften eines Baumes:

1. Es existiert genau **ein eindeutiger Pfad** zwischen zwei beliebigen Knoten.
2. Ein Baum ist ein **minimaler zusammenhängender Graph**:
    - Entfernt man eine Kante, wird der Graph unzusammenhängend.
3. Ein Baum ist ein **maximaler azyklischer Graph**:
    - Fügt man eine Kante hinzu, entsteht ein Zyklus.

---

## Typen von Bäumen
### 1. **Binäre Bäume**
[hier](https://studyflix.de/informatik/binarbaum-1362)
Ein Baum, bei dem jeder Knoten höchstens zwei Kinder (linkes und rechtes Kind) hat.

- **Eigenschaften**:
    
    - Höhe eines binären Baumes: Die Länge des längsten Pfades von der Wurzel zu einem Blatt.
    - Anzahl der Knoten n: $2^{h−1}$ (für einen vollständig balancierten Baum mit Höhe h).
- **Spezielle Formen**:
    
    - **Vollständiger Binärbaum**: Jeder Knoten hat entweder 0 oder 2 Kinder.
    - **Perfekter Binärbaum**: Alle Ebenen sind vollständig gefüllt.
    - **Balancierter Baum**: Die Höhe der linken und rechten Teilbäume unterscheidet sich maximal um 1.
![[Pasted image 20241119142334.png]]

---

### 2. **Suchbäume**
[hier](https://studyflix.de/informatik/binaerer-suchbaum-1364)
Ein spezieller binärer Baum, bei dem die linke Teilmenge kleiner und die rechte größer ist als der aktuelle Knotenwert.

- Beispiele: **Binary Search Tree (BST)**, **AVL-Bäume**, **Rot-Schwarz-Bäume**.

---

### 3. **Spannbäume**

Ein Unterbaum eines Graphen, der alle Knoten verbindet und keinen Zyklus enthält.

- **Minimaler Spannbaum (MST)**: Ein Spannbaum mit minimaler Kantengewichtssumme (z. B. [Kruskal-](Kruskal-Algorithmus) oder [[Prim-Algorithmus]]).
![[Pasted image 20241119142700.png]]

