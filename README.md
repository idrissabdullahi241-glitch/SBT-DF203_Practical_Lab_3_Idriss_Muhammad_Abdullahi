SBT-DF203 Lab 3: TCP SYN Analysis and Bounded Simulation
2
 
3
## Overview
4
This lab focused on the forensic analysis of TCP SYN activity using Tshark and Apache on a Linux environment. A normal TCP handshake was captured to establish a baseline, followed by a controlled loopback SYN simulation using Scapy. Packet captures were analyzed to identify SYN, SYN-ACK, ACK, and RST behavior and to distinguish normal traffic from incomplete connection attempts.
5
 
6
## Objectives
7
- Analyze normal TCP three-way handshakes.
8
- Identify SYN flood indicators using packet captures.
9
- Extract TCP fields and statistics with Tshark.
10
- Perform a safe loopback-only SYN simulation.
11
- Preserve evidence using SHA-256 hashing.
12
- Develop findings and security recommendations based on observed traffic.
13
 
14
## Tools Used
15
- Apache2
16
- Tshark/Wireshark
17
- Python3
18
- Scapy
19
- Linux Command Line Utilities
20
 
21
## Key Findings
22
- Normal HTTP traffic completed the expected SYN → SYN-ACK → ACK handshake.
23
- The Scapy simulation generated four authorized SYN packets to the local Apache server.
24
- Multiple SYN packets with unique source ports were observed.
25
- No actual denial-of-service condition occurred because the simulation was limited to four packets and executed only on the loopback interface.
26
- Evidence integrity was maintained through SHA-256 hash verification.
27
 
28
## Conclusion
29
The lab successfully demonstrated how to identify TCP connection establishment behavior and recognize patterns associated with SYN-based attacks. Through packet analysis and controlled simulation, key forensic indicators of incomplete handshakes and SYN flooding techniques were examined in a safe and authorized environment.
30
 
31
## Author
**Idriss Muhammad Abdullahi**
33  2025FWSD11475
 
34
**Course:** SBT-DF203 Digital Forensics Lab 3
35
**Topic:** TCP SYN Analysis and Bounded Simulation
