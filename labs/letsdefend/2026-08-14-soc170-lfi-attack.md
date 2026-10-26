# SOC170: Local File Inclusion (LFI) attack

## Overview / Objective
Triage a LetsDefend alert for a possible LFI attack against a web server.

## Platform & date
| Platform | Alert | Date | Time to triage |
|---|---|---|---|
| LetsDefend | SOC170 (LFI) | 14 August 2026 | ~22 minutes |

## What I did / key steps
1. Reviewed the HTTP traffic related to the alert.
2. Found requests targeting sensitive files such as `/etc/passwd`.
3. Confirmed the alert as a **True Positive**.

## Findings / outcome
- **Verdict:** True Positive (LFI attempt targeting sensitive files)
- **Mistake:** I accidentally marked an unplanned test as *planned*, which cost me a few points.

## MITRE ATT&CK mapping
| Technique | Relevance |
|---|---|
| T1190 Exploit Public-Facing Application | LFI against a web application |

## Lessons learned
Pay close attention to every playbook question, not just the final verdict. Every case teaches something new.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7494169623152570368/)
