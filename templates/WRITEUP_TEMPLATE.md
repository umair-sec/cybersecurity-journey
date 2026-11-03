# <Lab / room / alert title>

> Copy this file into the right `labs/<platform>/` folder and name it `YYYY-MM-DD-short-title.md`.
> Delete any section that doesn't apply (for example, MITRE mapping for a pure theory room).

## Overview / Objective
What was the goal of this lab or investigation? One or two sentences.

## Platform & date
| Platform | Room / alert | Completed |
|---|---|---|
| TryHackMe / LetsDefend / Splunk home lab / ... | [Name](link) | DD Month YYYY |

## Tools used
- e.g. Splunk (SPL), Kibana (KQL), Event Viewer, Sysmon, Wireshark, CyberChef, VirusTotal, ANY.RUN

## What I did / key steps
1. Step one: what I looked at and why
2. Step two: the pivot I made from the first finding
3. Step three: how I validated the result

Queries used (put reusable ones in [`detections/`](../detections/) too):

```spl
index=<index> sourcetype=<sourcetype> <search terms>
| stats count by <field>
```

## Findings / IOCs
| Type | Value | Notes |
|---|---|---|
| IP / domain / URL | `x.x.x.x` | e.g. C2 server |
| File / hash | `sha256` | e.g. dropped payload |
| Account / host | `user01` / `PC01` | e.g. compromised user |

Verdict: True positive / False positive, and whether it was escalated (and why).

## MITRE ATT&CK mapping
| Technique | Where it appeared |
|---|---|
| T1059.001 Command and Scripting Interpreter: PowerShell | e.g. encoded command in process creation logs |

## Lessons learned
- What I'd do differently next time
- What logging or visibility was missing

---
🔗 [Original LinkedIn post](<link to the LinkedIn post>)
