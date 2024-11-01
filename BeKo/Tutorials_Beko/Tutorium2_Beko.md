---
id: Tutorium2_Beko
aliases: []
tags: []
---

1. 
    a)
    b)
    c) Does not work because for every number n, we need to find a prime number bigger than n. Therefore if we look at an $\infty$ amount of n's, we would never find a number bigger than n.

2. 

$$
f(n) := \begin{cases} 
1, &\textnormal{is in } \pi \\
0, & \text{else}
\end{cases}
$$


$$
f(n) := \begin{cases} 
1, &\textnormal{n comes n times back to back in } \pi \\
0, & \text{else}
\end{cases}
$$

```Python
def func(n):
    if n<=m:
        return 1
    else:
        return 0
```




