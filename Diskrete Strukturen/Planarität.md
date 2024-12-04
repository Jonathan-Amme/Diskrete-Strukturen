
>Die **Planarität** eines Graphen ist ein Konzept der Graphentheorie, das beschreibt, ob ein Graph in der Ebene gezeichnet werden kann, ohne dass sich seine Kanten überschneiden (außer an den Knotenpunkten).

---

### **Definition**

Ein **Graph ist planar**, wenn er so in die Ebene eingebettet werden kann, dass keine zwei Kanten sich schneiden (außer an gemeinsamen Knoten). Eine solche Zeichnung nennt man eine **planare Einbettung**.

---

### **Beispiele**

1. **Planarer Graph**:
    
    - Ein einfacher Dreieck-Graph mit Knoten A,B,C und Kanten (A,B),(B,C),(C,A) ist planar, da er ohne Überschneidungen gezeichnet werden kann.
2. **Nicht-planarer Graph**:
    
    - Der vollständige Graph $K_5$​ (5 Knoten, wobei jeder Knoten mit jedem anderen verbunden ist) ist **nicht planar**. Es ist unmöglich, ihn ohne Überschneidungen in die Ebene einzubetten.

---

### **Kriterien für Planarität**

Es gibt mehrere Methoden, um die Planarität eines Graphen zu bestimmen:

#### 1. **Eulersche Formel** (für zusammenhängende planare Graphen)

Die **Eulersche Polyederformel** lautet:

$∣V∣−∣E∣+∣F∣=2$

wobei:

- ∣V∣: Anzahl der Knoten,
- ∣E∣: Anzahl der Kanten,
- ∣F∣: Anzahl der Flächen (inklusive der unendlichen Außenfläche).

Für einen planaren Graphen gilt immer diese Beziehung. Wenn sie verletzt wird, ist der Graph nicht planar.

#### 2. [[Kuratowski’s Theorem]]

### **Planare Graphen und ihre Eigenschaften**

1. **Maximale Anzahl der Kanten in einem planaren Graphen**:
    
    - Für einen planaren Graphen mit n Knoten gilt:$∣E∣≤3∣V∣−6,wenn->n≥3.$
    - Für einen planaren Graphen ohne Mehrfachkanten oder Schleifen (also ohne Parallel- oder Eigenkanten).
2. **Dualer Graph**:
    
    - Jeder planare Graph hat einen **dualen Graphen**, in dem jede Fläche des ursprünglichen Graphen einem Knoten im dualen Graphen entspricht.
3. **Färbungsproblem**:
    
    - Planare Graphen können immer mit **höchstens 4 Farben** so gefärbt werden, dass keine zwei benachbarten Knoten dieselbe Farbe haben (siehe [[Vier-Farben-Satz]]).

# Übungen
## Übung(Übungsblatt 7/ Aufgabe 3)
### Aufgabenstellung

### Lösung
$∣V∣=∑_{i=1}^k​∣V_i​∣$ 
$∣E∣=∑_{i=1}^k​∣E_i∣​$

$∣F∣=∑_{i=1}^k∣F_i∣−k+1$
(k-1, da bei jeder Zusammenhangskomponente die Umgebung mit gezählt wird aber alle Komponenten sich die Umgebung teilen)

-> Einsetzen in die eulersche Formel für alle Komponenten
$∑_{i=1}^k​(∣V_i​∣−∣E_i​∣+∣F_i​∣)=2k$
$∣V∣−∣E∣+(∣F∣+(k−1))=2k$
-> $∣V∣−∣E∣+∣F∣=k+1$

## Übung(Übungsblatt/Aufgabe 4)
### Aufgabenstellung
![[Pasted image 20241204150850.png]]
### Lösung
$4∣V∣=∑_{i=1}^n​∣deg(n)​∣$

$2∣E∣=∑_{i=1}^n​∣deg(n)​∣$

$∣F∣<=(2∣E∣+1)/5$

$∣V∣ = 1/2 ∣E∣$
$1/2∣E∣−∣E∣+∣F∣=2$

$∣F∣=2+ 1/2∣E∣$

in die dritte einsetzen

(2+1/2|E|)<=2∣E∣/5+1/5 ->Widerspruch Links ist größer