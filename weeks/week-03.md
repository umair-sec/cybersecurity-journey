# Week 3: Security+ domains, Splunk, Kill Chain and phishing

**Dates:** September 2026 (Day 1 logged on 4 September, week closed on 27 September)

> Moved from the main README (the content is unchanged) so that each week has its own file.

---

## Week 3 summary

- Domain 2 complete; Domains 3–4 started; Domain 5 nearly complete
- Practice Exam 2 (75 Qs) plus mistake review
- Bandit 22–27 this week (total 0–27)
- Cyber Kill Chain complete ([write-up](../labs/letsdefend/2026-09-03-cyber-kill-chain-module.md)); MITRE ATT&CK started
- Phishing module complete ([write-up](../labs/letsdefend/2026-09-18-phishing-expert-training.md)); alerts **14/90**
- Splunk: install ([write-up](../labs/splunk-home-lab/2026-09-02-splunk-enterprise-setup.md)), basic searches, custom roles

---

## Day 7 (27 September 2026)

### Completed
- **Udemy:** Domain 2 (Architecture) completed
- **Udemy:** Domain 3 started; Domains 4 and 5 continuing in parallel (videos mixed)
- **LetsDefend:** phishing module cases counted, **3 additional alerts** (total **14/90**)
- Week 3 closed

### Security+

| Domain | Status |
|--------|--------|
| Domain 1 (Threats) | Complete |
| Domain 2 (Architecture) | Complete |
| Domain 3 (Implementation) | Started |
| Domain 4 (Operations) | Started |
| Domain 5 (GRC/Compliance) | Nearly complete |

---

## Day 6 (23 September 2026)
- ExamCompass mistake review; Bandit 27; previous alerts reviewed

## Day 5 (20 September 2026)
- Practice Exam 2 (75 Qs); Domain 4 started; phishing module; Bandit 26

## Earlier in Week 3
- Splunk, Kill Chain, MITRE, Security Principles and Bandit 22–25

---

## SOC alerts (LetsDefend: 14/90)

| # | Alert | Type |
|---|-------|------|
| 1–2 | SharePoint / related | True Positive |
| 3 | Lumma Stealer SOC338 | Social engineering / data leak |
| 4–5 | SharePoint ToolShell RCE | RCE |
| 6 | SOC169 IDOR ([write-up](../labs/letsdefend/2026-08-16-soc169-idor-attack.md)) | IDOR (Tier 2) |
| 7 | SOC138 XLS Macro ([write-up](../labs/letsdefend/2026-08-20-soc138-excel-macro-powershell.md)) | Macro → PowerShell → C2 |
| 8–11 | Additional + malware | Solved |
| 12–14 | Phishing module alerts | Phishing / email auth / SOC response |
