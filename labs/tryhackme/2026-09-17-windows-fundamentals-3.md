# Windows Fundamentals 3

## Overview / Objective
Understand the security features built directly into the Windows operating system.

## Platform & date
| Platform | Room | Completed |
|---|---|---|
| TryHackMe | Windows Fundamentals 3 | 17 September 2026 |

## What I did / key steps
- Windows Update and Patch Tuesday
- Windows Security and Microsoft Defender: Virus & Threat Protection, real-time and cloud-delivered protection
- Windows Defender Firewall and firewall profiles
- Microsoft Defender SmartScreen
- Core Isolation and Memory Integrity
- Trusted Platform Module (TPM)
- BitLocker Drive Encryption
- Volume Shadow Copy Service (VSS)
- Defence in Depth, Trust but Verify and Zero Trust
- Living Off The Land

## Key concepts
- **BitLocker + TPM + startup key:** BitLocker protects data at rest by encrypting the drive. The TPM provides hardware-based protection for the cryptographic material used during boot. On systems without a compatible TPM, a removable USB startup key can be used instead.
- **Living Off The Land:** attackers abusing built-in Windows utilities to blend in with normal activity.

## Findings / outcome
Legitimate Windows tools are not always used for legitimate purposes. That is why context matters in an investigation: the user, command line, parent process, time and network activity.

## Lessons learned
Knowing the built-in defences, and how they can be bypassed or abused, is part of Windows security fundamentals for a SOC analyst.

---
🔗 [Original LinkedIn post](https://www.linkedin.com/feed/update/urn:li:activity:7506501984884199424/)
