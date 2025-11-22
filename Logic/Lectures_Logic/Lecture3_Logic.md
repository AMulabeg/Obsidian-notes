---
id: Lecture3_Logic
aliases: []
tags: []
---

# Normalform and Substitution

## Central Idea of Logic
- Let $\varphi,\psi \epsilon AL$ Formula:
    - **Model**: 
        - For a $\varphi$ there is a fitting occupancy $\beta$ that fulfills $\varphi$, or a modal from $\varphi$, when $\textlbrackdbl \varphi \textrbrackdbl ^{\beta} = 1$. We write $\beta \models \varphi$
    - $**Conclusion (Folgerung)**:
        - $\psi$ follows from  $\varphi$, written as $\varphi \models \psi$, for all fitting $\varphi$ and $\psi$ for the fitting occupancy $\beta$:
        - When $ \beta \models \varphi$, then is $\beta \models \psi$
    - **Equivalence (Äquivalenz)**:
        - $\varphi and \psi$ are equivalent, $\varphi \equiv \psi$, when for all $\psi, \varphi$ there exists a fitting occupancy $\beta \models \varphi$, exactly when $\beta \models \psi$
    - **Feasibility (Erfüllbarkeit)**:
        - $varphi$ if feasible, if there is a occupancy $\beta$ that fulfills $\varphi$
            - else, $\varphi$ is not feasible
    - **Universal Validity (Allgemeingültig)**:
        - $\psi$ is universaly valid, or is a Tautologie, if for each $\psi$ there is a fitting occupancy $\psi$

        


- Let $\varphi, \psi \in AL$ formulas and $\Phi, \Psi \subseteq AL$ formula sets:

    - **Model (Modellbeziehung):**
        - A valuation $\beta$ fits $\varphi$ if $\beta$ satisfies every $\varphi \in \Phi$.
        - $\beta \models \varphi$ if $\beta \models \varphi$ for all $\varphi \in \Phi$.
        - For a single formula: a valuation $\beta$ satisfies $\varphi$ (is a model of $\varphi$) when $\textlbrackdbl \phi \textrbrackdbl ^{\beta} = 1$:
          We write $\beta \models \varphi$.

    - **Conclusion (Folgerung):**
        - $\psi$ follows from $\varphi$, written $\Phi \models \psi$, if for every valuation $\beta$ that fits $\Phi$:
        - If $\beta \models \varphi$ for all $\varphi \in \Phi$, then $\beta \models \psi$.

    - **Equivalence (Äquivalenz):**
        - $\varphi$ and $\Psi$ are equivalent, written $\Phi \equiv \Psi$, if for every fitting valuation $\beta$:
        - $\beta \models \varphi$ exactly when $\beta \models \Psi$.

    - **Satisfiability (Erfüllbarkeit):**
        - $\varphi$ is satisfiable if there exists a valuation $\beta$ that satisfies $\Phi$.
        - Otherwise, $\varphi$ is unsatisfiable.

    - **Universal Validity (Allgemeingültigkeit):**
        - $\varphi$ is universally valid, or a tautology, if every valuation $\beta$ satisfies $\varphi$.

   



