>Die **Zermelo-Fraenkel-Mengenlehre (ZF)** ist ein axiomatisches System, das die Grundlage der modernen Mengenlehre bildet. Es wurde entwickelt, um die grundlegenden Eigenschaften von Mengen zu formalisieren und Paradoxien, wie sie in der naiven Mengenlehre auftreten, zu vermeiden. Mit der Hinzunahme des Auswahlaxioms wird das System als **ZFC** bezeichnet.

---

#### Die Axiome des Zermelo-Fraenkel-Systems

Das ZF-System besteht aus mehreren Axiomen, die verschiedene Aspekte von Mengen und ihrer Konstruktion definieren. Im Folgenden sind die wichtigsten Axiome ohne Verwendung von formalen Symbolen beschrieben:

---

1. **Axiom der Extensionalität**:
    
    - Zwei Mengen sind gleich, wenn sie genau dieselben Elemente enthalten.
    - Beispiel: Die Mengen {1,2,3}\{1, 2, 3\}{1,2,3} und {3,2,1}\{3, 2, 1\}{3,2,1} sind gleich, da sie dieselben Elemente enthalten.
2. **Axiom der leeren Menge**:
    
    - Es gibt eine Menge, die keine Elemente enthält, die sogenannte leere Menge.
    - Notation: Diese Menge wird oft als ∅\emptyset∅ geschrieben.
3. **Axiom der Paarbildung**:
    
    - Für beliebige Mengen AAA und BBB existiert eine Menge, die genau AAA und BBB als Elemente enthält.
    - Beispiel: Für die Mengen A={1}A = \{1\}A={1} und B={2}B = \{2\}B={2} existiert die Menge {{1},{2}}\{\{1\}, \{2\}\}{{1},{2}}.
4. **Axiom der Vereinigung**:
    
    - Für jede Menge AAA existiert eine Menge, die alle Elemente enthält, die Elemente von AAA sind.
    - Beispiel: Wenn A={{1},{2,3}}A = \{\{1\}, \{2, 3\}\}A={{1},{2,3}}, ist die Vereinigung von AAA die Menge {1,2,3}\{1, 2, 3\}{1,2,3}.
5. **Axiom der Potenzmenge**:
    
    - Zu jeder Menge AAA existiert eine Menge, die alle Teilmengen von AAA enthält (Potenzmenge).
    - Beispiel: Für A={1,2}A = \{1, 2\}A={1,2} ist die Potenzmenge {∅,{1},{2},{1,2}}\{\emptyset, \{1\}, \{2\}, \{1, 2\}\}{∅,{1},{2},{1,2}}.
6. **Axiom der Trennung (Schema)**:
    
    - Aus einer gegebenen Menge können Teilmengen gebildet werden, die eine bestimmte Eigenschaft erfüllen.
    - Beispiel: Aus der Menge A={1,2,3,4}A = \{1, 2, 3, 4\}A={1,2,3,4} kann die Teilmenge {2,4}\{2, 4\}{2,4} extrahiert werden, wenn die Eigenschaft "gerade Zahl" gewählt wird.
7. **Axiom der Unendlichkeit**:
    
    - Es existiert eine Menge, die die leere Menge enthält und für jedes ihrer Elemente auch die Menge enthält, die dieses Element und zusätzlich ein weiteres enthält.
    - Diese Menge bildet die Grundlage für die Konstruktion der natürlichen Zahlen.
8. **Axiom der Ersetzung (Schema)**:
    
    - Wenn eine Regel definiert wird, die jedem Element einer Menge ein eindeutiges Element zuordnet, dann existiert eine neue Menge, die aus genau diesen zugeordneten Elementen besteht.
    - Beispiel: Aus der Menge A={1,2,3}A = \{1, 2, 3\}A={1,2,3} kann durch die Regel "quadriere jedes Element" die Menge {1,4,9}\{1, 4, 9\}{1,4,9} gebildet werden.
9. **Axiom der Fundierung**:
    
    - Jede nicht-leere Menge enthält ein Element, das keine Elemente aus der Menge selbst enthält. Dies verhindert unendliche Abwärtsketten von Mengen.
    - Beispiel: Es kann keine Menge AAA geben, die sich selbst als Element enthält (A∈AA \in AA∈A).