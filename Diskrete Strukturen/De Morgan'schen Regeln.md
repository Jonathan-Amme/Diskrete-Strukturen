## Allgemeine Form der De Morgan'schen Regeln

Die beiden De Morgan'schen Gesetze lauten:

1. Die Negation einer Vereinigung ist der Durchschnitt der Negationen:
	$$¬(A∪B)=¬A∩¬B$$
    
2. Die Negation eines Durchschnitts ist die Vereinigung der Negationen:
    
    $$¬(A∩B)=¬A∪¬B$$    
Diese Regeln lassen sich sowohl in der Aussagenlogik als auch in der Mengenlehre anwenden und sind eng miteinander verbunden.

## Beweis der De Morgan'schen Regeln

Hier ist ein kurzer Beweis der Regeln in der Mengenlehre.

### Beweis des ersten Gesetzes

>Wir wollen zeigen, dass:
$$
(A \cup B)^c = A^c \cap B^c$$
Sei $x∈(A∪B)^c$. Das bedeutet, dass x weder in A noch in B liegt, also:

$$x \in A^c \quad \text{und} \quad x \in B^c$$

>Daraus folgt, dass:
$$x \in A^c \cap B^c$$

>Also gilt:

$$(A \cup B)^c \subseteq A^c \cap B^c$$

>Umgekehrt, sei $x \in A^c \cap B^c$. Das bedeutet, dass x weder in A noch in B liegt, also:

$$x \in (A \cup B)^c$$
>Also gilt:

$$A^c \cap B^c \subseteq (A \cup B)^c$$

### Beweis des zweiten Gesetzes

>Analog lässt sich zeigen, dass:

$$(A \cap B)^c = A^c \cup B^c$$

>Indem wir die Negation und die logischen Verknüpfungen ähnlich behandeln.