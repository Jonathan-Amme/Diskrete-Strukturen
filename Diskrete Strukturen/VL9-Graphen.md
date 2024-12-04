Graphen sind eine grundlegende mathematische Struktur, die verwendet wird, um Beziehungen zwischen Objekten zu modellieren. Sie bestehen aus: 
- **Knoten (Nodes, Vertices):** Die Objekte, die dargestellt werden.
- **Kanten (Edges):** Die Verbindungen zwischen den Knoten. Graphen finden Anwendung in vielen Bereichen wie Informatik, Physik, Sozialwissenschaften und Verkehrsplanung.

--- 

# Arten von Graphen 
1. **Ungerichteter Graph**: Die Kanten haben keine Richtung. Eine Verbindung zwischen zwei Knoten \(u\) und \(v\) wird durch eine ungeordnete Menge \(\{u, v\}\) dargestellt. 
2. **Gerichteter Graph (Digraph)**: Die Kanten haben eine Richtung, dargestellt durch ein Paar \((u, v)\), wobei \(u\) der Startknoten und \(v\) der Endknoten ist. 
3. **Gewichteter Graph**: Jeder Kante ist ein Wert (z. B. Gewicht, Kosten) zugeordnet. 
4. **Ungewichteter Graph**: Kanten haben keine zusätzlichen Werte.
5. **Planarer Graph**: Ein Graph, der in einer Ebene gezeichnet werden kann, ohne dass sich Kanten schneiden
6. [[Bipartiter Graph]]
7. [Eulerscher Graph](Euler-Kreis)
8. [Hamiltonischer Graph](Hamilton-Kreis)
# Wichtige Begriffe
**Grad eines Knotens**:  
        Die Anzahl der Kanten, die mit einem Knoten verbunden sind. Die Grade eines Graphens lassen sich zu einer [Gradfolge](VL12-Gradfolgen) abbilden. Im gerichteten Graphen unterscheidet man:
            Eingangsgrad: Anzahl der eingehenden Kanten.
            Ausgangsgrad: Anzahl der ausgehenden Kanten.
	    Für jede akkumulierte Gradzahl eines Graphen gilt das [[Handschlaglemma]]
**Pfad**:  
        Eine Abfolge von Knoten, bei der jeder benachbarte Knoten über eine Kante verbunden ist.
        
 **Kreis**:  
        Ein geschlossener Pfad, bei dem der Startknoten gleich dem Endknoten ist.
        
 [Baum](Bäume):  
        Ein spezieller Graph, der zusammenhängend ist und keine Kreise enthält.

# Darstellung von Graphen
### **Knoten- und Kantenlisten**

- **Knotenliste**: Eine Liste aller Knoten des Graphen.
- **Kantenliste**: Eine Liste aller Verbindungen (Kanten) zwischen den Knoten.

**Beispiel:** Für den Graphen G mit Knoten V={A,B,C,D} und Kanten E={(A,B),(B,C),(C,D),(A,D)}:

- Knotenliste: V={A,B,C,D}
- Kantenliste: E={(A,B),(B,C),(C,D),(A,D)}

---

### **Adjazenzmatrix**

Eine **Adjazenzmatrix** ist eine quadratische Matrix, in der Einträge 11 (oder 00) angeben, ob zwei Knoten verbunden sind.

- A[i][j]=1=: Es existiert eine Kante zwischen Knoten i und j.
- A[i][j]=0=0: Keine Kante zwischen i und j.

**Beispiel für ungerichteten Graph:**

![[Pasted image 20241126143037.png]]

---

### **Adjazenzliste**

Eine **Adjazenzliste** ist eine kompakte Darstellung, bei der für jeden Knoten die direkt angrenzenden Nachbarknoten aufgelistet werden.

**Beispiel:**

- A:[B,D]
- B:[A,C]
- C:[B,D]
- D:[A,C]
# Realisierbarkeit

#### 1. **Handschlaglemma**

Die Summe der Grade aller Knoten muss gerade sein:

$i=1∑^n ​d_i$​ ist gerade.

Grund: Jede Kante trägt zu zwei Knotengraden bei.

Wenn diese Bedingung nicht erfüllt ist, ist die Gradfolge nicht realisierbar.

#### 2. **Havel-Hakimi-Kriterium**

Das **Havel-Hakimi-Algorithmus** ist ein iteratives Verfahren, das prüft, ob eine Gradfolge realisierbar ist.

##### Algorithmus:

1. Sortiere die Folge $d=(d_1,d_2,…,d_n)$ in absteigender Reihenfolge.
2. Entferne den größten Wert $d_1$​ aus der Folge.
3. Ziehe 1 von den nächsten $d_1$​ Werten in der Folge ab.
    - Beispiel: Wenn $d_1=3$, reduziere die drei nächsten Werte um 1.
4. Wiederhole den Vorgang mit der neuen Folge.
    - Falls ein Wert negativ wird, ist die Folge nicht realisierbar.
5. Die Gradfolge ist realisierbar, wenn am Ende nur Nullen übrig bleiben.

##### Beispiel:

Gegeben d=(4,3,3,3,3):

1. $d_1=4$, ziehe 1 von den nächsten 4 Werten ab: $d=(3,2,2,2)$.
2. $d_1=3$​, ziehe 1 von den nächsten 3 Werten ab: $d=(2,1,1)$.
2. $d_1=2$, ziehe 1 von den nächsten 2 Werten ab: $d=(1,0)$.
3. $d_1=1$, ziehe 1 von den nächsten 1 Werten ab: $d=(0)$.
4. Die Gradfolge ist realisierbar, da nur Nullen übrig bleiben.
## Übungen
### Aufgabenstellung(Übungsblatt 7/Aufgabe 2)
![[Pasted image 20241204143327.png]]
### Lösung
a) (1,1,2,2,2)->(1,1,1,1)->(1,1)->()
(1,1,1,1,2)->(1,1)->()
(1,1,1,1)->(1,1)->()
(1,2,2,3)->(1,1)->()

b)
$D_1:$Summe der Grade ist 12 von n=6-> kein baum, da nicht 2(n-1)= 10 erfüllt ist
$D_2:$Summe der Grade ist 12 von n=7-> baum, da 2(n-1)= 12 erfüllt ist
$D_3:$Summe der Grade ist 8 von n=5-> baum, da nicht 2(n-1)= 8 erfüllt ist
$D_4:$Summe der Grade ist 16 von n=5-> kein baum, da nicht 2(n-1)= 8 erfüllt ist

c) 
da es nur 2 knoten des grades 4 gibt auf einen Grpahen mit 5 knoten müssen, die 4rer verbunden sein(n-1 größtmöglcihe gradanzahl, verbunden mit allen anderen knoten)
beide knoten verbinden sich mit 2,3,3 nicht unterscheidbar

d)



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
        - Eingangsgrad von C: 2.
        - Ausgangsgrad von A: 2.
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
        - $∣E∣=∣V∣−1$
        - Es gibt genau einen Pfad zwischen zwei beliebigen Knoten.
11. **Isomorphie**
    
    - Zwei Graphen sind isomorph, wenn sie durch Umbenennung ihrer Knoten identisch gemacht werden können.

# Beispiele