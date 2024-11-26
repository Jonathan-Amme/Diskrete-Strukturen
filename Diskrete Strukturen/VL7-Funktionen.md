# Äquivalenzrelation 
>Eine **Äquivalenzrelation** auf einer Menge A ist eine Relation $R⊆A×A$, die folgende drei Eigenschaften erfüllt:

1. **Reflexivität**:
    
    $∀a∈A:(a,a)∈R$
    
    Jedes Element steht zu sich selbst in Relation.
    
2. **Symmetrie**:
    
    $∀a,b∈A:(a,b)∈R  ⟹  (b,a)∈R$
    
    Wenn a in Relation zu b steht, dann steht auch b in Relation zu a.
    
3. **Transitivität**:
    
    $∀a,b,c∈A:(a,b)∈R∧(b,c)∈R  ⟹  (a,c)∈R$
    
    Wenn a in Relation zu b und b in Relation zu c steht, dann steht auch a in Relation zu c.
    
## **Äquivalenzklassen**

>Eine Äquivalenzrelation teilt eine Menge A in disjunkte Teilmengen, die sogenannten **Äquivalenzklassen**. Für ein Element $a∈A$ ist die Äquivalenzklasse:

$$[a]={x∈A∣(a,x)∈R}$$

#### Beispiel:

Bei der Kongruenz modulo n sind die Äquivalenzklassen die Restklassen:

$[a]n={b∈Z∣b≡a (mod n)}$

## Ordnungsrelationen
>Eine **Ordnungsrelation** auf einer Menge A ist eine Relation $R⊆A×A$, die mindestens die folgenden Eigenschaften erfüllt:

1. **Reflexivität** (schwache Ordnung) oder Antisymmetrie (strenge Ordnung):
    - Reflexivität: ∀a∈A:(a,a)∈R
    - Antisymmetrie: ∀a,b∈A:(a,b)∈R∧(b,a)∈R  ⟹  a=b
2. **Transitivität**:$∀a,b,c∈A:(a,b)∈R∧(b,c)∈R  ⟹  (a,c)∈R$
---

### **Arten von Ordnungsrelationen**

#### a) **Partielle Ordnung**

Eine Relation R auf A ist eine **partielle Ordnung**, wenn sie folgende Eigenschaften hat:

1. **Reflexivität**: $∀a∈A:(a,a)∈R$,
2. **Antisymmetrie**: $∀a,b∈A:(a,b)∈R∧(b,a)∈R  ⟹  a=b$,
3. **Transitivität**: $∀a,b,c∈A:(a,b)∈R∧(b,c)∈R  ⟹  (a,c)∈R$

##### Beispiel:

- Teilmengenrelation ⊆ auf der Potenzmenge P(A).
- Teilbarkeitsrelation ∣ auf $Z^+$.

#### b) **Totale Ordnung**

Eine Relation R auf A ist eine **totale Ordnung**, wenn sie eine partielle Ordnung ist und zusätzlich:
$$∀a,b∈A:(a,b)∈R oder (b,a)∈R.$$

Jedes Paar von Elementen ist vergleichbar.

##### Beispiel:

- Natürliche Ordnung ≤ auf R.
- Alphabetische Ordnung bei Wörtern.

#### c) **Strenge Ordnung**

Eine Relation R ist eine **strenge Ordnung**, wenn sie:

1. **Irreflexiv**: ∀a∈A:(a,a)∉R
2. **Transitiv**: $∀a,b,c∈A:(a,b)∈R∧(b,c)∈R  ⟹  (a,c)∈R$

##### Beispiel:

- „Kleiner als“ (<) auf R.