# Logs Fundamentals

## Overview / Objective
Understand why logs are such an important source of evidence in security investigations, and practise analysing them manually.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Logs Fundamentals | 21 September 2026 |

## What I did / key steps
- Studied the different log types and their use cases: System, Security, Application, Audit, Network and Access logs
- Used Windows Event Viewer and important Event IDs
- Filtered Windows Security logs
- Analysed web server access logs: IP addresses, timestamps, HTTP methods, URLs, status codes and User-Agent strings
- Did manual log analysis with `cat`, `grep` and `less`
- Used logs to investigate suspicious activity and reconstruct what happened during an incident

The practical exercises covered both **Windows Event Logs** and **web server access logs** from different incident scenarios.

## Key concepts & commands
- Windows Event Viewer and Security log filtering
- Web access log fields
- `cat`, `grep`, `less`

## Findings / outcome
Logs are the digital footprints of activity inside a system. They help answer the key investigation questions:
- **Who** performed the activity?
- **What** happened?
- **When** did it happen?
- **Where** did it come from?
- **How** was it carried out?

## Lessons learned
Being able to reconstruct an incident from raw logs, even without a SIEM, is a core SOC analyst skill.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7507944232377147392/)
