---
id: Lecture2_Beko
aliases: []
tags: []
---

# Computability Concept

- Intuitive Computablity:
    - Input -> Algorithm -> Output
     
    - Examle of Algorithms: Although people can intuitively calculate $\{a^n b^n | n>= 0\}$
        - [[Lecture1_BeKo#Finite Automata|DFA]]:
            - Limited Resources (We do not have infinite storage)

        - [[Lecture1_BeKo#turing-machines|Turing Machine]]:
            - Storage and RAM are **NOT** limited

        - LOOP -/WHILE-/GOTO Programs:
            - Variable size is **NOT** limited


- Definition:
    - A (partial) function $f:\mathbb N^k -> \mathbb N$ is called computable when there is a finite algorithm $\mathbb A$, so that for all $n_1 ....., n_k, m \epsilon \mathbb N$, we have:
        - $f(n_1,.....n_k) =m$ <==> for input $(n_1,....n_k)$, $\mathbb A$ stops after a finite time with the output m

- Existential Example:
    - 1 (k=1):
    1. INPUT (n)
    2. WHILE true DO {}
    ~> $\Omega: \mathbb N$ -> $\mathbb N$ with $n$ |->$\bot$


- Example 2:


$$
f(n) := \begin{cases} 
1, & \text{in case } \exists_{i \in \mathbb{N}} \left\lfloor \pi \cdot 10^i \right\rfloor = n \\
0, & \text{else}
\end{cases}
$$

- Explanation: 

    - $f(n) = 1$ when n is exactly the "The first decimal point" of $\pi$
    - Algorithm:
        - Approximate $\pi$ (Sufficiently Accurately)
        - Compare to input
    
    - Here are more examples:
    ![[Pasted image 20241030150026.png]]



- Problem: Computablity Concept is based on the definition from the "Church–Turing Thesis"
    - Intuitive Computablity = Turing Predictability


### Turing-Computability

- A (eventually partial) function $f: \mathbb N^k$ -> $\mathbb N$ is turing-computable when a DTM M = $(Z, \Sigma,\Gamma,\delta, z_0, \square, E)$ exists so that for all $n_1,.....n_k, m \epsilon \mathbb N$ we have $f(n_1,....n_k)$ = m <==> for input $(n_1,...n_k)$  $\mathbb A$ terminates after finite time with the output m.
    - <==> $\exists_{z \epsilon E}z_0$ BIN($n_1$)#...BIN($n_k$): 
    - With BIN being binary representation of a number
- A (eventually partial) function $f: \Sigma^*$ ->$\Sigma^*$ is Turing computable when there is a $\text{DTM M} = (Z, \Sigma, \Gamma, \delta, z_0, \square, E)$ so that for all $x,y \epsilon \Sigma^*$ the following is true:
    - $f(x)=y$ <==> $\exists_{z \epsilon E} z_0x \vdash_M^* zy$

- A Language L is:
    - Decidable when $\mathbb X_L$ is computable
    - Semi-Deicable when $\mathbb X'_L$ is computable

- Characteristic Function:
$$
f(n) := \begin{cases} 
1, & \text{in case } x \epsilon L \\
0, & \text{in case } x \not{\epsilon} L
\end{cases}
$$

- Half Characteristic Function:
$$
f(n) := \begin{cases} 
1, & \text{in case } x \epsilon L \\
\bot, & \text{in case } x \not{\epsilon} L
\end{cases}
$$



![[Pasted image 20241104134307.png]]


#### Multiband Turing Machines

![[Pasted image 20241104134415.png]]

- Transfer Function $\delta: (Z \backslash E) \times \Gamma^{k}$ -> $Z \times (\Gamma \times {L,R,N})^{k}$
    - $\Gamma^{k}$ -> All symbols on the all k Turing Machines

- Configuration: $\alpha_1 z \beta_1,\alpha_2 \circ \beta_1,......,\alpha_k \circ \beta_k$
- [[Lecture1_BeKo#turing-machines|Start Configuration]]: $z_0 x_1, \circ x_2,..., \circ x_k$
- Follow Configuration: $\vdash_M^1$ 

- For $z \epsilon Z \; \text{and} \;z_e \epsilon E \;\text{and}\; \alpha_1.....\alpha_k,\beta_1.....,\beta_k \epsilon \Gamma^*$
- Calculation of the Function:
    - $BIN(x_1),BIN(x_2),....BIN(x_k) \vdash_M^* z_e BIN(f(x_1,....,x_k)), \alpha_2 \circ \beta_2,....\alpha_2 \circ \beta_2,...., \alpha_k \circ \beta_k$

- Acceptance of the Language:
    - $BIN(x_1),BIN(\square),....BIN(\square) \vdash_M^* z_e BIN(f(x_1,....,x_k)), \alpha_2 \circ \beta_2,....\alpha_2 \circ \beta_2,...., \alpha_k \circ \beta_k$

![[Pasted image 20241104140358.png]]

##### Multiband-TM Equivalence

- For every k-band-TM M we have a single-band TM Q with T(M) = T(Q)
    - This means that a k-band-TM can't fix issues that a single-band TM has, meaning they both have the same limitations


![[Pasted image 20241104143324.png]]
- For k-tape TM we have:
    - We can simulate M with Q (fat tape)
    - To simulate M, Q must have 2k "Lanes". One lane contains symbols from the $\Gamma$, the other lane contains only 0,1
        - We read 2 lanes at the same time. When we read a 1, we add the represented symbol from the other lane
	
![[Pasted image 20241104143434.png]]

- $\Gamma_{Q} = (\Gamma_M \times {0,1})^k$
	- $S_M: (Z \backslash E) \times T_M^k$ -> $Z_M \times \{L,R,N\}^k$
