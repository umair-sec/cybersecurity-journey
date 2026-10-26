# Windows Logging for SOC

## Overview / Objective
Investigate Windows authentication, user-management, Sysmon and PowerShell evidence the way a SOC analyst would. The aim was to build and follow an attack chain, not to memorise Event IDs.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Windows Logging for SOC | 25 October 2026 |

## What I did / key steps
1. **Authentication logs:** I found that a 4624 event with Logon Type 10 was not enough on its own. To identify the actual malicious RDP session, I correlated the **Source IP**, **username** and **Logon ID**.
2. **User-management investigation:** At first I was looking at the wrong log source instead of the provided `.evtx` file. Once I corrected that, I tracked the same **Logon ID** across the authentication events and the account/group changes, and the attack chain became much clearer.
3. **Sysmon:** I tried to use DNS activity to find an exact download URL. Then I realised that a DNS query only shows which domain was resolved, not necessarily where the file was downloaded from.
4. **PowerShell:**
   - I could read the Administrator's PowerShell history. However, when I tried to locate the history file itself, Windows kept opening it directly in Notepad, so I had to browse to the folder to understand where the PSReadLine history is stored.
   - `Get-LocalUser` did not work on the machine, so I used `net user` to list the local accounts instead.
   - I checked Bob's PowerShell history first and found the final flag there.

## Key concepts & commands
- Event ID **4624** (successful logon) with **Logon Type 10** (RemoteInteractive / RDP)
- Correlation on **Source IP + username + Logon ID**
- Working from the provided `.evtx` file, not the live logs
- Sysmon DNS query events: they show the domain resolved, not the download URL
- PSReadLine PowerShell history file
- `net user` (used as a fallback when `Get-LocalUser` failed)

## Findings / outcome
- Identified the malicious RDP session by correlation, not from a single event.
- Linked authentication activity to account/group changes through the shared Logon ID.
- Found the final flag in Bob's PowerShell history.
- ✅ Room completed.

## MITRE ATT&CK mapping
| Technique | Where it appeared |
|---|---|
| T1021.001 Remote Services: Remote Desktop Protocol | Malicious RDP session (Logon Type 10) |
| T1098 Account Manipulation | Account/group changes tied to the attacker's Logon ID |
| T1059.001 Command and Scripting Interpreter: PowerShell | PowerShell activity reviewed through PSReadLine history |

## Lessons learned
SOC investigation is not about knowing one perfect Event ID. For each step I ask three questions:
- What evidence do I need?
- Where should I look for it?
- How can I correlate it with the rest of the activity?

Choosing the **correct evidence source** (the `.evtx` file instead of the live logs, process/network events instead of DNS) matters as much as the query itself.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7520263933358923776/)
