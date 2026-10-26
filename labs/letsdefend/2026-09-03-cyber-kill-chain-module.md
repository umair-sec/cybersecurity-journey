# Cyber Kill Chain module

## Overview / Objective
Go through the 7 phases of the Cyber Kill Chain properly and understand where SOC detection fits in each one.

## Platform & date
| Platform | Module | Completed |
|---|---|---|
| LetsDefend | Cyber Kill Chain | 3 September 2026 |

## What I did / key steps
- Studied all 7 phases of the Cyber Kill Chain
- Mapped which defensive controls realistically detect each phase

## Key concepts
| Phase(s) | Where detection usually comes from |
|---|---|
| Reconnaissance and weaponization | Mostly threat intel and OSINT, not a typical SOC dashboard |
| Exploitation and installation | EDR |
| Command & control | Network monitoring |

## Findings / outcome
Most SOC alerts only catch the middle phases. Reconnaissance and weaponization happen long before any alarm goes off, and by the time C2 traffic is visible, the attacker is already established inside.

## Lessons learned
My mindset changed from "detect everything" to **"detect what you can, understand what you can't"**.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7501384145709735937/)
