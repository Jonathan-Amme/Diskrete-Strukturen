### Wiederholung: Zusammenhang bei Digraphen
(G = (V, E), Digraph G mit Knotenmenge V und Kantenmenge E)
- zusammenhängend ($u(E\cup E^{-1})\text{*} v)$ 
	- "Alle Knoten sind durch Kanten (Richtung egal) verbunden."
- stark zusammenhängend ($u E \text{*}v$ und $v E \text{*}u$ für alle $u, v \in V$)
	- "Alle Knoten sind in beide Richtungen verbunden."
- (starke) Zusammenhangskomponente ($G[U]$ (stark) zusammenhängend ($U \subseteq V$))
	- "Teilgraph von G, der (stark) zusammenhängend ist."
- maximale (starke) Zusammenhangskomponente
	- "Teilgraph von G, der (stark) zusammenhängend ist und keine Verbindung zu anderen Knoten außerhalb des Teilgraphen ist"
	- Beispiel
		- Für einen ungerichteten Graphen mit den folgenden Knoten und Kanten:
			- Knoten: {A, B, C, D, E, F}
			- Kanten: {(A, B), (B, C), (D, E)}
			- maximale Zusammenhangskomponenten
				- {A, B, C} (alle Knoten sind miteinander verbunden)
				- {D, E} (verbunden, aber getrennt von anderen Knoten)
				- {F} (dieser Knoten ist isoliert)
### Zusammenhang bei ungerichteten Graphen
- ungerichteter Graph G = (V, E)
- zusammenhängend (für jedes Paar $u, v \in V$ mit $u \neq v$ gibt es einen verbindenden Pfad)

### Wiederholung: Bäume
- Ein Baum ist ein kreisfreier und zusammenhängender Graph
- Ein Baum mit $n$ Knoten hat genau $n -1$ Kanten
- Jeder Baum mit $|V| \geq 2$ hat mindestens zwei Blätter
### Spannbäume
- Definition
	- Sei $G = (V, E)$ ein einfacher Graph
	- Dann ist $T = (V, E')$ mit $E' \subseteq E$ ein Teilgraph, der selbst ein Baum ist. Man nennt diesen dann **Spannbaum von G**
	- Jeder zusammenhängende Graph hat einen Spannbaum. Man entfernt einfach jede Kante, die nicht für den Zusammenhang nötig ist
	