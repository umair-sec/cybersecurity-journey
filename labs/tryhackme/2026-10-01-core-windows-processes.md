# Core Windows Processes

## Overview / Objective
Understand what normal Windows process behaviour looks like, so that abnormal behaviour stands out during endpoint investigations.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Core Windows Processes | 1 October 2026 |

## What I did / key steps
Studied the key processes:

| Process | Role |
|---|---|
| `System` | Always PID 4 |
| `smss.exe` | Session Manager |
| `csrss.exe` | Client Server Runtime Process |
| `wininit.exe` | Windows Initialization Process |
| `services.exe` | Service Control Manager |
| `svchost.exe` | Service Host |
| `lsass.exe` | Local Security Authority Subsystem Service |
| `winlogon.exe` | Windows Logon Process |
| `explorer.exe` | Windows Explorer / user shell |

For each process, I practised checking:
- Image path
- Parent process
- User account
- Number of instances
- Start time
- Command line
- Expected parent-child relationships

## Key concepts
- Validating a process by more than its name
- Normal process trees as a baseline

## Findings / outcome
Attackers can **masquerade** as legitimate Windows processes by using the same name or a slightly misspelled one, so a process name alone is never enough.

## MITRE ATT&CK mapping
| Technique | Relevance |
|---|---|
| T1036 Masquerading | Malicious processes using the same or misspelled names as legitimate ones |

## Lessons learned
Knowing normal process trees makes suspicious behaviour much easier to spot during SOC and endpoint investigations.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7511578284552511488/)
