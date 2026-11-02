# Splunk 2 (Boss of the SOC v2)

## Overview / Objective
Investigate the Boss of the SOC (BOTS) v2 dataset in Splunk and answer a series of investigation questions, validating each answer with evidence rather than stopping at the first match.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | [Splunk 2](https://tryhackme.com/room/splunk2gcd5?utm_campaign=social_share&utm_medium=social&utm_content=share-completed-room&utm_source=linkedin&sharerId=6a37e7b4889f268cff26ad15) | 28 October 2026 |

## What I did / key steps
1. Practised **SMTP** analysis and **SSL/TCP** investigation in Splunk.
2. Pivoted through **Sysmon**, **Scheduled Tasks** and the **Registry**.
3. Analysed **PowerShell** activity and decoded **Base64 / UTF-16LE** payloads.
4. Validated **C2** traffic and did a final verification of the answer.

Investigation chain:

```
Scheduled Task → PowerShell → Registry → Base64/UTF-16LE decoding → C2 traffic → final verification
```

## Wrong turns (and how I corrected them)
- An `http` match that turned out to be the normal **Sysmon Microsoft schema** URL, not attacker traffic.
- Searches that created more noise than signal.
- A decoded payload pointing to `news.php`, when the question actually asked for the **most contacted** webpage.

Instead of stopping at the first match, I kept validating the evidence. That extra verification led to the correct majority behaviour: **`process.php`**.

## Key concepts
- SPL searches across SMTP, SSL/TCP and Sysmon data
- Scheduled Task and Registry persistence pivots
- Decoding PowerShell `-EncodedCommand` payloads (Base64, UTF-16LE)
- Distinguishing a single indicator from majority behaviour in C2 traffic

## Findings / outcome
- Identified `process.php` as the most contacted C2 webpage after ruling out `news.php`.
- ✅ Room completed.

## MITRE ATT&CK mapping
| Technique | Where it appeared |
|---|---|
| T1053.005 Scheduled Task/Job: Scheduled Task | Scheduled Task used in the attack chain |
| T1059.001 Command and Scripting Interpreter: PowerShell | Encoded PowerShell payload |
| T1112 Modify Registry | Registry pivots |
| T1027 Obfuscated Files or Information | Base64 / UTF-16LE encoding |
| T1071.001 Application Layer Protocol: Web Protocols | C2 traffic to `process.php` |

## Lessons learned
A SOC investigation is rarely a straight line. **Don't hunt for the answer — hunt for evidence, then verify it.**

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7521267904353570816/)
