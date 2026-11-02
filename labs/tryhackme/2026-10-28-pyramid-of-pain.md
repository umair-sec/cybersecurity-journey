# Pyramid of Pain

## Overview / Objective
Understand the Pyramid of Pain: why detections built on attacker **behaviour** (tools and TTPs) hurt an adversary far more than detections built on easily changed indicators such as hashes, IPs and domains. Then apply the concept through practical investigation.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | [Pyramid of Pain](https://tryhackme.com/room/pyramidofpainax) | 28 October 2026 |

## What I did / key steps
1. Worked up the Pyramid from **Hash Values** and **IP Addresses** through domains, network/host artifacts and tools, all the way to **Tactics, Techniques & Procedures (TTPs)**.
2. Investigated suspicious process and network activity in [ANY.RUN](http://ANY.RUN).
3. Analysed malicious verdicts with **VirusTotal**.
4. Examined **User-Agent strings**, **HTTP POST** activity and C2-related network artifacts.
5. Compared **exact hashing** with **fuzzy hashing (SSDeep)**.
6. Investigated attacker behaviour through **MITRE ATT&CK**.
7. Looked at C2 and data-exfiltration concepts, using **Cobalt Strike** as an example of attacker tooling.

## Key concepts
- The six levels of the Pyramid of Pain: hash values → IP addresses → domain names → network/host artifacts → tools → TTPs
- Exact (cryptographic) hashes vs fuzzy hashes (SSDeep)
- Sandbox analysis (ANY.RUN) and reputation lookups (VirusTotal)
- User-Agent strings and HTTP POST as network artifacts of C2
- MITRE ATT&CK as the language for TTPs

## Findings / outcome
- Seeing the same process communicating over the same port does **not** automatically mean it is connecting to the same destination. The evidence has to be correlated before reaching a conclusion.
- ✅ Room completed.

## MITRE ATT&CK mapping
| Technique | Where it appeared |
|---|---|
| T1071.001 Application Layer Protocol: Web Protocols | HTTP POST / User-Agent C2 artifacts |
| T1041 Exfiltration Over C2 Channel | Data-exfiltration concepts |
| S0154 Cobalt Strike (software) | Example of attacker tooling at the "Tools" level |

## Lessons learned
The most valuable lesson was not a specific IOC or tool, it was the investigation process itself. Before searching for an answer, ask:

> What evidence would prove or disprove my hypothesis, and where should I look for it?

Detecting a hash is useful. Detecting an IP or domain is useful. But detecting **how an attacker operates** is much more powerful: the higher the detection moves up the Pyramid of Pain, the more difficult and costly it becomes for an adversary to adapt.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7521009936252895232/)
