# 30-Week SOC Analyst Journey

**Goal:** land my first SOC Analyst (Level 1) role by January 2027  
**Location:** Italy | **Start date:** August 2026

I'm Umair Ahmed, an aspiring SOC Analyst currently studying for **CompTIA Security+ (SY0-701)**. This repository documents my 30-week journey in public: hands-on lab write-ups from TryHackMe, LetsDefend and my Splunk home lab, plus weekly progress logs.

---

## 📁 Repository structure

```
cybersecurity-journey/
├── labs/
│   ├── tryhackme/        # SOC Level 1 path rooms and modules
│   ├── letsdefend/       # SOC alert investigations and training modules
│   └── splunk-home-lab/  # My own Splunk Enterprise lab
├── weeks/                # Weekly progress logs
└── README.md
```

Each lab write-up follows the same structure: **Objective → Platform & date → Key steps → Key concepts / commands → Findings → MITRE ATT&CK (where applicable) → Lessons learned → link to the original LinkedIn post**.

---

## 📊 Current status (last weekly log: Week 3, 27 September 2026)

| Metric | Progress |
|--------|----------|
| Security+ | Domains 1–2 complete; Domains 3–4 started; Domain 5 nearly complete |
| Linux | OverTheWire Bandit level **27** |
| Practice exams | Exam 1 (50 Qs) + Exam 2 (75 Qs) + mistake review |
| SOC alerts | **14/90** on LetsDefend |
| LetsDefend | Cyber Kill Chain complete; Phishing Expert complete; MITRE ATT&CK in progress |
| TryHackMe | SOC Level 1 path in progress (latest: Windows Logging for SOC, 25 October 2026) |
| Anki | **100** cards |

---

## 🧪 Lab write-ups

| Date | Platform | Lab | Focus |
|------|----------|-----|-------|
| 2026-08-11 | TryHackMe | [Linux Fundamentals Part 3](labs/tryhackme/2026-08-11-linux-fundamentals-part-3.md) | Permissions, find/grep/awk, processes |
| 2026-08-14 | LetsDefend | [SOC170: LFI attack](labs/letsdefend/2026-08-14-soc170-lfi-attack.md) | Web attack triage |
| 2026-08-16 | LetsDefend | [SOC169: IDOR attack](labs/letsdefend/2026-08-16-soc169-idor-attack.md) | Web attack, Tier 2 escalation |
| 2026-08-20 | LetsDefend | [SOC138: Excel macro → PowerShell](labs/letsdefend/2026-08-20-soc138-excel-macro-powershell.md) | Malware, process lineage |
| 2026-08-24 | TryHackMe | [Network Fundamentals](labs/tryhackme/2026-08-24-network-fundamentals.md) | OSI, LAN, firewalls |
| 2026-08-25 | LetsDefend | [SOC282: "Free Coffee Voucher" phishing](labs/letsdefend/2026-08-25-soc282-phishing-free-coffee-voucher.md) | Phishing, typosquatting, Kali VM |
| 2026-08-27 | TryHackMe | [SOC Role in Blue Team](labs/tryhackme/2026-08-27-soc-role-in-blue-team.md) | SOC roles, L1 vs L2 |
| 2026-08-30 | TryHackMe | [Humans as Attack Vectors](labs/tryhackme/2026-08-30-humans-as-attack-vectors.md) | Social engineering |
| 2026-08-30 | TryHackMe | [Windows Fundamentals 1](labs/tryhackme/2026-08-30-windows-fundamentals-1.md) | NTFS, UAC |
| 2026-09-01 | TryHackMe | [Systems as Attack Vectors](labs/tryhackme/2026-09-01-systems-as-attack-vectors.md) | Vulnerabilities vs misconfigurations |
| 2026-09-01 | TryHackMe | [Windows Fundamentals 2](labs/tryhackme/2026-09-01-windows-fundamentals-2.md) | Admin tools from a SOC view |
| 2026-09-02 | Splunk home lab | [Splunk Enterprise setup](labs/splunk-home-lab/2026-09-02-splunk-enterprise-setup.md) | Local SIEM |
| 2026-09-03 | TryHackMe | [SOC L1 Alert Triage](labs/tryhackme/2026-09-03-soc-l1-alert-triage.md) | Triage lifecycle |
| 2026-09-03 | LetsDefend | [Cyber Kill Chain](labs/letsdefend/2026-09-03-cyber-kill-chain-module.md) | Detection coverage |
| 2026-09-04 | TryHackMe | [SOC L1 Alert Reporting](labs/tryhackme/2026-09-04-soc-l1-alert-reporting.md) | 5 Ws, escalation |
| 2026-09-06 | Splunk home lab | [Threat-hunting noise-reduction workflow](labs/splunk-home-lab/2026-09-06-noise-reduction-threat-hunting-workflow.md) | Baselines, Logon Type 10 |
| 2026-09-09 | TryHackMe | [SOC Workbooks & Lookups](labs/tryhackme/2026-09-09-soc-workbooks-and-lookups.md) | Enrichment, context |
| 2026-09-10 | Splunk home lab | [plink.exe / Event ID 4688 investigation](labs/splunk-home-lab/2026-09-10-plink-event-4688-investigation.md) | Process lineage, logging gaps |
| 2026-09-12 | TryHackMe | [SOC Metrics and Objectives](labs/tryhackme/2026-09-12-soc-metrics-and-objectives.md) | MTTD/MTTA/MTTR |
| 2026-09-17 | TryHackMe | [Introduction to EDR](labs/tryhackme/2026-09-17-introduction-to-edr.md) | Endpoint telemetry |
| 2026-09-17 | TryHackMe | [Security Principles](labs/tryhackme/2026-09-17-security-principles.md) | CIA/DAD, Zero Trust |
| 2026-09-17 | TryHackMe | [Windows Fundamentals 3](labs/tryhackme/2026-09-17-windows-fundamentals-3.md) | Defender, BitLocker, TPM |
| 2026-09-18 | LetsDefend | [Phishing Expert training](labs/letsdefend/2026-09-18-phishing-expert-training.md) | Headers, SPF/DKIM/DMARC |
| 2026-09-20 | TryHackMe | [Introduction to SIEM](labs/tryhackme/2026-09-20-introduction-to-siem.md) | Ingestion, correlation, TP/FP |
| 2026-09-21 | TryHackMe | [Logs Fundamentals](labs/tryhackme/2026-09-21-logs-fundamentals.md) | Windows and web logs |
| 2026-09-24 | TryHackMe | [Splunk: The Basics](labs/tryhackme/2026-09-24-splunk-the-basics.md) | SPL, VPN logs |
| 2026-10-01 | TryHackMe | [Core Windows Processes](labs/tryhackme/2026-10-01-core-windows-processes.md) | Normal process trees |
| 2026-10-01 | TryHackMe | [Elastic Stack (ELK)](labs/tryhackme/2026-10-01-elastic-stack-elk.md) | Kibana, KQL, dashboards |
| 2026-10-05 | TryHackMe | [Introduction to Cryptography](labs/tryhackme/2026-10-05-introduction-to-cryptography.md) | PKI, TLS, hashing |
| 2026-10-09 | TryHackMe | [Introduction to SOAR](labs/tryhackme/2026-10-09-introduction-to-soar.md) | Playbooks, automation |
| 2026-10-20 | TryHackMe | [Windows Event Logs](labs/tryhackme/2026-10-20-windows-event-logs.md) | Validating evidence |
| 2026-10-25 | TryHackMe | [Windows Logging for SOC](labs/tryhackme/2026-10-25-windows-logging-for-soc.md) | RDP, Sysmon, PowerShell |

---

## 🗓️ Weekly logs

| Week | Log | Notes |
|------|-----|-------|
| Week 1 | [week-01.md](weeks/week-01.md) | Linux Fundamentals 1–3, Bandit 0–14, first 6 SOC alerts, ExamCompass 89.83% |
| Week 2 | [week-02.md](weeks/week-02.md) | Domain 1 complete, Bandit 0–21, 11 alerts, SOC Level 1 path started |
| Week 3 | [week-03.md](weeks/week-03.md) | Domain 2 complete, Bandit 27, Kill Chain, phishing module, 14 alerts |
| Week 4+ | *Not yet written* | Lab work from late September onwards is documented in the lab write-ups above |

---

## 🛠️ Skills & tools

- **SIEM / log analysis:** Splunk (SPL, home lab), Elastic Stack / Kibana (KQL), Windows Event Viewer
- **Windows:** Security Event IDs (4624, 4672, 4688), Sysmon, PowerShell history (PSReadLine), core process analysis
- **Endpoint:** EDR concepts, process trees, containment actions
- **Email security:** header analysis, SPF/DKIM/DMARC, URL/domain reputation, sandbox analysis
- **SOC process:** alert triage, reporting (5 Ws), escalation, workbooks, SOC metrics, SOAR playbooks
- **Frameworks:** Cyber Kill Chain, MITRE ATT&CK
- **Linux & networking:** OverTheWire Bandit, Kali Linux, Wireshark, OSI/TCP-IP, firewalls
- **Study:** Anki spaced repetition, ExamCompass practice tests

## 🎓 Certifications

| Certification | Status |
|---|---|
| CompTIA Security+ (SY0-701) | 📖 In progress |

## 🎯 Platforms

TryHackMe (SOC Level 1 path) · LetsDefend · OverTheWire · CyberDefenders · Splunk home lab

---

## 🤝 Connect with me

- LinkedIn: [Umair Ahmed](https://www.linkedin.com/in/umair-ahmed-063a03426)
- GitHub: [umair-sec](https://github.com/umair-sec)

---

*Updated regularly as I progress toward a SOC Analyst role. Licensed under [MIT](LICENSE).*
