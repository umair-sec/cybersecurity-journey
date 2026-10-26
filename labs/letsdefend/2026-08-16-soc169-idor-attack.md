# SOC169: IDOR attack

## Overview / Objective
Investigate a LetsDefend alert for a possible Insecure Direct Object Reference (IDOR) attack.

## Platform & date
| Platform | Alert | Date | Time to investigate |
|---|---|---|---|
| LetsDefend | SOC169 (IDOR) | 16 August 2026 | ~38 minutes |

## What I did / key steps
1. Investigated the web requests behind the alert.
2. Found that the attacker was **systematically enumerating user IDs** to access unauthorised data.
3. Confirmed it as a **True Positive**.
4. **Escalated to Tier 2.**
5. Contained the host to stop the data leak.

## Findings / outcome
- **Verdict:** True Positive
- **Actions:** escalated to Tier 2 and contained the host

## MITRE ATT&CK mapping
| Technique | Relevance |
|---|---|
| T1190 Exploit Public-Facing Application | IDOR abuse of a web application to access unauthorised data |

## Lessons learned
Following the proper containment and escalation procedures matters. I'm getting more comfortable with the playbooks step by step.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7494902940869005312/)
