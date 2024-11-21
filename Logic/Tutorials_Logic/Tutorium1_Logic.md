---
id: Tutorium1_Logic
aliases: []
tags: []
---
# Beweise

- Direct Proof
- Proof through Contradiction
- Proof through Contrposition
- Full step Induction

1. 
    (i) $\phi_0$ = A $\vee \textlnot A$  -> Universally Valid; For every occupancy $\beta$, regardless if the input is 0 or 1, it will always be valid
    (ii) $\phi_1$ = X $\wedge$ (Y $\vee$ Z) -> Fulfilable, but not Universally Valid; Cases like this happen because the formula can be fulfiable for certain combination of variables, but not all
    (iii) $\phi_2$ = (Y$\to$Z)$\wedge$(Y $\to$ Z$\vee$X))$\vee \textlnot$Z -> Universally Valid
        - We can prove this with using **contradiction** that this is Valid.
        - Take into consideration that there is a fitting $\beta$ that proves that the formula is **not** fulfillable. 
        - We can take into consideration that $\beta$(Z) = 1, otherwise the formula is valid. This also means that $\textlbrackdbl{Z \to Y}\textrbrackdbl^{\beta}$ = 1 and so is  $\textlbrackdbl{Z \vee X}\textrbrackdbl^{\beta}$ = 1.
        - With this we can say that  $\textlbrackdbl{Y \to Z \vee X}\textrbrackdbl^{\beta}$ = 1 and  $\textlbrackdbl{Y \to Z}\textrbrackdbl^{\beta}$
        - This means that the formula does **not** complete the contradiction meaning it is Universally Valid
    (iv) $\phi_3$ = (D$\Leftrightarrow$E)$\wedge$(A$\wedge$B$\wedge$(A$\vee$B))$\wedge$(C$\Leftrightarrow$D)$\wedge$(E$\Leftrightarrow \textlnot$C) -> This formula is not fulfilabe because in any combination of inputs, we yield 0;
        - In the first case: $\beta$(C) = 1, due to the case (C$\Leftrightarrow$D), $\beta$(D) must also equal to 1. Due to the case D$\Leftrightarrow$E), $\beta$(E) must also equal 1. **However**, due to E$\Leftrightarrow \textlnot$C), for this to equal 1, $\beta$(C) must be 0, but we have $\beta$(C) defined as 1. Therefore the function does not work. 
        - If you do this for $\beta$(C) = 0, the outcome is the same

2. 
    H = Hammerkopf 
    A = Amboss 
    E = Eisen
    R = Rechen
    C = Külen
    T = Temperaturen
    K = Kupfer


    a) $\phi_1:$ H$\to$A
    b) $\phi_2:$ E$\vee$R$\vee$C
    c) $\phi_3:$ E$\wedge$A$\to$T
    d) $\phi_4:$ K$\wedge$T$\Leftrightarrow \textlnot$E

    e) $\beta \vDash \psi$ so that:
       $\beta \vDash \phi_1$ 
       $\beta \vDash \phi_2$ 
       $\beta \vDash \phi_3$ 
       $\beta \vDash \phi_4$ 
    - Result:
       $\beta$(H) = 1
       $\beta$(A) = 1
       $\beta$(T) = 1
       $\beta$(E) = 0
       $\beta$(K) = 1
       $\beta$(R) = 0 
       $\beta$(C) = 0 

   f) $\psi:$H$\wedge \textlnot$E$\wedge$ $\phi_1 \wedge \phi_2 \wedge \phi_3 \wedge \phi_4$
       $\beta$(H) = 1
       $\beta$(A) = 1
       $\beta$(T) = 1
       $\beta$(E) = 0
       $\beta$(K) = 1
       $\beta$(R) = 0 
       $\beta$(C) = 0 





