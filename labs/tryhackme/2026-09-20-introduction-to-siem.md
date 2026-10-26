# Introduction to SIEM

## Overview / Objective
Learn how a SIEM brings together logs from different sources and turns individual events into meaningful security context.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Introduction to SIEM | 20 September 2026 |

## What I did / key steps
- Host-centric vs network-centric log sources
- Centralised log collection and ingestion
- Parsing and normalisation of logs
- Correlating events from multiple sources
- How detection rules work and how alerts are triggered
- Investigating the events behind an alert
- Telling **True Positives** from **False Positives**
- Common ingestion methods: agents/forwarders, Syslog, manual uploads and port forwarding

## Key concepts
- Ingestion → parsing/normalisation → correlation → detection rule → alert
- TP vs FP verdicts

## Findings / outcome
The practical lab showed that **an alert alone does not prove an attack**. The analyst has to examine the triggering event, understand the detection rule, correlate the available context, and then decide what actually happened.

## Lessons learned
Always investigate the rule and the raw event behind an alert before giving a verdict.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7507575277531627520/)
