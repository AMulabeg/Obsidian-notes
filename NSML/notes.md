---
id: notes
aliases: []
tags: []
---

- However, widely used encryption techniques (IPSec, TLS/SSL etc.) randomize all the communication contents, which makes the performance of traditional traffic classification methods suffer.
- DNS-based algorithms can immediately classify network flows, requiring just the IP header of the first packet and the information extracted from DNS query-response conversations.
    - However, with the rapid evolution of network protocols over time, some previously unencrypted fields began to be encrypted, reducing the classification performance of these methods (DNS to DOH, TLS1.2 to TLS1.3).
    - These models do not rely on data packet fields, which allows them to be protocol-independent and handle both encrypted and unencrypted traffic. 
