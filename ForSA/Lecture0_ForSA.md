---
id: Lecture0_ForSa
aliases: []
tags: []
---

   
# Aussagenlogik/Propositional Logic

- Junktoren : { 
    - $\vee$ - OR, 
    - $\wedge$ - AND,
    - $\rightarrow$ - Implies,
    - $\leftrightarrow$ - Exactly when, then
    - $\neg$ - Negation
    } $\cup$ { $\forall, \exists$ }

- Propositional Variables {
    - V = {p,q,... } $\Rightarrow \beta \text{(p)} \epsilon \text{\{1,0}\}$
    - $\top$ -> True $\textlbrackdbl{\top}\textrbrackdbl^{\beta}=1$
    - $\bot$ -> False $\textlbrackdbl{\bot}\textrbrackdbl^{\beta}=0$
    } 

## What is a Logical statement?
- Is a set of arguments that is represented through a formal language that proves if a statement is true (1) or false (0)
- This is represented through logical junctions and prepositional variables
- Every problem can be broken down into a When, then problem, and the result will always be true (1) or false (0)
    - When is represented through "Annahme"
    - Then is represented through "Beweis"
- For example:
    - $\phi \vee \neg\phi \equiv \top$ -> This is ALWAYS True as $\vee$ is "either or" meaning 0 and 1 make 1 
    - $\sum_{k=0}^{n} k = \frac{n(n+1)}{2}$ -> This is a formula that proves that there is a sum of numbers between 0 and n
        - This formula can be broken down well using the when, then statment
        - (A1) n$\epsilon \mathbb{N}$
        - (Z1) $\sum_{k=0}^{n} k = \frac{n(n+1)}{2}$ 


- A Conjunction is a representation of an "and" logical statement

- A Disjunction is a representation of an "or" logical statement

### Conjunction

![[Pasted image 20250423181320.png]]

- If we want to prove a conjunction within a logical statement we can break it down into this:
    - Example:
        - If the conjunction is in the "Annahme": (A1): $P_{1}(x) \wedge P_{2}(y)$, we can take the singular terms are already correct and we can look at them separately
        
            - Annahme (A2): $P_{1}(x)$
            - Annahme (A3): $P_{2}(y)$
            
	    -  Else if the conjunction is in the "Ziel": (Z1): $P_{1}(x) \wedge P_{2}(y)$, we have to prove that each of the points are vaild by themselves
	    
            - Teil 1: Zu Zeigen(Z1.1): $P_{1}(x)$
            - Teil 1: Zu Zeigen(Z2.1): $P_{2}(x)$

#### Disjunction
![[Pasted image 20250428154345.png]]

- If we want to prove a disjunction within a logical statement we can break it down into this:
    - Example:
        - If the disjuction is in the "Ziel": (Z1):$P_{1}(x) \vee P_{2}(y)$, we "only" have to prove that one side is correct, therefore we can choose which side we want:
            - Zu Zeigen (Z2): $P_{i}(z)$ (Again, the target doesn't matter)

        - Else if the disjuction is the "Annahme": (A1):$P_{1}(x) \vee P_{2}(y)$, we have to prove that at least 1 of the sides is correct at any given moment. Therefore we need to make a case:
            - Fall 1: Annahme(A1.1):$P_{1}(x)
            - Fall 2: Annahme(A2.1):$P_{2}(y)

- Summary:![[Pasted image 20250428160703.png]]



