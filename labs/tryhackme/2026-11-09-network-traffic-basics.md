# Network Traffic Basics

## Overview / Objective
Learn where and how to capture network traffic efficiently.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Network Traffic Basics | 9 November 2026 |

## What I did / key steps
1. Network TAP placement
2. HTTP request/response analysis
3. Web proxy traffic visibility
4. DNS traffic analysis and DNS TXT records
5. Full Packet Capture concepts
6. Logs vs packet captures vs flow metadata
7. NetFlow and IPFIX

## Key concepts
Wireshark, DNS, NetFlow, IPFIX, packet capture

## Lessons learned
Capturing at the firewall/router path shows the traffic but also a huge amount of unnecessary data; narrowing to individual hosts only works if you already know the workstation involved. In the second scenario, information was found inside a DNS TXT record.

> Good traffic analysis is not about capturing everything. It is about capturing the right traffic from the right point.

**Next step:** Balance visibility, efficiency, storage and investigation scope.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7525530635080429569/)
