# Separating real threats from noise: a Splunk threat-hunting workflow

## Overview / Objective
While practising log investigation and threat hunting in Splunk, one question kept coming up: **how do you separate real threats from thousands of daily logs that are just noise?** Reviewing every log by hand wastes most of the analyst's time.

## Platform & date
| Platform | Date |
|---|---|
| Splunk (home-lab practice) | 6 September 2026 |

## What I did / key steps
1. **Rejected the "filter by IP" approach.** Filtering by IP addresses falls apart quickly because of dynamic IPs (DHCP).
2. **Noise reduction:** filtered out the system's own internal accounts (such as `SYSTEM`), **EventCode 4672**, and routine users. These produce most of the false positives and clutter the view.
3. **Time-based anomaly check:** built a simple baseline of when legitimate users normally log in. A known user authenticating outside their usual working hours stands out immediately.
4. **Focus on Logon Type 10:** instead of only watching the traditional RDP port 3389, I focused on Windows **Logon Type 10** (RemoteInteractive) sessions. Even if an attacker uses a different port or tunnelling, the remote session itself is harder to hide.

## Key concepts
- Windows **EventCode 4672** (special privileges assigned to a new logon), filtered out as noise
- **Logon Type 10**: RemoteInteractive / RDP sessions
- Behavioural baselining of normal logon hours
- Why IP-based filtering is unreliable with DHCP

## Findings / outcome
I ended up with a filter-first workflow: reduce the noise, compare against a baseline, then focus on remote interactive sessions.

## MITRE ATT&CK mapping
| Technique | What the workflow targets |
|---|---|
| T1021.001 Remote Services: Remote Desktop Protocol | Logon Type 10 sessions, whatever the port |
| T1078 Valid Accounts | Known users authenticating at unusual times |

## Lessons learned
A strong SOC analyst isn't the one who looks at every log. It's the one who builds a filter-first mindset and behavioural baselines, so they can go straight to the real threats.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7502522638964084736/)
