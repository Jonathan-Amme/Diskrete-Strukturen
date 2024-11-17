>Eine **Menge** ist eine grundlegende mathematische Struktur, die eine Sammlung von Objekten, den sogenannten **Elementen**, zusammenfasst. Diese Objekte können Zahlen, Buchstaben, andere Mengen oder abstrakte Konzepte sein. Mengen sind ein zentrales Konzept in der Mathematik und bilden die Grundlage der modernen Mengenlehre.
# Eigenschaften von Mengen
## Eindeutigkeit der Elemente
- Jedes Element einer Menge ist eindeutig. Eine Menge kann keine doppelten Elemente enthalten.
- Beispiel: {1,2,3} und {1,1,2,3} sind gleich, da doppelte Einträge ignoriert werden.

---

## Ungeordnetheit

- In einer Menge spielt die Reihenfolge der Elemente keine Rolle.
- Beispiel: {1,2,3} = {3,2,1}.

---

#### 3. **Endlichkeit und Unendlichkeit**

- Eine Menge kann endlich (z. B. {1,2,3}) oder unendlich (z. B. {1,2,3,… }) sein.
## Mächtigkeit einer Menge

>Die **Mächtigkeit** (auch Kardinalität genannt) einer Menge ist die Anzahl der Elemente in der Menge.

- Für endliche Mengen ist die Mächtigkeit die Anzahl der Elemente. Beispiel: ∣A∣=3|, wenn A={1,2,3}.
    
- Für unendliche Mengen spricht man von unendlicher Mächtigkeit. Beispiel: ∣N∣=∞, wenn N die Menge der natürlichen Zahlen ist.
    

---


## Gleichheit von Mengen

Zwei Mengen A und B sind **gleich** (geschrieben A=B), wenn sie genau die gleichen Elemente enthalten. Dies bedeutet, dass A⊆B und B⊆A.
$$A=B⇔∀x(x∈A⇔x∈B)$$

---
# Wichtige Mengen
## Endliche und unendliche Mengen

- **Endliche Mengen**: Mengen, die eine endliche Anzahl von Elementen enthalten.  
    Beispiel: A={1,2,3}.
    
- [[Unendliche Mengen]]: Mengen mit unendlich vielen Elementen.  
    Beispiel: N={1,2,3,…} (die Menge der positiv natürlichen Zahlen).
## Teilmenge

>Eine Menge A ist eine **Teilmenge** einer Menge B, wenn jedes Element von A auch ein Element von B ist. Dies wird durch A⊆B ausgedrückt.

$$A⊆B⇔∀x(x∈A→x∈B)$$

- **Echte Teilmenge**: A⊂B bedeutet, dass $A⊆B$ und $A≠B$.
- 
## Potenzmenge

>Die **Potenzmenge** P(A) einer Menge A ist die Menge aller **Teilmengen** von A. Sie enthält auch die leere Menge und die Menge A selbst.

$$P(A)={B∣B⊆A}$$

Beispiel:  
Sei A={1,2}, dann ist die Potenzmenge von A:
$$P(A)={∅,{1},{2},{1,2}}$$
Die Mächtigkeit der Potenzmenge P(A) ist $2 ^A$.
![[Pasted image 20241115195058.png]]
## Leere Menge

Die **leere Menge** ∅ ist die Menge, die **keine** Elemente enthält.

∅={}

*Eigenschaften:*
- Die leere Menge ist eine **Teilmenge** jeder anderen Menge.
- ∅⊆A gilt für jede Menge A.
## Partition
Eine Partition einer Menge A ist eine Sammlung von Teilmengen {A1,A2,…,An}, die folgende Eigenschaften erfüllen:

1. **Vereinigung**: Die Vereinigung aller Teilmengen ergibt die ursprüngliche Menge:
    
    $$A1∪A2∪⋯∪An=A$$
2. **Disjunktheit**: Die Teilmengen überschneiden sich nicht:
    
    $$Ai∩Aj=∅ für i≠j$$
3. **Nicht-Leere Teilmengen**: Keine der Teilmengen ist leer:
    
    $$Ai≠∅$$
![[Pasted image 20241115195324.png]]

## Weiterführende Themen

### Mengenoperationen

Für eine ausführliche Erklärung der grundlegenden Mengenoperationen wie **Vereinigung**, **Durchschnitt**, **Differenz** und **Komplement**, siehe [Mengenoperationen](Mengenoperationen).

---

### Beweise mit Mengen

Beispiele für Beweise, die Mengen involvieren, wie der Nachweis von Teilmengen oder Gleichheit von Mengen, [Beweise mit Mengen](Beweise).

---

### Mengenaxiome

Für eine detaillierte Diskussion über die **Axiome der Mengenlehre** (z.B. das [[Zermelo-Fraenkel-System]]), siehe [Mengenaxiome](link: Mengenaxiome).

---
### Veranschaulichung von Mengen
![[Pasted image 20241115194902.png]]

# Übungen
