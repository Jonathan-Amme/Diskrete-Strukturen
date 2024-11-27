
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

- Beispiele: **Binary Search Tree (BST)**, **AVL-Bäume**, **Rot-Schwarz-Bäume**.

---

### 3. **Spannbäume**

Ein Unterbaum eines Graphen, der alle Knoten verbindet und keinen Zyklus enthält.

- **Minimaler Spannbaum (MST)**: Ein Spannbaum mit minimaler Kantengewichtssumme (z. B. [Kruskal-](Kruskal-Algorithmus) oder [[Prim-Algorithmus]]).
![[Pasted image 20241119142700.png]]

# Übungen
## Übungsblatt 6(Übung 1)

### Aufgabenstellung
![[Pasted image 20241127141535.png]]
### Lösung
a) (4,4,3,2,2,1,1,1,1,1,1,1)
b) 
c) I) Für jeden Baum gilt E=n-1 und $∑​deg(v)=2∣E∣$ , ergo gilt $∑_i^n ​d_i​=2n−2$
 II)jeder baum hat mindestens zwei Knoten mit Grad 1, das ergibt sich aus der Tatsache, dass Bäume keine Zyklen haben und keine Knoten mit Grad 0 zulassen (jeder Knoten ist verbunden und $n≥2$
 d)
 Basis: n=2 (1,1) -> $1+1 =2*2-2=2$
 Annahme: angenommen es kann jede aufsteigende Gradsequenz mit I) und II) realisiert werden
 Schritt:
 Für $(d_1,d_2,.....d_n, d_{n+1})$ gilt: $∑_i^{n+1} ​d_{i}​=2n$
	 -> Entferne ein Blatt $(d_1,d_2,.....d_n, d_{n+1})$ -> $(d_2,.....d_n, d_{n+1})$ 
 Es gilt: $∑_{i=2}^{n+1}​ d_i​−1=2n−2$

## Übungsblatt 6(Übung 2)
### Aufgabenstellung
![[Pasted image 20241127144040.png]]
### Lösung
a) Algorithmus arbeitet wie folgt: 
1. Beginne bei einem Startknoten $v_1$.
2. Suche in der Nachbarschaft des aktuellen Knotens nach einem unbesuchten Knoten und füge diesen hinzu.
3. Wenn kein unbesuchter Nachbar vorhanden ist, gehe im Baum zurück, bis du einen Knoten mit unbesuchten Nachbarn findest.
4. Wiederhole diesen Prozess, bis alle Knoten im Baum sind.
 
 Der Algorithmus kreiert nicht garantiert, dass jeder [[Spannbaum]] ein [[Pfadgraph]] ist, da auf bereits besuchte knoten immer zurückgepsrungen wird, wenn man in der tiefe keinen besuchten knoten mehr findet.

b) Kanten: 8
- **Knoten 1:** Nachbarn {3,5}.
- **Knoten 2:** Nachbarn {4,5,6}.
- **Knoten 3:** Nachbarn {1,5,6}.
- **Knoten 4:** Nachbarn {2,6}.
- **Knoten 5:** Nachbarn {1,2,3}.
- **Knoten 6:** Nachbarn {2,3,4}.

- schließt Verzweigungen oder Zyklen aus, wodurch eine lineare Abfolge entsteht, die der Struktur eines Pfadgraphen entspricht.
- Egal, welche Reihenfolge der Nachbarn gewählt wird, der resultierende Spannbaum hat dieselbe lineare Struktur (d. h., er bleibt isomorph zu $P_6$).

Isomorphie:![[Pasted image 20241127150451.png]]
c)
G ist zusammenhängend.
Nehmen wir an, dass jeder Knoten w ein Trennknoten ist
    - Das bedeutet, dass bei Entfernung eines beliebigen Knotens G in zwei oder mehr Zusammenhangskomponenten zerfällt.
    - Dies ist ein Widerspruch zur Eigenschaft von Zyklen oder zur Existenz von Blättern in einem Spannbaum.
Schlussfolgerung:
    - Es existiert mindestens ein Knoten w, der kein Trennknoten


## Übungsblatt 6(Aufgabe 3)
### Aufgabenstellung
![[Pasted image 20241127150827.png]]
### Lösung
Es müssen mindestens zwei Zusammenhangskomponenten existieren
als m = k über 2+ n-k über 2

Das garantiert die größtmögliche Anzahl an Kanten in einem nicht zusammenhängenden Graphen, da die maximale Gradanzahl für einen zusammenhängenden Graphen m=(2n​) beträgt