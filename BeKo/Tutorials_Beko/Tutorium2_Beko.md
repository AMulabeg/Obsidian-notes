---
id: Tutorium2_Beko
aliases: []
tags: []
---

- [~] Finished 
1. 
    a) Yes. Because in any case, we either return 1 or return 0
    b) $$
f(n) := \begin{cases} 
1, &\textnormal{if n > 2 and is a sum of 2 prime numbers} \\
0 & \text{}
\end{cases}
$$

```Python

 A = [True] * (n + 1)
    A[0] = A[1] = False  # 0 and 1 are not primes

    # Loop from 2 up to sqrt(n)
    for i in range(2, int(n**0.5) + 1):
        if A[i]:
            # Mark all multiples of i starting from i^2 as False
            for j in range(i * i, n + 1, i):
                A[j] = False

    # Return all numbers that are still marked True
    primes = [i for i in range(2, n + 1) if A[i]]
    return primes
```
Sieve of Eratosthenes
This works because the numbers are smaller than n

c) Does not work because for every number n, we need to find a prime number bigger than n. Therefore if we look at an $\infty$ amount of n's, we would never find a number bigger than n. This does not work because the numbers are bigger than n

d) Yes it works. We need to prove if p and q or Prime Numbers. Then we can use the algorithm $|p-q|=2$

e) $$
f(n) := \begin{cases} 
1, &\textnormal{if Prime duo exists } \\
0, & \text{}
\end{cases}
$$



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

We check what the upper limit is. Everything over the limit is 0 and everything else is 1.

3.

It's the same because we can simulate 2 tracks in 1. We can make a tupel for all possibilities. 

4. 
