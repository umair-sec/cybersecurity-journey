# Windows Fundamentals 2: system administration tools

This write-up combines two related posts: the Windows Fundamentals 2 room (1 September) and a follow-up on the admin tools from a SOC perspective (5 September).

## Overview / Objective
Explore Windows' built-in administration and troubleshooting utilities, and understand why they matter for security monitoring.

## Platform & date
| Platform | Room | Dates |
|---|---|---|
| TryHackMe | Windows Fundamentals 2 | 1 September 2026, with a follow-up on 5 September 2026 |

## What I did / key steps
- **`msconfig`**: checked boot configuration and system services
- **`sysdm.cpl`**: hardware management and advanced system properties
- Virtual memory / paging files, and how crash dump files handle system failures
- **`compmgmt.msc`**, **`msinfo32`**, **`resmon`** and **`regedit`**, reviewed again from a SOC point of view

## Key concepts & tools
| Tool | Why it matters for security |
|---|---|
| `regedit` | Monitoring registry keys helps catch persistence |
| `resmon` | Not only a performance tool: it can show unusual network connections from a process |
| `compmgmt.msc` | Event Viewer, Task Scheduler and Local Users in one place, all areas attackers target and defenders should check |
| `msconfig` | Boot configuration and services |
| `msinfo32` | System information |

## Findings / outcome
I had seen most of these tools before but never understood why they matter for security. Now they feel less like random Windows utilities and more like real investigation tools.

## Lessons learned
Windows internals are part of security monitoring and troubleshooting. Attackers target the same places (registry, scheduled tasks, local users) that defenders should check.

---
🔗 Original LinkedIn posts: [1 Sep 2026](https://www.linkedin.com/feed/update/urn:li:activity:7500699519798403072/) · [5 Sep 2026](https://www.linkedin.com/feed/update/urn:li:activity:7501998288045539328/)
