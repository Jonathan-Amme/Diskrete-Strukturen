>Ein **Spannbaum** ist ein Teilgraph eines gegebenen Graphen \( G = (V, E) \), der folgende Eigenschaften erfüllt:
- **Zusammenhängend:** Der Spannbaum verbindet alle Knoten aus \( G \). 
- **Azyklisch:** Der Spannbaum enthält keine Zyklen. 
- **Minimal:** Der Spannbaum enthält genau \( |V| - 1 \) Kanten. 
Ein Spannbaum ist also ein Baum, der alle Knoten des ursprünglichen Graphen \( G \) enthält, aber so wenige Kanten wie möglich. 
---
## Eigenschaften 
1. Ein Spannbaum eines Graphen \( G \) hat: 
- \( |V| \) Knoten (alle Knoten des ursprünglichen Graphen), 
- \( |V| - 1 \) Kanten. 
2. **Existenz:** Jeder zusammenhängende Graph besitzt mindestens einen Spannbaum.
3. **Eindeutigkeit:** Wenn \( G \) ein vollständiger Graph ist und alle Kanten unterschiedliche Gewichte haben, gibt es genau einen minimalen Spannbaum.

![[Pasted image 20241127145449.png]]
