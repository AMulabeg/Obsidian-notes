---
id: Lecture5_Beko
aliases: []
tags: []
---

# Bounties of LOOP Computability 

- What we know: 
    - All LOOP Computability is Total ([[Lecture3_Beko|Look Here For more info]])
- Question:
    - Are there total functions that are not LOOP-Computable? (Yes)(Diagonalisation)

![[Pasted image 20241122125648.png|500]]

- The left side represent the diagnalization ([[Diagonalization.md|Look here]] )
- The right side represents all the possible combinations of a list of LOOPs

- Theorem:
    - Let L be a list of all 1-digit LOOP-Computable functions. We then difine g:$\mathbb N \to \mathbb N$ with 
    $$  
        g(n):=L_n(n)+1 (1)
    $$
    total and not LOOP-Computable. (Due to there being no defined limit for n)

- To prove that L is not computable, we need to prove that a variable, for example g, is LOOP-Computable.
- This would mean that there exists a k $\epsilon \mathbb N$ with $L_k = g$ (2)
    $$
    \leadsto g(k) =^{1} L_k(k) + 1 =^{2} g(k) + 1
    $$
