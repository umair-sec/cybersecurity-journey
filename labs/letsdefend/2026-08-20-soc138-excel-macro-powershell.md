# SOC138: Excel macro spawning PowerShell

## Overview / Objective
Investigate a LetsDefend alert for a malicious Excel macro that launched PowerShell.

## Platform & date
| Platform | Alert | Date |
|---|---|---|
| LetsDefend | SOC138 (Excel macro) | 20 August 2026 |

## What I did / key steps
1. **Endpoint Security:** At first there was no PID, no execution time and no command line, only the process name. I pivoted on the process name and eventually recovered the timeline and the **full PowerShell command that Excel had spawned**.
2. **Payload:** The PowerShell payload was **base64-encoded and heavily obfuscated**, a classic evasion technique. The file name was `order_sheet_spec.xlsm`.
3. **Delivery vector:** I checked Email Security, endpoint logs, file logs and network connections, and most came up empty.
   - **Terminal history** showed the encoded PowerShell commands.
   - **Browser history** was clean, so the delivery vector remained unknown.
4. **Response:** I flagged the file hash and the C2 URL, isolated the host **Sofi (172.16.17.56)**, and closed the playbook.

## Key concepts
- Pivoting on the process name when PID, time and command line are missing
- Process lineage: `Excel → PowerShell`
- Encoded/obfuscated PowerShell

## Findings / outcome
| Item | Value |
|---|---|
| Malicious file | `order_sheet_spec.xlsm` |
| Behaviour | Excel spawned PowerShell with a base64-encoded, obfuscated payload |
| Affected host | Sofi, 172.16.17.56 (isolated) |
| IOCs flagged | File hash and C2 URL |
| Delivery vector | Not determined: email, file and browser evidence did not show it |

## MITRE ATT&CK mapping
| Technique | Relevance |
|---|---|
| T1204.002 User Execution: Malicious File | Macro-enabled `.xlsm` file |
| T1059.001 Command and Scripting Interpreter: PowerShell | Excel spawned PowerShell |
| T1027 Obfuscated Files or Information | Base64-encoded, obfuscated payload |

## Lessons learned
- Process lineage matters. Excel spawning PowerShell is a red flag you can't ignore.
- When the logs don't tell the full story, keep digging until something clicks. Sometimes it doesn't, and you learn to document the gap honestly.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7496352065653248000/)
