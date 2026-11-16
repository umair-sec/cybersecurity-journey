# Alert Triage With Splunk

## Overview / Objective
Move from a security alert to evidence-based conclusions in Splunk.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Alert Triage With Splunk | 11 November 2026 |

## What I did / key steps
1. **Linux Brute Force**: authentication activity, failed vs successful logins, post-compromise behaviour
2. **Windows Persistence**: malicious Scheduled Task, process/parent-process relationships, attacker discovery activity
3. **Web Shell Exploitation**: malicious web traffic, Hydra brute force against WordPress, interaction with the `b374k.php` web shell (attacker made 4 requests through the web shell)

## Key concepts
Splunk, SIEM, alert triage, Hydra, web shell

## Lessons learned
Follow a structured process: **Alert → Logs → Filtering → Timeline → Correlation → Verdict**.

A suspicious event alone is not enough. Context, timeline and supporting evidence must be correlated before classifying an alert as a True Positive and escalating it.

**Next step:** Keep improving Splunk, SIEM, alert-triage and SOC investigation skills.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7526303110072369153/)
