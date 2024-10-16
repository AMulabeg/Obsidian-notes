---
id: Lecture1_BeKo
aliases: []
tags: []
---

# Introduction

# The "Hello World" - Problem

-  Goal: Develop a Program E with the following specs:
    -  Input: Program P
    -  Output: Print: "Top", when P contains the string "Hello, World", else print: "Flop"
-  Remark: E has "A type of higher order",(which means that the input is text from a program P)
-  Ex: 
``` C
    main() {
      printf("Hello, world");
    }```

-  Does there exist a program E for a special input P? ->  Yes
-  Does there exist a program E for every program P? -> Not possible

## Finite Automata

-  A deterministic finite automata (DFA) is a quintuple M = {Z,$\Sigma, \delta, z\_0, E$} with:
    - Z is a non empty, finate group of states
    - $\Sigma$ is a non empty, finite alphabet of input characters with $Z\cap E = 0$ 
    - $\delta: Z\times \Sigma$ -> Is a partial transfer function
    - For M we define a partial function $\delta: Z\times\Sigma^*$ -> Z is inductive for all  $z \epsilon Z$:
        - $\delta (z, \epsilon):=z$
        - $\forall x \epsilon \Sigma^{\ast} \quad \delta (z, ax):= \hat{\delta}(\delta(z,a),x)$ in case $\delta(z,a) != \bot$
 
    - A DFA M = {Z,$\Sigma, \delta, z\_0, E$} accepts a word $W \epsilon E$ if $\hat{\delta}(z_0,w)\epsilon E$ 

    - The words from M are an accepted language:
        - T(M):= {${x \epsilon \Sigma^{\ast} \;| \; \hat{\delta}(z_0,x)\epsilon E}$}

    Example:

    - M = ($\{z_0, z_1, z_2\},\{ 0,1\}, \delta ,z_0,\{ z_2\}$)
    
        |$\delta| \ z_0| \ z_1|\ z_2|$
        ----------
        |0|$\ z_0|\ z_2|\ z_1|$
        |1|$\ z_1| \ z_0|\ z_2 |$


 










