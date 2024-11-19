>Ein **eulerscher Graph** ist ein Graph, der einen **Eulerkreis** besitzt. Ein Eulerkreis ist ein geschlossener Weg im Graphen, der jede Kante genau **einmal** benutzt und am Ausgangspunkt endet. [hier](https://studyflix.de/informatik/euler-und-hamiltonkreis-1287/video)

---

### **Eigenschaften eines eulerschen Graphen**

Ein Graph ist **eulerscher Graph**, wenn folgende Bedingungen erfüllt sind:

1. **Ungerichteter Graph**:
    
    - Jeder Knoten hat einen **geraden Grad** (die Anzahl der Kanten, die an einem Knoten anliegen, ist gerade).
    - Der Graph ist zusammenhängend (es gibt eine Verbindung zwischen allen Knoten, wenn man Kanten ignoriert).
2. **Gerichteter Graph**:
    
    - Jeder Knoten hat den gleichen **Ein- und Ausgangsgrad**.
    - Der Graph ist stark zusammenhängend (es gibt einen gerichteten Weg von jedem Knoten zu jedem anderen).

---

### **Eulerpfad (statt Eulerkreis)**

>Falls ein Graph **keinen Eulerkreis** besitzt, kann er möglicherweise einen **Eulerpfad** haben. Ein Eulerpfad ist ein Weg, der jede Kante **genau einmal** benutzt, aber nicht notwendigerweise am Startknoten endet.

- **Bedingungen für einen Eulerpfad in ungerichteten Graphen**:
    
    - Der Graph ist zusammenhängend.
    - Genau **zwei Knoten haben ungeraden Grad**.
- **Bedingungen für einen Eulerpfad in gerichteten Graphen**:
    
    - Der Graph ist stark zusammenhängend.
    - Genau **ein Knoten hat einen Ausgangsgrad, der um eins größer ist als der Eingangsgrad**, und ein anderer Knoten hat einen Eingangsgrad, der um eins größer ist als der Ausgangsgrad.