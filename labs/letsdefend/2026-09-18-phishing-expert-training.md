# Phishing Expert training

## Overview / Objective
Learn and practise end-to-end phishing email analysis.

## Platform & date
| Platform | Training | Completed |
|---|---|---|
| LetsDefend | Phishing Expert | 18 September 2026 |

## What I did / key steps
- How phishing attacks work
- The Cyber Kill Chain and the **Delivery** phase
- Email spoofing
- Email header analysis: `From`, `Reply-To`, `Return-Path`, `Received` and `Message-ID`
- Email authentication: **SPF, DKIM and DMARC**
- Identifying suspicious email infrastructure
- Static analysis of URLs, domains and files
- Dynamic analysis in sandbox environments
- IP and domain reputation checks
- How attackers abuse trusted platforms such as Google Drive, Microsoft services, WordPress and Google Forms

## Key concepts
Header fields, SPF/DKIM/DMARC, static vs dynamic analysis, reputation checks and abuse of trusted platforms.

## Findings / outcome
Training completed. The phishing-module alerts brought my LetsDefend alert count to 14 (see [Week 3](../../weeks/week-03.md)).

## MITRE ATT&CK mapping
| Technique | Relevance |
|---|---|
| T1566 Phishing | Main subject of the training |

## Lessons learned
A trusted-looking sender or domain, or even passing email authentication, does **not** automatically mean an email is safe. A proper phishing investigation looks at the complete context.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7506853842240602112/)
