---
id: Tutorium1_Beko
aliases: []
tags: []
---

1.  a)[[Lecture1_BeKo#interpreting-the-actions-of-a-turing-machine|For Definition Look Here]]
	![[Pasted image 20241026174805.png|300]]

    b) $$\ z_0 abb 
    \vdash z_0 bb 
    \vdash aa z_1 b  
    \vdash aab z_1 \square 
    \vdash aa z_2 bc 
    \vdash a z_3 abc 
    \vdash aa z_0 bc 
    \vdash aaa z_1 c 
    \vdash aaac z_1 \square 
    \vdash aaa z_2 cc 
    \vdash aa z_2 acc 
    \vdash aa z_4 acc$$

    c)  $a^* b^+$ <==> ($b^+ == bb^*$)
        $a^* b^i$  i>=1 
    
    d) 
	    $$ 
	    z0bbb ⊢ az1bb ⊢ abz1b ⊢ abbz1□ ⊢ abz2bc ⊢ az3bbc ⊢ z3abbc ⊢ az0bbc ⊢ aaz1bc ⊢ aabz1c ⊢
	    aabcz1□ ⊢ aabz2cc ⊢ aaz2bcc ⊢ az3abcc ⊢ aaz0bcc ⊢ aaaz1cc ⊢ aaacz1c ⊢ aaaccz1□ ⊢
	    aaacz2cc ⊢ aaaz2ccc ⊢ aaz2accc ⊢ aaz4accc
	    $$



        
