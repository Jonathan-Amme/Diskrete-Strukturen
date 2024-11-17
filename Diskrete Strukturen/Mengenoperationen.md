## Grundlagen der Mengenlehre

>Eine **Menge** ist eine Zusammenstellung von klar definierten und unterscheidbaren Objekten, genannt Elemente. Zwei Mengen A und B heißen **disjunkt**, wenn sie keine gemeinsamen Elemente haben, d.h. A∩B=∅. Diese werden in geschweiften Klammern notiert, z.B.:

*A={1,2,3},B={a,b,c}*
![[Pasted image 20241115195401.png]]

### Notationen

- **Element einer Menge**: x∈Ax bedeutet, dass das Element x in der Menge A enthalten ist.
- **Leere Menge**: ∅ ist die Menge ohne Elemente.
- **Teilmenge**: A⊆B bedeutet, dass alle Elemente von A auch in B enthalten sind.

---

## Mengenoperationen

### Vereinigung (Union)

>Die **Vereinigung** zweier Mengen A und B enthält alle Elemente, die entweder in A oder B oder in beiden enthalten sind:

*A∪B={x∣x∈A oder x∈B}*

**Beispiel**:

*A={1,2,3},B={3,4,5}⇒A∪B={1,2,3,4,5}*

### Durchschnitt (Intersection)

Der **Durchschnitt** zweier Mengen A und B enthält alle Elemente, die sowohl in A als auch in B enthalten sind:

*A∩B={x∣x∈A und x∈B}*

**Beispiel**:

*A={1,2,3},B={3,4,5}⇒A∩B={3}*

### Differenz (Difference)
>Die **Differenz** A∖B enthält alle Elemente, die in A, aber nicht in B enthalten sind:

*A∖B={x∣x∈A und x∉B}*

**Beispiel**:

*A={1,2,3},B={3,4,5}⇒A∖B={1,2}*

### Symmetrische Differenz

Die **symmetrische Differenz** zweier Mengen A und B enthält alle Elemente, die entweder in A oder in B sind, aber nicht in beiden gleichzeitig:

*AΔB=(A∖B)∪(B∖A)*

**Beispiel**:

*A={1,2,3},B={3,4,5}⇒AΔB={1,2,4,5}*

---

## Kartesisches Produkt

>Das **kartesische Produkt** zweier Mengen A und B, bezeichnet als A×B, ist die Menge aller geordneten Paare (a,b), wobei a∈A und b∈B:

*A×B={(a,b)∣a∈A,b∈B}*

**Beispiel**:

*A={1,2},B={a,b}⇒A×B={(1,a),(1,b),(2,a),(2,b)}*
 
---

## Komplement

>Das **Komplement** einer Menge A im Bezug auf eine Grundmenge U (Universum) enthält alle Elemente, die in U, aber nicht in A enthalten sind:

$A^c=U∖A$

**Beispiel**: Wenn U={1,2,3,4,5} und A={1,2}, dann ist Ac={3,4,5}.

---

## Gesetze der Mengenlehre

### Assoziativgesetz
$$A∪(B∪C)=(A∪B)∪C, A∩(B∩C)=(A∩B)∩C$$
### Distributivgesetz
$$A∪(B∩C)=(A∪B)∩(A∪C), A∩(B∪C)=(A∩B)∪(A∩C)$$

### De Morgan'sche Gesetze
Die [[De Morgan'schen Regeln]] sind grundlegende Gesetze in der Mengenlehre und Logik, die den Zusammenhang zwischen den logischen Operationen der Negation, Konjunktion und Disjunktion (bzw. in der Mengenlehre Durchschnitt und Vereinigung) beschreiben.