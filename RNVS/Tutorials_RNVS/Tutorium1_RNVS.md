---
id: Tutorium1_RNVS
aliases: []
tags: []
---
# 1. Verzögerung in Kommunikatiosnetzen

- Packages:
    - Packages are used to store and send data from source to destination. This is usually communication between routers. They are broken in smaller pieces. Most packets are stored before being sent. The packet switcher must first receive the who packet before sending it further.

- Propagation Delay:
    - The time needed to propagate from one router to another. How much does it take for the first package to arrive.

- Transmition Delay:
    - The delay is L/R (Length of the package/ Bitrate). This is the amount of time required to push all the packet's bits into the switch/destination.

- Processing Delay:
    - The sender needs time to process all the incoming packets. This is integrated into transmition delay.

- Queuing Delay:
    - The packetes form a queue. The delay represent the time the packets wait in the queue before being transmited between.

## 2. Linientopologie

- p = 10 000 bit 
- r = 100 kbits/s -> $10^5$
- d = 10 ms
- h = 100 bit -- header bits are used to relay type information

- A -> B -> C

a)

-- 2d becasue we have 2 nodes
- delay = 2d = 20 ms = $20 * 10^{-3} s$

- $T= 20 * 10^{-3} + 2 * \frac{10 000 + 100}{10^5} = 222ms$
- $T = 2d + 2(\frac{p+h}{r})$

- $Delay + 2*(\frac{packages}{bit rate})$

b)
- $s = h + \frac{p}{5} = 2100 \text{ bits}$ (2000 bits in 5 packets + 100 bit header), 
- $T = 2d + 6 \frac{s}{r} = 146ms$
-- Tutor did not explain this well not fully sure why it's 6
-- General idea was that we send the 5 packets to B, and 1 to C because idk

c) 
- $T(n) = 2d + (n+1)(h+\frac{p}{n}))/r$ -> $2d + 1/r(hn+h+p+\frac{p}{n}))$

d) 
    - Redundant. -- Again not really explained by the tutor

e)
- $T'(n) = \frac{1}{r*(h-(\frac{p}{n^2}))}$

### 3. Linientopologie
  
#### 4. Forwarding

- r = 4800 $bits/s$
- p = 800000 bit
- d = 20 ms
- Mediation = 300ms
- Handshake = 100ms

##### 5. Paket Übertragung

a) 
- Distance =  200km
- p = 10 000bit
- r = 100 mbit/s
- v = 200 000 km/s
- t = $\frac{1}{1000}s$

=> $\frac{(100bit+10 000bit)}{10^8 bits} = 0.001 s$

b)
  
- $\frac{1}{1000} + \frac{(100bit+10 000bit)}{10^8 bits} = \frac{1}{1000s} + 0.001 s$ 
  


  
