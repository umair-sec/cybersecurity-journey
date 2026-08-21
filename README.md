# 30-Week SOC Analyst Journey

**Goal:** Land my first SOC Analyst (Level 1) role by January 2027  
**Location:** Italy | **Start Date:** August 2026

---

## About Me

- Aspiring SOC Analyst
- Currently studying: CompTIA Security+ (SY0-701)
- Practicing on: TryHackMe, LetsDefend, OverTheWire, CyberDefenders, Splunk
- Tools: Anki (spaced repetition), Wireshark

---

## Current Status (Week 2)

| Metric | Progress |
|--------|----------|
| Security+ | Domain 2 in progress |
| Linux | Bandit Level 15 |
| Networking | OSI 7 Layers + Wireshark basics |
| SOC Alerts | **7/90** solved |
| Anki | 70 cards |

---

## Week 2 – Day 1 (August 21, 2026)

### Completed
- **TryHackMe:** Network Fundamentals completed (OSI 7 Layers)
- **Wireshark:** Installed on Kali Linux + basic capture practice
  - Captured Google DNS (8.8.8.8) ping traffic
  - Analyzed packet structure
- **OverTheWire:** Bandit Level 15 completed
- **LetsDefend:** 7th SOC Alert — SOC138 Suspicious XLS Macro Execution
- **Anki:** 70 total cards

### SOC138 Investigation

| Field | Details |
|-------|---------|
| Case ID | SOC138 |
| Host | Sofi (172.16.17.56) |
| File | order_sheet_spec.xlsm |
| Attack Vector | Malicious macro-enabled Excel |
| Technique | PowerShell with Base64 encoding |
| C2 Communication | Confirmed |
| Containment | Host isolation applied |
| Status | Closed |

**Investigation notes:** Standard logs initially looked incomplete (no clear Process ID, command line, file origin, or outbound traffic). Breakthrough came from Process Name → Process Time → Command Line → Terminal History, which revealed the decoded PowerShell command and confirmed C2.

**Key learning:** When standard logs do not show the full picture, dig deeper. Process Name led to Time, Time led to Command Line, Command Line led to the truth.

---

## Week 1 Complete (Summary)

| Metric | Achieved |
|--------|----------|
| Security+ | Domain 1–2 started |
| Linux | Bandit 0–14, Fundamentals 1–3 |
| SOC Alerts | 6 solved |
| Anki | 60 cards |
| LinkedIn | 17+ connections |
| Practice Test | ExamCompass 89.83% (19/25) |

### SOC Alerts (LetsDefend — now 7/90)

| # | Alert | Type |
|---|-------|------|
| 1 | SharePoint Tool Shell | True Positive |
| 2 | Second alert | True Positive |
| 3 | Lumma Stealer SOC338 | Social Engineering / Data leak |
| 4–5 | SharePoint-related / RCE cases | RCE |
| 6 | SOC169 IDOR Attack | IDOR (Tier 2) |
| 7 | SOC138 Suspicious XLS Macro | Macro → PowerShell → C2 |

---

## Skills Tracker

### Linux
- TryHackMe Linux Fundamentals 1–3
- OverTheWire Bandit 0–15

### Networking
- What is Network? / Intro to LAN / OSI 7 Layers
- Wireshark installed + basic packet capture

### Security+
- Domain 1: largely covered
- Domain 2: in progress (Firewalls/VPNs remaining)

---

## Week 2 Plan (remaining)

| Focus |
|--------|
| Domain 3 (Implementation / Cryptography) |
| More Network Fundamentals + TCP/IP, subnetting |
| Bandit 16+ |
| More LetsDefend alerts |
| Practice questions + Anki |
| Windows Fundamentals (later in week) |

---

## Connect With Me

- LinkedIn: [Umair Ahmed](https://www.linkedin.com/in/umair-ahmed-063a03426)
- GitHub: [umair-sec](https://github.com/umair-sec)

---

*Updated regularly as I progress toward a SOC Analyst role.*
