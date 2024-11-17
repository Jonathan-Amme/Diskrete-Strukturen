
>Ein **Beweis** ist eine logische Argumentation, die zeigt, dass eine gegebene Aussage oder ein Theorem wahr ist. Ein Beweis beginnt in der Regel mit Axiomen, Definitionen oder vorher bewiesenen Theoremen und verwendet logische Schlussfolgerungen, um zur gewünschten Aussage zu gelangen.

# Arten von Beweisen

### Direkter Beweis

>Beim direkten Beweis zeigt man, dass aus den Voraussetzungen P logisch die Schlussfolgerung Q folgt. Man startet mit der Annahme, dass P wahr ist, und leitet Schritt für Schritt ab, dass Q ebenfalls wahr sein muss.

#### Beispiel:

**Aussage**: "Wenn eine Zahl gerade ist, dann ist ihr Quadrat ebenfalls gerade."
$$

$$
- **Voraussetzung**: n ist eine gerade Zahl, also gibt es eine ganze Zahl k, sodass n=2k
- **Schritt 1**: $n^2=(2k)^2=4k^2$
- **Schlussfolgerung**: Da $n^2=4k^2$, ist $n^2$ eine gerade Zahl (da es durch 2 teilbar ist).

### Indirekter Beweis (Widerspruchsbeweis)

>Beim **indirekten Beweis** (auch als **Beweis durch Widerspruch** bekannt) nimmt man an, dass die zu beweisende Aussage falsch ist und leitet daraus einen Widerspruch ab. Wenn diese Annahme zu einem Widerspruch führt, muss die ursprüngliche Aussage wahr sein.

#### Beispiel:

**Aussage**: "Es gibt unendlich viele Primzahlen."

- **Annahme**: Es gibt nur endlich viele Primzahlen.
- **Schritt 1**: Sei $p1,p2,...,pn$ die Menge aller Primzahlen.
- **Schritt 2**: Betrachte die Zahl $N=p1⋅p2⋅...⋅pn+1$
- **Schlussfolgerung**: N ist nicht durch eine der Primzahlen teilbar, was einen Widerspruch zur Annahme führt, dass es nur endlich viele Primzahlen gibt.
- **Ergebnis**: Die Annahme ist falsch, also gibt es unendlich viele Primzahlen.

### Beweis durch vollständige Induktion

Dieser Beweis wird verwendet, um Aussagen über natürliche Zahlen zu beweisen. Der Beweis erfolgt in zwei Schritten:

1. **Induktionsbasis**: Zeige, dass die Aussage für den kleinsten Wert (oft n=1) gilt.
2. **Induktionsschritt**: Zeige, dass, wenn die Aussage für $n=k$ gilt, sie auch für $n=k+1$ gilt.

#### Beispiel:

**Aussage**: Für alle $n∈Nn$ gilt: $1+2+3+...+n= \frac{n(n+1)}{2}$.

- **Induktionsanfang**: Für $n=1: 1=\frac{1(1+1)}{2} = 1$ (wahr).
- **Induktionsannahme**: Angenommen, die Aussage gilt für $n=k$, d.h. $1+2+...+k= \frac{k(k+1)}2.$
- **Induktionsschritt**: Zeige, dass die Aussage für $n=k+1$ gilt: $1+2+...+k+(k+1)= \frac{k(k+1)}{2} + (k+1) = \frac{k(k+1) + 2(k+1)}{2} = \frac{(k+1)(k+2)}{2}$. Damit ist die Aussage für $n=k+1$ ebenfalls wahr.

### Beweis durch Fallunterscheidung

>Beim **Beweis durch Fallunterscheidung** wird das zu beweisende Problem in verschiedene Fälle aufgeteilt, und jeder Fall wird separat bewiesen. Wenn alle möglichen Fälle geprüft und bewiesen wurden, ist die Aussage wahr.

#### Beispiel:

**ge**: "Das Quadrat einer ganzen Zahl ist entweder eine gerade oder eine ungerade Zahl."

- **Fall 1**: Sei n gerade, also n=2k. Dann ist $$n^2=(2k)^2=4k^2$$, was eine gerade Zahl ist.
- **Fall 2**: Sei n ungerade, also n=2k+1. Dann ist $$n^2=(2k+1)^2=4k^2+4k+1^2$$, was eine ungerade Zahl ist.
- **Schlussfolgerung**: In beiden Fällen ist die Aussage wahr.

# Formale Beweisstruktur

Die Struktur eines formalen Beweises kann wie folgt dargestellt werden:

1. **Gegeben**: Nenne die Voraussetzungen, Axiome oder Hypothesen, die als wahr angenommen werden.
2. **Zu Zeigen**: Die Aussage oder das Theorem, das bewiesen werden soll.
3. **Beweis**:
    - Schrittweise logische Ableitungen, basierend auf den gegebenen Voraussetzungen und gültigen logischen Regeln.
    - Jede Schlussfolgerung sollte klar auf vorhergehenden Annahmen oder Regeln basieren.
4. **Q.E.D.**: Am Ende des Beweises schreibt man oft **Q.E.D.** (abgeleitet aus dem Lateinischen „quod erat demonstrandum“), was „was zu zeigen war“ bedeutet.

# Übungen
## Übung(Woche 1/Aufgabe 3):
### Aufgabenstellung
![[Pasted image 20241115190409.png]]
### Lösung
![[Pasted image 20241115190435.png]]
## Übung(Woche 1/Aufgabe 4):
### Aufgabenstellung
![[Pasted image 20241115190548.png]]
### Lösung
![[Pasted image 20241115190617.png]]
## Übungen(Woche 2/Aufgabe 4)
### Aufgabenstellung
![[Pasted image 20241115191630.png]]
### Lösung
![[Pasted image 20241115191656.png]]
![[Pasted image 20241115191714.png]]
## Übungen(Woche 2/Hausaufgabe 2)
### Aufgabenstellung
![[Pasted image 20241115191823.png]]
### Lösung
![[Pasted image 20241115191858.png]]
![[Pasted image 20241115191926.png]]
