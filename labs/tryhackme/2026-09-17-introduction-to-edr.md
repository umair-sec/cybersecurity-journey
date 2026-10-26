# Introduction to Endpoint Detection & Response (EDR)

## Overview / Objective
Learn how EDR gives much deeper endpoint visibility than traditional antivirus, and how SOC analysts use endpoint telemetry to investigate suspicious activity.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Introduction to EDR | 17 September 2026 |

## What I did / key steps
- EDR architecture: agents/sensors and the central console
- Investigated process trees and parent-child relationships
- Analysed process, command-line, network, file and registry telemetry
- Detection methods: behavioural and anomaly-based detection, IOC matching, MITRE ATT&CK mapping and machine learning
- Response actions: host isolation, process termination, quarantine and remote response
- Practised alert investigation in a simulated environment, tracing **payload downloads** and **data-exfiltration attempts**

## Key concepts
- Endpoint telemetry types
- Process trees
- Containment actions

## Findings / outcome
In the simulated environment I traced payload downloads and data-exfiltration attempts by correlating endpoint telemetry.

## Lessons learned
A single event rarely tells the full story. To understand the complete attack chain, you have to correlate process behaviour, network activity, IOCs and endpoint context.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7506472464399400961/)
