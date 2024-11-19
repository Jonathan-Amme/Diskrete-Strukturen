Graphen sind eine grundlegende mathematische Struktur, die verwendet wird, um Beziehungen zwischen Objekten zu modellieren. Sie bestehen aus: - **Knoten (Nodes, Vertices):** Die Objekte, die dargestellt werden. - **Kanten (Edges):** Die Verbindungen zwischen den Knoten. Graphen finden Anwendung in vielen Bereichen wie Informatik, Physik, Sozialwissenschaften und Verkehrsplanung. --- 

# Arten von Graphen 
1. **Ungerichteter Graph**: Die Kanten haben keine Richtung. Eine Verbindung zwischen zwei Knoten \(u\) und \(v\) wird durch eine ungeordnete Menge \(\{u, v\}\) dargestellt. 
2. **Gerichteter Graph (Digraph)**: Die Kanten haben eine Richtung, dargestellt durch ein Paar \((u, v)\), wobei \(u\) der Startknoten und \(v\) der Endknoten ist. 
3. **Gewichteter Graph**: Jeder Kante ist ein Wert (z. B. Gewicht, Kosten) zugeordnet. 
4. **Ungewichteter Graph**: Kanten haben keine zusätzlichen Werte.
5. **Planarer Graph**: Ein Graph, der in einer Ebene gezeichnet werden kann, ohne dass sich Kanten schneiden
6. [Eulerscher Graph](Euler-Kreis)
7. [Hamiltonischer Graph](Hamilton-Kreis)
# Wichtige Begriffe
**Grad eines Knotens**:  
        Die Anzahl der Kanten, die mit einem Knoten verbunden sind. Im gerichteten Graphen unterscheidet man:
            Eingangsgrad: Anzahl der eingehenden Kanten.
            Ausgangsgrad: Anzahl der ausgehenden Kanten.
**Pfad**:  
        Eine Abfolge von Knoten, bei der jeder benachbarte Knoten über eine Kante verbunden ist.
        
 **Kreis**:  
        Ein geschlossener Pfad, bei dem der Startknoten gleich dem Endknoten ist.
        
 [Baum](Bäume):  
        Ein spezieller Graph, der zusammenhängend ist und keine Kreise enthält.

# Darstellung von Graphen
Adjazensmatix, Adjazenzliste....
# Eigenschaften von Graphen

1. **Knotenanzahl ($∣V∣$)**
    
    - Die Anzahl der Knoten im Graphen.
    - Beispiel: Ein Graph mit den Knoten ${A,B,C,D}$ hat $∣V∣=4$.
2. **Kantenanzahl ($∣E∣$)**
    
    - Die Anzahl der Kanten im Graphen. 
    - Beispiel: Ein Graph mit den Kanten ${(A,B),(B,C),(C,A)}$ hat $∣E∣=3$.
3. **Gerichtete und ungerichtete Kanten**
    
    - **Ungerichtete Kanten**: Es gibt keine Richtung; die Verbindung ist symmetrisch. Beispiel: $(A,B)=(B,A)$.
    - **Gerichtete Kanten**: Die Verbindung hat eine Richtung. Beispiel: $(A→B)≠(B→A)$ .
4. **Gewichtete und ungewichtete Kanten**
    
    - **Gewichtete Kanten**: Jede Kante hat ein zugeordnetes Gewicht (z. B. Kosten, Entfernung).
    - **Ungewichtete Kanten**: Alle Kanten sind gleichwertig.
5. **Grad eines Knotens**
    
    - **Grad (ung. Graph)**: Anzahl der Kanten, die mit dem Knoten verbunden sind.
    - **Ein- und Ausgangsgrad (gericht. Graph)**:
        - Eingangsgrad: Anzahl der eingehenden Kanten.
        - Ausgangsgrad: Anzahl der ausgehenden Kanten.
    - Beispiel: Im gerichteten Graphen $A→B,B→C,A→C$:
        - Eingangsgrad von C: 222.
        - Ausgangsgrad von A: 222.
6. **Zusammenhängend und nicht zusammenhängend**
    
    - **Zusammenhängender Graph**: Jeder Knoten ist durch Pfade mit jedem anderen Knoten verbunden.
    - **Nicht zusammenhängender Graph**: Es gibt mindestens zwei Teilmengen von Knoten, zwischen denen keine Verbindung besteht.
7. **Kreise und Zyklen**
    
    - Ein **Kreis** (auch Zyklus genannt) ist ein geschlossener Pfad, bei dem Start- und Endknoten identisch sind.
    - Beispiel: $A→B→C→A$ .
8. **Planarität**
    
    - Ein Graph ist [planar](Planarität von Graphen), wenn er in einer Ebene gezeichnet werden kann, ohne dass sich Kanten schneiden. Die Planarität eines Graphen kann unteranderem durch [[Kuratowski’s Theorem]] nachgewiesen werden.
9. **Bipartitheit**
    
    - Ein Graph ist [bipartit](Bipartitheit von Graphen), wenn die Knoten in zwei Mengen U und W aufgeteilt werden können, sodass alle Kanten nur zwischen Knoten aus U und W verlaufen, aber nicht innerhalb einer Menge.
    
10. **Baumeigenschaften**
    
    - Ein Baum ist ein spezieller Graph, der zusammenhängend ist und keine Kreise enthält.
    - Eigenschaften:
        - ∣E∣=∣V∣−1|E| = |V| - 1∣E∣=∣V∣−1.
        - Es gibt genau einen Pfad zwischen zwei beliebigen Knoten.
11. **Isomorphie**
    
    - Zwei Graphen sind isomorph, wenn sie durch Umbenennung ihrer Knoten identisch gemacht werden können.

# Beispiele