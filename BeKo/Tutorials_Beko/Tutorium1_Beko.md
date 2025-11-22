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

    c)  $a^* b^+ \leftrightarrow (b^+ == bb^*$)
        $a^* b^i$  i>=1 
        $a^{i+j} c^j$
    
    d) 

    4n + 2
    bbb
        
	$$ 
	    z0bbb \vdash az1bb \vdash abz1b \vdash abbz1 \square \vdash abz2bc \vdash az3bbc \vdash z3abbc \vdash az0bbc \vdash aaz1bc \vdash aabz1c \vdash
	    aabcz1 \square \vdash aabz2cc \vdash aaz2bcc \vdash az3abcc \vdash aaz0bcc \vdash aaaz1cc \vdash aaacz1c \vdash aaaccz1 \square \vdash
	    aaacz2cc \vdash aaaz2ccc \vdash aaz2accc \vdash aaz4accc
	$$

    

2. 


![[Pasted image 20251030141311.png]]