# SOC282: phishing, "Free Coffee Voucher"

## Overview / Objective
Investigate a phishing email alert and respond to it.

## Platform & date
| Platform | Alert | Date |
|---|---|---|
| LetsDefend | SOC282 (phishing) | 25 August 2026 |

## What I did / key steps
1. Reviewed the email: subject **"Free Coffee Voucher"**, sent to the user **Felix**.
2. Identified the sender `free@coffeeshooop.com` as **typosquatting**, with extra "o"s in the domain.
3. The platform's environment had limitations, so I set up **my own Kali Linux VM** to analyse the suspicious URL safely. I tested the link in an isolated environment, verified how the simulation payload behaved, and continued the investigation workflow.
4. Checked the email headers and flagged the domain and IP (`103.80.134.63`).
5. Deleted the email from Felix's mailbox and closed the alert.

## Findings / outcome
| Item | Value |
|---|---|
| Sender | `free@coffeeshooop.com` (typosquatted domain) |
| IP flagged | `103.80.134.63` |
| Response | Email deleted from the mailbox, alert closed |

## MITRE ATT&CK mapping
| Technique | Relevance |
|---|---|
| T1566.002 Phishing: Spearphishing Link | Phishing email with a malicious URL |

## Lessons learned
Sometimes the built-in tools aren't fully available and you have to rely on your own lab setup. Being resourceful matters as much as following the playbook.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7498004785531404288/)
