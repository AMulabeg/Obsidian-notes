---
id: BigPractice1_Bako
aliases: []
tags: []
---

1. A Turing Machine (DTM) is a septuple group M = $(Z, \Sigma , \Gamma , \delta, \ z_0, \boxed  \,, E)$ with:
    -  Z is a non empty, finate group of states
    -  $\Sigma$ is a non empty, finite alphabet of input characters with $Z\cap E = 0$ 
    -  $\Gamma \supseteq \Sigma$ is a Work and/or ribbon alphabet with $\Gamma \cap Z = 0$
    -  $\delta: (Z \backslash E)\times\Gamma -> Z\times\{L,R,N\}$ is the partial transfer function
     

2. Configuration:

    -  For a configuration k = $\ a_1 ....a_mzb_1.....b_n$ we set (in case n=0, then $b:= \boxed\;$):
        -  Case 1: $(\delta(z,b_1) = (z',c, N)):k \vdash_M^1 a_1.....a_mz'cb_2.....b_n$
        -  Case 2: $(\delta(z,b_1) = (z',c, R)):k \vdash_M^1 a_1.....a_mcz'b_2.....b_n$
        -  Case 3: $(\delta(z,b_1) = (z',c, R)):$
            - $k \vdash_M^1 a_1.....a_m-1z'cb_2.....b_n$ -> If m>0
            - $k \vdash_M^1z'\boxed \; b_2.....b_n$ -> If m=0









