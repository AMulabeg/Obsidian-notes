---
id: Tutorium3_Beko
aliases: []
tags: []
---
- [ ] Finished
# LOOP

- LOOP $x_i$, DO $P_1$, END
- $x_i = x_j +/-x_y$


1.   

a) 
    $x_3=x_2+1$ 
    $x_4=x_1+0$
    LOOP $x_1$,
    DO $x_3$ - 1  -- This is $x_2 - x_1$
    LOOP $x_2$,
    DO $x_4$ - 1  -- This is $x_1 - x_2$
    LOOP $x_3$ do $x_3=x_{99}+1$
    LOOP $x_4$ do $x_4=x_{99}+1$ 
    LOOP $x_3$ do $P_1$
    LOOP $x_4$ do $P_2$ 

b)  $P_1 \text{and} P_2$
    LOOP $x_1$ DO
            IF $x_2 > x_1$
            THEN ($x_0:=x_1 +0$)
            ELSE $x_1:=x_1 - x_2$
        END
        $x_0 = x_1 +0$

## WHILE:
- LOOP Syntax
- WILE $x_1 \neq 0$ DO $P_1$ END

2. 

a)

f(4) = 2
f(3) = $\bot$

b)

- Checks if n a perfect square is

c) No, because loop functions can't be partal functions
### GOTO:
- IF $x_i$ = 0


3.
b) Fibonachi
c) 
