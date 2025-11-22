---
id: Tutorium2_RNVS
aliases: []
tags: []
---



1. Layers 

a) 

- Network (Linked) Layer
- Internet Layer
- Transport Layer
- Application Layer

b) 

- Ethernet -> IP -> TCP

c) 

- Sending Port -> Every Browser has their own port (This is used in TCP)
- Receiving Port -> (This is used in UDP)
- Sending address 
- Receiving address

- The hourglass model is used to represent the amount of options we have for each layer
- In the Internet model, it doesn't matter which transport, application or data protection and physical layer implementations for come into use
- As long as IP is supported, various Protocols above and below can be used.


2. DNS
- Names identify an entity (Who)
- Addresses describe where they can be found (Where)

- In the layer model, a value can also take on both roles. 
- In the application layer, 93.184.216.34 is the address for the name example.com, in the network access layer, however, it is a name to which, for example a MAC address, for example.

- Iterative: 

![[Pasted image 20241114145411.png]]


- Recursive: 

![[Pasted image 20241114145644.png]]

- TTL -> Time to Live => The time an input is vaild on a server
- This ensures that the cached information updated correctly

- There are 3 states of Name server records:
    - A -> Saves the Address (IPv4) and hostname
    - NS-Record (Name Server Record) -> Saves which DNS server is required for the correct domain

3.
- In TCP and UDP, ports allow the incoming data packets to be assigned to the correct application. 
- This allows several data streams to be multiplexed on one host.

4.

- Client: No
- Server: Yes

=> Both are always online

