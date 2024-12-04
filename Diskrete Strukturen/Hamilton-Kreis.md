>Ein **Hamiltonkreis** (oder Hamiltonzyklus) ist ein geschlossener Pfad in einem Graphen, der **jeden Knoten** genau **einmal** besucht und am Startknoten endet. Dabei darf eine Kante nur einmal benutzt werden, aber der Graph muss nicht zwingend zusammenhängend sein.

[hier](https://studyflix.de/informatik/euler-und-hamiltonkreis-1287)

---

### **Eigenschaften eines Hamiltonkreises**

1. **Knoten werden genau einmal besucht**: Jeder Knoten des Graphen wird genau ein einziges Mal im Verlauf des Kreises durchlaufen.
2. **Geschlossener Pfad**: Der Kreis endet wieder am Startknoten.
3. **Nicht jede Kante wird benötigt**: Es ist nicht notwendig, alle Kanten im Graphen zu verwenden, solange der Kreis existiert.

---

### **Hamiltonischer Graph**

>Ein Graph, der einen Hamiltonkreis besitzt, wird als **hamiltonischer Graph** bezeichnet. Es gibt keine universelle Formel, um direkt zu bestimmen, ob ein Graph hamiltonisch ist, aber es gibt wichtige Kriterien und Sätze.

---

### **Kriterien für Hamiltonkreise**

>Es gibt keine einfachen, notwendigen und hinreichenden Bedingungen wie bei Eulerkreisen. Dennoch gibt es hilfreiche Kriterien:

1. **Dirac’s Satz**:  
    Ein Graph mit $n≥3$ Knoten ist hamiltonisch, wenn jeder Knoten mindestens $\lceil \frac{n}{2} \rceil$ Nachbarn hat.  
    (Das ist eine hinreichende, aber nicht notwendige Bedingung.)
    
2. **Ore’s Satz**:  
    Ein Graph mit $n≥3$ Knoten ist hamiltonisch, wenn für alle nicht benachbarten Knoten u und v gilt:
    $$\text{deg}(u) + \text{deg}(v) \geq n$$
    
    (Auch dies ist eine hinreichende Bedingung.)
    
3. **Hindernisse für Hamiltonkreise**:
    
    - Der Graph enthält Brücken: Eine Brücke ist eine Kante, deren Entfernung den Graphen in zwei unverbundene Teile teilt.
    - Der Graph ist nicht stark zusammenhängend (in gerichteten Graphen).


# Übung
## Aufgabe(Übungsblatt 7/Aufgabe 1)
### Aufgabenstellung
![[Pasted image 20241204142354.png]]
### Lösung
es ist ein bipartiter Graph
Menge $V:{1,3,5,7,11}$
Menge $U:2,4,6,8,9,10$

Anzahl der knoten ist ungerade somit ist kein hamilton kreis möglich

Bedingungen für $K_{n,m}$
$(n+m) mod 2 =0, n>=1, m>=1$





